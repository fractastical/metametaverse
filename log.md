Start of day 1 of the MetaEra (June 27)

<img width="446" alt="initial_render" src="https://user-images.githubusercontent.com/589191/176097315-593098e9-6170-4412-9021-5942ac544633.png">

End of day 1

<img width="410" alt="day1_render" src="https://user-images.githubusercontent.com/589191/176097275-e4305212-8086-4cbb-a5b2-13587af9743c.png">

28 June. First lambda selectors  


<img width="565" alt="Screenshot 2022-06-28 at 12 08 02" src="https://user-images.githubusercontent.com/589191/176228075-7b9f72ca-d933-4fd9-8277-01502a55553f.png">

First game

<img width="525" alt="Screenshot 2022-06-28 at 13 09 20" src="https://user-images.githubusercontent.com/589191/176242235-c6e0515f-7d0e-40e2-8e5b-52592a742c16.png">

with energy

<img width="752" alt="Screenshot 2022-06-28 at 15 55 39" src="https://user-images.githubusercontent.com/589191/176273342-d3d68f62-68f3-49d3-9918-180977d585eb.png">


Chaotic functions


<img width="594" alt="Screenshot 2022-06-28 at 17 54 20" src="https://user-images.githubusercontent.com/589191/176306987-be623920-a166-4827-92cc-3cf768bae612.png">

Allow dynamic insertion of custom lambdas 




<img width="218" alt="Screenshot 2022-06-28 at 20 50 03" src="https://user-images.githubusercontent.com/589191/176327950-937895cb-d324-4729-9e9f-adee6eefae65.png">


First time we have a clear winner


<img width="743" alt="Screenshot 2022-06-28 at 23 21 46" src="https://user-images.githubusercontent.com/589191/176344370-b45be0ff-39d7-4b6c-a871-f960055814fb.png">

Pseudocode for metalambda controller 

<img width="790" alt="Screenshot 2022-07-09 at 20 14 47" src="https://user-images.githubusercontent.com/589191/178119831-72b5758b-69b2-46fd-8a48-713a505cfacb.png">


Metalambdas now working with seeds and win counts. 

<img width="435" alt="Screenshot 2022-07-10 at 02 24 26" src="https://user-images.githubusercontent.com/589191/178125663-284ec27e-731f-4488-92a3-237ad6ce0050.png">

Arbitrary number of CAs each working with metalambda seeds. 

<img width="245" alt="Screenshot 2022-07-10 at 13 38 16" src="https://user-images.githubusercontent.com/589191/178141387-5820137c-446b-4cd9-9ce8-ffbffa539d29.png">

Added logging. Running about 40ms per computatational step. 

<img width="288" alt="Screenshot 2022-07-10 at 14 20 13" src="https://user-images.githubusercontent.com/589191/178142756-3d1d9f36-3568-414f-9441-07831429b207.png">

Knocked off about 10 ms per step. 

<img width="697" alt="Screenshot 2022-07-10 at 17 09 33" src="https://user-images.githubusercontent.com/589191/178148474-558a2a3b-2190-4c3b-ba1d-7329535b3bc9.png">

Creating system for logging all winners (and more involved system for generating metalambda seeds). 

<img width="611" alt="Screenshot 2022-07-10 at 23 10 28" src="https://user-images.githubusercontent.com/589191/178161165-1404a0ef-eb68-4158-8b9e-7853347761f1.png">

Combat mode partially working (spaceships with rays modifying the environment). 

<img width="522" alt="Screenshot 2022-07-11 at 17 09 23" src="https://user-images.githubusercontent.com/589191/178284011-0b68b659-5204-4608-887f-464c01f28ce8.png">

In line editor for lambda control functions

<img width="708" alt="Screenshot 2022-07-11 at 18 24 15" src="https://user-images.githubusercontent.com/589191/178299956-5fe6a610-c37e-49c6-a3b7-521aadaba7b7.png">

Combat mode now officially works (counting hits). 

Recent "progress" has been in determining a metalayer for the mutation of the rules, securing compute resources to do large scale simuilations, auditing existing computational biology software, and considering a full or partial re-write in a faster language (e.g. Rust). Also considering rolling back the random elements and making it fully deterministic at the level of an individual simulation, partially for the reason that you always reach the same final state and this also allows multiple client implementation (and potentially a solution to proof-of-excellence). Also added some idle game-esque dynamics. 

Academic paper draft ready for circluation 
