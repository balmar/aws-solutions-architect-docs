#Decoupling 
[[Serverless]] orchestration service, which allows for building your application workflows in a graphical console.
### Types of workflows
#### Standard
* Has exactly one [[State Machine Execution|Execution]]
* Can run for up to one year
* Useful for long-running workflows, which need an auditable history
* Rates up to 2000 [[State Machine Execution|executions]] per second
* Pricing based per state transition
#### Express
* At-least-once workflow execution
* Can run for up to 5 minutes
* Useful for high-event-rate workloads
* Example use is IoT data streaming and ingestion
* Pricing based on numbers of executions, durations and memory consumed
### Language
States and workflows are defined in [[Amazon States Lanugage]].
### States
States are elements within your [[State Machine]]. They are referred by name.
#### State types
* *Pass* - passes input directly to output
* *Task* - Single unit of work
* *Choice* - Conditional branch logic
* *Wait* - Time delay
* *Succeed* - stops executions successfully
* *Fail* - Stops executions as failures
* *Parallel* - runs two or more branches in parallel
* *Map* - runs a set of steps on an array of inputs
### Related
[[State Machine]]
[[Step Task|Task]]

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/57f49ecc-1678-4aab-ae83-241a03d0d1f2/watch