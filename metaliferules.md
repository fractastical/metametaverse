#The game of metalife 

Metalang has the following functions

Create a lifeform by passing it a function and a certain amount of energy. 

create(rand(x,y,z),f(x), energy)

Life performs its function at each computational step. Certain actions require energy, namely creating new life. 

Each life form can alter any adjacent space in the x y or z coordinates such that

create((x+1,y+1,z), f(x), energy)

A new life form is passed as much energy as desired by its parent, but it cannot exceed the parent’s total amount of energy. 

In short, if the parent had the value of energy of 10 and called create((x+1,y+1,z), f(x), 3) 

This would deduct 4 energy from parent (1 by calling create, 3 passed to the child) and leave the child with 3 energy.  

Additionally, there may be fuel at any coordinates upon which a new lifeform is created. If so, this fuel is added to the total fuel of the lifeforms.

Additionally, if a lifeform attempts to create a lifeform on top of a place where another lifeform exists, that lifeform is destroyed and all of its energy is absorbed into the new lifeform. 


Default conditions:

Life = 100 
Randomly dispersed fuel: 100,000 nuggets of 10 each.
By default, each parent lifeform has a color and all its children retain that color 
Any invalid function call is not called but subtracts one energy
Valid operands: if/then, modulus, plus, minus, and create  
Each entry submits a function. 
Winner is the one with most populated color at the end of 1,000 computational steps. 


==
 Metalang has the follow operations: 
- Goto (by default an object can only go to the next coordiante in the coordinate space)
- Absorb (take on the energy and composition of another life form that exists in that space)
- Insert (add an object to that space) 

 
