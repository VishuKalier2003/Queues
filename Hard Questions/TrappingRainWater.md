

# ${Trapping \space Rain \space Water \space Problem}$

## ${Problem \space Statement}$

    Given n non-negative integers representing an elevation map where the width of each bar is 1, 
    compute how much water it can trap after raining.

------

## ${Test \space Cases}$

### Case 1

    Input                                             Output
    height = [0, 1, 0, 2, 1, 0, 1, 3, 2, 1, 2, 1]     Trapped Water = 6

We can draw a diagram with height 0 as the ground level and then we can deduce the water trapped. As an example, between index 1 and index 3, ***1 unit of water*** 
will be trapped. Between index 3 and index 7, ***4 units of water***. Between index 8 and index 10, ***1 unit of water***. So, the total unit water trapped 
is ***1 + 4 + 1 = 6 units of water trapped***.

    
### Case 2

    Input                                             Output
    height = [4, 2, 0, 3, 2, 5]                       Trapped Water = 6

We can draw a diagram with height 0 as the ground level and then we can deduce the water trapped. As an example, between index 0 and index 5, ***9 units of water*** 
will be trapped. So, the total unit water trapped is ***9 units of water trapped***.


------

## ${Code, \space Implementation \space and \space Complexity}$
<b><i>Link [here](https://github.com/VishuKalier2003/DSA-Trapping-Water-Problem/blob/main/TrappingWater.java)
  
## ${Ciphered \space By}$
  <b><i>Vishu Kalier
    
    
    
