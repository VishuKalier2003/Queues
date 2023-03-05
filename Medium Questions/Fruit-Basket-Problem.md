
# ${Fruit \space Basket \space Problem}$

## ${Problem \space Statement}$
    
    You are visiting a farm that has a single row of fruit trees arranged from left to right. The trees are 
    represented by an integer array fruits where fruits[i] is the type of fruit the ith tree produces. You 
    want to collect as much fruit as possible. However, the owner has some strict rules that you must follow:
    Rule 1:- You only have two baskets, and each basket can only hold a single type of fruit. There is no 
    limit on the amount of fruit each basket can hold.
    Rule 2:- Starting from any tree of your choice, you must pick exactly one fruit from every tree (including
    the start tree) while moving to the right. The picked fruits must fit in one of your baskets.
    Rule 3:- Once you reach a tree with fruit that cannot fit in your baskets, you must stop.
    Given the integer array fruits, return the maximum number of fruits you can pick take the value stored as
    the sum of fruits in both basket. 


## ${Test \space Cases}$

### Case 1
  
    Input                                                             Output
    fruits = [1, 2, 1]                                                basket = 3

Since there are only two types of fruits we take all the fruits. The total number of fruits in the basket is ***2 fruits of type 1*** and ***1 fruit of type 2***. So, 
Total fruits in the basket are 2 + 1 = 3.

### Case 2
  
    Input                                                             Output
    fruits = [0, 1, 2, 2]                                             basket = 3

We have three varieties of fruits *** 1 fruit of type 0***, ***1 fruit of type 1*** and ***2 fruit of type 2***. So, we will start from tree index 1, to maximise the
number of fruits in the basket. Also, they occur in sequence. Thus, the number of fruits collected are 1 + 2 = 3.

### Case 3
  
    Input                                                             Output
    fruits = [1, 2, 3, 2, 2]                                          basket = 4

We have three varieties of fruits ***1 fruit of type 1***, ***3 fruits of type 2*** and ***1 fruit of type 3***. So, to maximise the number of fruits we start from 
index 1. Also, they occur in sequence. Thus, the number of fruits collected are 3 + 1 = 4.


## ${Code, \space Implementation \space and \space Complexity }$

${Link}$ [here](https://github.com/VishuKalier2003/Trapping-Water-Problem/blob/main/TrappingWater.java)

### ${Ciphered \space By}$
<b><i> Vishu Kalier
  
  
  
  


