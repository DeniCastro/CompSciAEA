# 7.5 Validation and verification  
In order for computer system to only accept data inputs that are reasonable and accurate, every item of data needs to be examined before it is accepted by the system.  
Two different methods, with very similar sounding names, are used. For data entry, validation ensures that only data that is reasonabl is accepted.  
Verification is used to check that the data does not change as it is being entered.  

## 7.5.1 Validation  
**Validation** is the automated checking by a program data is reasonable before it is accepted into a computer system. When data is validated by a computer system, if the data is rejected a message should be output explaining why the data was rejected and another opportunity given to enter the data.  

There are many different types of validation checks including:  


- **range checks**  
- **length checks**
- **type checks**
- **presence checks**
- **format checks**
- **check digits**  


Different types of check may be used on the same piece of data; for example, an examination mark could be checked for reasonableness by using a range check, a type check and a presence check.  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Range%20Check.jpg" alt="Range Check" width="500"> 
</div>        
   
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Length%20Check.jpg" alt="Length Check" width="500"> 
</div>       

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Length%20Check%202.jpg" alt="Length Check 2" width="500"> 
</div>  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Type%20Check%20and%20Presence%20Check.jpg" alt="Type Check and Presence Check" width="500"> 
</div>          

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Figure%207.12%20Presence%20check%20error%20message.jpg" alt="Figure " width="500">   
</div>        

### **Format check and check digit**
  
A **format check** checks that the charactes entered conformt to a pre-defined pattern, for example, in Chapter 9 the cub number must be in theform CUB9999. The pseudocode for this example will be given in the string handling section of Chapter 9.  
A **check digit** is the final digit included in a code; it is calculated from all the other digits in the code. Check digits are used for barcodes, product codes, International Standard Book Numbers (ISBN) and Vehicle Identification Numbers (VIN).  
Check digits are used to identify errors in data entry caused by mis-typig or mis-scanning a barcode. They can usually detect the following types of error:  
- an incorrect digit entered, for example, 5327 entered instead of 5307  
- transposition errors where two numbers have changed order for example 5037 instead of 5307  
omitted or extra digits, for example, 537 instead of 5307 or 53107 instead of 5307  
- phonetic errors, for example, 13, thirteen, instead of 30, thirty.  



</div>        
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Figure%207.13%20ISBN%2013%20Code%20with%20check%20digit.jpg" alt="Figure 7.13" width="200"> 
</div>      


</div>        
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Actiity%207.7.jpg" alt="Activity 7.7" width="800"> 
</div>      
  
[Access the complete explanation here.](https://www.youtube.com/watch?v=jCpCOxbitPM&ab_channel=PerhloAcademy2)  


## 7.5.2 Verification   
**Verification** is checking that data has ben accurately copied from one source to another - for instance, input into a computer or transfered one part of a computer system to another.  
Verification methods for input data include.  
- Double entry.  
- Screen/visual check.  
For **double entry** the data is entered twice, somethimes by different operators. The computer system compares both entries and if they are different outputs an error message requesting that the data is entered again.    

</div>        
<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Figure%207.14%20-%20Double%20Entry.jpg" alt="Figure 7.14" width="500"> 
</div>       

A **screen/visual check** is a manual check completed by the user who is entering the data. When the data entry is complete the data is displayed on the screen and the user is asked to confirm that it is correct before continuing. The user either checks the data on the screen against a paper document that is being used as an input form or, confirms whether it is correct from their own knowledge.   

