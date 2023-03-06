
# ${ Keys \space And \space Rooms \space Problem}$

## ${Problem \space Statement}$

      here are n rooms labeled from 0 to n - 1 and all the rooms are locked except for room 0. Your goal
      is to visit all the rooms. However, you cannot enter a locked room without having its key. When you
      visit a room, you may find a set of distinct keys in it. Each key has a number on it, denoting which
      room it unlocks, and you can take all of them with you to unlock the other rooms. Given an array rooms
      where rooms[i] is the set of keys that you can obtain if you visited room i, return true if you can
      visit all the rooms, or false otherwise.

-------

## ${Test \space Cases}$

### Case 1

      Input                                                                    Output
      rooms = [[1], [2], [3], [4]]                                             Unlocked = True

Since there are 4 rooms. We will create a table and check the key and its corresponding room.
| Room Number | Key | Room Opened |
|-|-|-|
| 0 | 1 | 0, 1 |
| 1 | 2 | 0, 1, 2 |
| 2 | 3 | 0, 1, 2, 3 |
| 3 | 4 | 0, 1, 2, 3 |


Since, we have unlocked all the rooms the output is ***True***.


### Case 2

      Input                                                                    Output
      rooms = [[1, 3], [3, 0, 1], [2], [0]]                                    Unlocked = False

Since there are 4 rooms. We will create a table and check the key and its corresponding room.
| Room Number | Key | Room Opened |
|-|-|-|
| 0 | 1, 3 | 0, 1, 3 |
| 1 | 0, 1, 3 | 0, 1, 3 |
| 2 | 2 | 0, 1, 3 |
| 3 | 0 | 0, 1, 3 |

Since the room indexed 2 in not unlocked. The output then results to ***False***.

### Case 3

      Input                                                                    Output
      rooms = [[1, 2, 3], [1], [2]]                                            Unlocked = True

Since there are 3 rooms. We will create a table and check the key and its corresponding room.
| Room Number | Key | Room Opened |
|-|-|-|
| 0 | 1, 2, 3 | 0, 1, 2 |
| 1 | 1 | 0, 1, 2 |
| 2 | 2 | 0, 1, 2 |

Since all rooms are unlocked we will return the output as ***True***.


### Case 4

    Input                                                                    Output
    rooms = [[], [1], [3]]                                                   Unlocked = True

Since there are 4 rooms. We will create a table and check the key and its corresponding room.
| Room Number | Key | Room Opened |
|-|-|-|
| 0 | None | 0 |
| 1 | 1 | 0 |
| 2 | 3 | 0 |

Since all rooms are not unlocked we will return output as ***False***.

------

## ${ Code, \space Implementation \space and Complexity }$

***Link*** [here](https://github.com/VishuKalier2003/Keys-and-Rooms-Problem/blob/main/KeysRooms.java)

## ${Ciphered \space By}$
***Vishu Kalier***
