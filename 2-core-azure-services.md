# Compute Services

* Virtual Machines (like AWS EC2 Instances)
* Container Instances (like AWS ECS)
* App Services
* Serverless Computing (Functions, like AWS Lambda)

## Virtual Machines (IaaS)

Images (like AWS AMI)

Scaling 
* Scale Set
    * Centrally manage, configure and update large number of VMs
    * Auto Scaling
    * Highly Availabile apps
* Batch
    * HPC (High Performance Computing)
    * Enables large-scale parallel and HPC batch jobs, with ability to scale

## Containers and Kubernetes

*VM - Virtualizes the Hardware, Containers - Virtualizes the OS

Deploy and manage containers (lightweight, virtualized application environments)

Run multiple instances of an application on a single host machine

* Container Instances
* Kubernetes Services (Orchestrator)
* Microservices (loosely coupled)

## App Services (PaaS)

Build and scale web, mobile and API apps

WebJobs - enables to run program (EXE, JAVA, Node JS) or scripts (.cmd, .bat, powershell)

## Severless Computing

Work in response to an event, timer or a request from other Azure service

Benefits
* No Infra Management
* Scalability
* Only pay for what u use

### FUNCTIONS
Can **execute code** in almost any modern language.

Can be either stateless or stateful. 

When stateless (the default), they behave as if they're restarted every time they respond to an event. 

When stateful (called Durable Functions), a context is passed through the function to track prior activity
### LOGIC APPS
Executes **workflows** (persisted as JSON files)

Designed in a GUI and can execute logic triggered by Azure services without writing any code


### Functions vs Logic Apps
|| **Functions** | **Logic Apps**
|:---|:---|:---|
State|Normally stateless, but Durable Functions provide state|Stateful.
Development|Code-first (imperative)|Designer-first (declarative).
Connectivity |About a dozen built-in binding types|Write code for custom bindings.

Large collection of connectors. Enterprise Integration Pack for B2B scenarios. Build custom connectors.

#### Actions

Each activity is an Azure function. Write code for activity functions.

Large collection of ready-made actions.

#### Monitoring

Azure Application Insights.

Azure portal, Log Analytics.

#### Management

REST API, Visual Studio.

Azure portal, REST API, PowerShell, Visual Studio.

#### Execution context

Can run locally or in the cloud.

Runs only in the cloud.
