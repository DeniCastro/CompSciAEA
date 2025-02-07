# 7.4.4 Linear Search  

A search is used to check if a value is stored in a list, performed systematically working through the items in the list. There are several standaard search methods, but you only need to understand one method for IGCSE Computer Science. This is called a **linear search**, which inspects each item in a list in turn to see if the item matches the value searched for.  
For example, searching for a name in a class list of student names, where all the names stored are different:

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Linear%20Search%201.jpg" alt="Linear Search 1" width="800"> 
</div>    


<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Linear%20Search%202.jpg" alt="Linear Search 2" width="800"> 
</div>      



<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Linear%20Search%203.jpg" alt="Linear Search 3" width="800"> 
</div>  
  
## 7.4.5 Bubble sort  
Lists can be more useful if the items are sorted in a meaningful order. For example, name could be sorted in alphabetical order, or temperatures could be sorted in ascending or descending order. There are several standard sorting methods available, but you only need to understand one method for IGCSE Computer Science.  
This method of sorting is called **bubble sort**. Each element is compared with next element and swapped if the elements are in the wrong order, starting from the first element and finishing with the next-to-last element. Once it reaches the end of the list, we can be sure that the last element is now in the correct place. However, other items in the list may still be out of order. Each element in the list is compared again apart from the last one because we know the final element is in the correct place. This continues to repeat until there is only one element to check or no swaps are made.
  
  
For example, the bubble sort algorithm can be used to sort a list of ten temperatures stored in the array, **Temperature[]**, into ascending order. It could be written in pseudocode as:  

<div align="center"> 
  <img src="https://github.com/DeniCastro/CompSciAEA/blob/ProgramDevelopmentCycle/Bubble%20sort.jpg" alt="Bubble sort" width="800"> 
</div>  

