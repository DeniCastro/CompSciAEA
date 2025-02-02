# CASE OF... OTHERWISE... ENDCASE  
For a **CASE** statement the value of a variable decides the path to be taken.  
Several values are usually specified. **OTHERWISE** is the path taken for all other values. The end of the statement is shown by **ENDCASE**.  

Have a look at the algorithm below that specifies what happens if the value of **Choice** is **1**, **2**, **3** or **4**.  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/CASE%20OF%20Choice.jpg" alt="CASE OF Choice" width="500"> 
</div>
  
## The pseudocode for iteration  
When some actions performed as part of an algorithm need repeating this is called iteration. Loop structures are used to perform the iteration.  
Pseudocode includes these three different types of loop structure:  

A set of number of repetitions **FOR ... TO ... NEXT**  
A repetition, where the number of repeats is not known, that is completed at least once: **REPEAT ... UNTIL**  
A repetition, where the number of repeats is not known, that may never be completed: **WHILE ... DO ... ENDWHILE***  

All types of loops can all perform the same task, for example displaying ten stars:  
  
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/loop_structure.jpg" alt="CASE OF Choice" width="500"> 
</div>

## FOR ... TO... NEXT loops  
A variable is set up, with a start value and an end value, this variable is incremented in steps of one until the end value is reached and the iteration finishes. The variable can be used within the loop so long as its value is not changed. This type of loop is very useful for reading values into lists with a known length.    

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/for...to...next%20loops.jpg" alt="FOR ... TO... NEXT Loops" width="500"> 
</div>  

## REPEAT ... UNTIL loop  
This loop structure is used when the number of repetitions/iterations is not known and the actions are repeated **UNTIL*** a given condition becomes true. The actions in this loop are always completed at least once. This is a post-condition loop as the test for exiting the loop is at the end of the loop.  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/REPEAT...%20UNTIL...%20loop.jpg" alt="REPEAT ... UNTIL" width="500"> 
</div>    
  
## WHILE ... DO ... ENDWHILE loop  
This loop structure is used when the number of repetitions/iterations is not known and the action are only repeated **WHILE** a given condition is true. If the **WHILE** condition is untrue then the actions in this loop are never performed. This is a pre-condition loop as the test for exiting the loop is at the beginning of the loop.  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/WHILE...%20DO...%20ENDWHILE%20loop.jpg" alt="WHILE... DO... ENDWHILE loop" width="500"> 
</div>  




