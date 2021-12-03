# Batch Flow Model of a Bakery

## Model Stub
The Batch Flow problem generally is one of scheduling. **Batches** are sequences of **tasks** that must be performed in a certain order. Each task requires a 
specific **machine** to complete its task. The crux of the problem is that the same machine is often required by different tasks; jobs will require many of the same
machines and thus each job must be prioritzed. The goal is to minimize the **makespan** - the length of time all the jobs, processed one after another, will take.

In the realm of a bakery, the batch flow problem is an applicable model for batch scheduling. 

Maybe link this README.md to separate pages.

**can we do two machines at the same time**
**how are immediate tasks handled - can things be left to wait if needed?**

## Model in Context
This part will build on the understanding developed in the [Model Stub](#Model-Stub)

### Assumptions
Several simplifying assumptions have been made. These assumptions not only change what the model truly represents, but also may make the model more generally 
applicable than it was previously.
- Assumptions

### Mathematical Framework
The mathematical framework necessary to create a Model Simulation: relate each of the assumptions to a part of the math (if an assumption cannot connect to the 
math, explicitly state why it is still of value to include).
- “First Principles” models describe a causal interaction that explains the model behavior (and possibly structure)
- These are performed in sequence
- What does a job shop do
- What 

#### Yields
- M1: Mixer - Raw dough (D)
- M2: Balling - Condensed or Ready-to-bake Trays (T<sub>c</sub> or T<sub>r</sub>) 35 or 12 cookies
- M3: Decondensing - Ready-to-bake Trays (T<sub>r</sub>) 12 cookies
- M4: Oven - Baked trays of cookies (T<sub>b</sub>) 12 cookies

#### Times
| Machines |Cookie 1|Cookie 2|Cookie 3|
| -------- | ------ | ------ | ------ |
| Mixer (M1)        | 20 min | 20 min | 20 min |
| Balling (M2)      | 6 min  | 17 min | 17 min |
| Decondensing (M3) |    -   | 5 min  | 5 min  |
| Oven (M4)         | 14 min | 14 min | 16 min |

#### Quantities
| Machine |Cookie 1|Cookie 2|Cookie 3|
| ------- | ------ | ------ | ------ |
| Mixer (M1)        | 320 oz D| 320 oz D| 320 oz D|
| Balling (M2)      | 1 T<sub>ready</sub> | 1 T<sub>condensed</sub> | 1 T<sub>condensed</sub> |
| Decondensing (M3) |        -            | 1 T<sub>ready</sub> | 1 T<sub>ready</sub> |
| Oven (M4)         | 1 T<sub>baked</sub> | 1 T<sub>baked</sub> | 1 T<sub>baked</sub> |

### Validation
Validation of models is an important—how would we know if this model is a good one?

### References
References—cite important works that give more thorough descriptions of part or all of the model being considered

[Google OR-Tools](https://developers.google.com/optimization/scheduling/job_shop)

## Model Simulation
Refer to the included .py file...

## Examples
Walk through how the model in context and model simulation work in a simple example scenario.  This may use real (empirical) or synthetic (handmade) data.

