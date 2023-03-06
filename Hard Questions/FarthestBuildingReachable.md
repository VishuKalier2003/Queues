

# ${ Farthest \space Building \space Reachable \space Problem}$

## ${Problem \space Statement}$

      You are given an integer array heights representing the heights of buildings, some bricks, and some ladders.
      You start your journey from building 0 and move to the next building by possibly using bricks or ladders. 
      While moving from building i to building i+1 (0-indexed),
      * If the current building's height is greater than or equal to the next building's height, you do not need
      a ladder or bricks.
      * If the current building's height is less than the next building's height, you can either use one ladder or
      (h[i+1] - h[i]) bricks.
      Return the furthest building index (0-indexed) you can reach if you use the given ladders and bricks optimally.

-------

## ${Test \space Cases}$

### Case 1

      Input                                                                    Output
      bricks = 10                                                              Farthest Building Index = 7
      ladders = 2
      height = [4, 12, 2, 7, 3, 18, 20, 3, 19]

We will create a table and check the allocation of resources for each jump.
| Height From | Height To | Resources Allocated | Resources Left |
|-|-|-|-|
| 4 | 12 | 1 ladder | 1 ladder, 10 bricks |
| 12 | 2 | None | 1 ladder, 10 bricks |
| 2 | 7 | 5 bricks | 1 ladder, 5 bricks |
| 7 | 3 | None | 1 ladder, 5 bricks |
| 3 | 18 | 1 ladder | 0 ladder, 5 bricks |
| 18 | 20 | 2 bricks | 0 ladder, 3 bricks |
| 20 | 3 | None | 0 ladder, 3 bricks |

Since we have lesser resources to jump to the next building ***from 3 to 19***. So the farthest building we have reached is ***3*** with the index ***7*** as the 
output. Also, using resources any other way we cannot reach beyond this building index. Thus the output is 7


### Case 2

      Input                                                                    Output
      bricks = 17                                                              Farthest Building Index = 3
      ladders = 0
      height = [14, 3, 19, 13]

We will create a table and check the allocation of resources for each jump.
| Height From | Height To | Resources Allocated | Resources Left |
|-|-|-|-|
| 14 | 3 | None | 0 ladder, 17 bricks |
| 3 | 19 | 16 bricks | 0 ladder, 1 brick |
| 19 | 13 | None | 0 ladder, 1 brick |

So the farthest building we have reached is ***13*** with the index ***3*** as the output. Also, using resources any other way we cannot reach beyond this building
index. Thus the output is 3

### Case 3

      Input                                                                    Output
      bricks = 5                                                               Farthest Building Index = 4
      ladders = 1
      height = [4, 2, 7, 6, 9, 14, 12]

We will create a table and check the allocation of resources for each jump.
| Height From | Height To | Resources Allocated | Resources Left |
|-|-|-|-|
| 4 | 2 | None | 1 ladder, 5 bricks |
| 2 | 7 | 1 ladder | 0 ladder, 5 bricks |
| 7 | 6 | None | 0 ladder, 5 bricks |
| 6 | 9 | 3 bricks | 0 ladder, 2 bricks |

Since we do not have enough resources for the next jump. So the farthest building we have reached is ***9*** with the index ***4*** as the output. 
Also, using resources any other way we cannot reach beyond this building index. Thus the output is 4


------

## ${ Code, \space Implementation \space and Complexity }$

***Link*** [here](https://github.com/VishuKalier2003/Farthest-Building-Reachable/blob/main/Buildings.java)

## ${Ciphered \space By}$
***Vishu Kalier***




