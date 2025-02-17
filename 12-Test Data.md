# 7.6 Test Data  
## 7.6.1 How to suggest and apply suitable test data  
In order to determine whether a solution is working as it should, it needs to be tested. Usually before a whole system is tested each sub-system is tested separately.  
Algorithms written in pseudocode or as flowcharts can be tested by a person working through them using any data that is required and seeing what the result is. Computer programs can be tested by running them on a computer using any data that is required and seeing what result is output. However, in order to test a solution thoroughly it may need to be worked through several times with different sets of test data.  
  
A **set of test data** is all the items of data required to work through a solution. For instance, the set of test data used for Activity 7.6 was 7 and 8.  
In order to prove that program or algorithm solutions do what they are supposed to do, a set of test data should be used that the program would normally be expected to work with, together with the result(s) that are expected from that data. The type of test data used to do this is called **normal data**. Normal data shold be used to work through the solution to find the actual results(s) and see if they are the same as the expected result(s).   
For example, consider an algorithm that records the percentage marks, entered in whole numbers, from ten end-of-term examinations for a pupil, and then finds the average mark. A set of normal test data for this purpose could be:  
Normal test data: 50, 50, 50,50, 50, 50,50, 50, 50, 50, 50, 50.  
Expected result: 50  

Solutions also need to be tested to prove that they do **not** do what they are  supposed not to do. In order to do this, test data should be chosen that would be rejected by the solution as not suitable, if the solution is working properly. This type of test data is called **abnormal test data**. (It is also sometimes called **erroneous test data.**)

For example, erroneous/abnormal data for our algorithm to find the average percentage marks from ten end of term examinations could be:  
- erroneous/abnormal data: -12, eleven  
- Expected results: both of these values should be rejected.

When testing algorithms with numerical values, sometimes only a given range of values should be allowed. For example, percentage marks should only be in the range 0 to 100. Our algorithm above should be tested with **extreme data**. Extreme data are the largest and smallest values that normal data can take. In this case:   
Extreme data: 0, 100  
Expected results: these values should be accepted  
There is another type of test data called **boundary data**. This is used to establish where the largest and smallest values occur. At each boundary two values are required: one value is accepted and the other value is rejected. For example, for percentage marks in the range of 0 to 100, the algorithm should be tested with the following **boundary data**:  
Boundary data for 0 is: -1, 0  
Expected results: -1 is rejected, 0 is accepted
