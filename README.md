# Job Shop Model of a Bakery

## Model Stub
The background information necessary to create one or various models in context.  It tells “the story setting without math”.  It gives key terms and introductory 
context to someone who has not been exposed to the set of ideas, and motivation behind why a model from this stub would be valuable to study.

The Job Shop problem generally is one of scheduling. **Jobs** are sequences of **tasks** that must be performed in a certain order. Each task requires a 
specific **machine** to complete its task. The crux of the problem is that the same machine is often required by different tasks; jobs will require many of the same
machines and thus each job must be prioritzed. The goal is to minimize the **makespan** - the length of time all the jobs, processed one after another, will take.

In the realm of a bakery, the job shop problem is an applicable model for batch scheduling. 

Maybe link this README.md to separate pages.

**can we do two machines at the same time**
**how are immediate tasks handled - can things be left to wait if needed?**

## Model in Context
This part will build on the understanding developed in the [Model Stub](#Model-Stub)

### Assumptions
Several simplifying assumptions have been made. These assumptions not only change what the model truly represents, but also may make the model more generally 
applicable than it was previously.
- An explicit list of assumptions made 
- What is included that is not mentioned in the Model stub, and why?  
- What is not included that is mentioned in the Model stub, and why not?

### Mathematical Framework
The mathematical framework necessary to create a Model Simulation: relate each of the assumptions to a part of the math (if an assumption cannot connect to the 
math, explicitly state why it is still of value to include).
- “First Principles” models describe a causal interaction that explains the model behavior (and possibly structure)
- “Black Box” models might have predictive value but otherwise may not explain much about how the phenomenon actually generates its behavior.

### Validation
Validation of models is an important—how would we know if this model is a good one?

### References
References—cite important works that give more thorough descriptions of part or all of the model being considered

[Google OR-Tools](https://developers.google.com/optimization/scheduling/job_shop)

## Model Simulation
Refer to the included .py file...

## Examples
Walk through how the model in context and model simulation work in a simple example scenario.  This may use real (empirical) or synthetic (handmade) data.

