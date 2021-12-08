# Batch Flow Model of a Bakery

## Model Stub
The Batch Flow problem generally is one of scheduling. For any given **job** there is a sequence of **tasks** that must be performed in a certain order. Each task requires a specific **machine** to complete its task. The crux of the problem is that the same machine is often required by different tasks; jobs will require many of the same machines and thus each job must be prioritzed. The goal is to minimize the **makespan** - the length of time all the jobs, processed one after another, will take. In the realm of a bakery, batch flow shop methods are an applicable model for job scheduling. Some machines will run in parallel, others will not. 

## Model in Context
This part will build on the understanding developed in the [Model Stub](#Model-Stub)

### Assumptions
Several simplifying assumptions have been made. These assumptions not only change what the model truly represents, but also may make the model more generally 
applicable than it was previously.
- No intermediate storage
- Varying batch sizes (Linearly scaling, 1x, 2x or 3x)
- Job processing will flow through a factory in workstation order
- Not all machines will be utilized by a given job
- All jobs end on the same workstation
- All machines in a given workstation are the same type
- No intermediate storage

### Mathematical Framework
The mathematical framework necessary to create a Model Simulation: relate each of the assumptions to a part of the math
- Though a job doesn't 
- What does a job shop do
Future work in this section

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
| Oven (M4)         | 8 T<sub>baked</sub> | 8 T<sub>baked</sub> | 8 T<sub>baked</sub> |

### References
[Google OR-Tools](https://developers.google.com/optimization/scheduling/job_shop)
[Model approximation for batch flow shop scheduling with fixed batch sizes](https://idealabs.byu.edu/publications/2013BatchFlowAproximation.pdf)
[intuit Quickbooks](https://quickbooks.intuit.com/r/growing-complex-businesses/batch-flow-continuous-and-custom-production-in-manufacturing/)

## Model Simulation
Future work

## Examples
Future work

