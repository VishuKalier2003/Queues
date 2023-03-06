

# ${ Maximum \space Meeting \space Room \space Problem}$

## ${Problem \space Statement}$

      You are given an integer n. There are n rooms numbered from 0 to n - 1. You are given a 2D integer array meetings where 
      meetings[i] = [starti, endi] means that a meeting will be held during the half-closed time interval [starti, endi]. All
      the values of starti are unique. Meetings are allocated to rooms in the following manner:
      * Each meeting will take place in the unused room with the lowest number.
      * If there are no available rooms, the meeting will be delayed until a room becomes free. The delayed meeting should 
      have the same duration as the original meeting.
      * When a room becomes unused, meetings that have an earlier original start time should be given the room.
      Return the number of the room that held the most meetings. If there are multiple rooms, return the room with the lowest 
      number. A half-closed interval [a, b] is the interval between a and b including a and not including b. 

-------

## ${Test \space Cases}$

### Case 1

      Input                                                                    Output
      rooms = 2                                                                maximum meeting room = 0
      meetings = [[1, 5], [2, 7], [0, 10], [3, 4]]

Since there are two rooms indexed 0 and 1. We will create a table and check the number of meetings in each specific room.
| Room Number | Meetings | Total Meetings |
|-|-|-|
| 0 | {0, 10} , {3, 4} | 2 |
| 1 | {1, 5} , {2, 7} | 2 |


Thus, the lowest index room with maximum meetings is 0.

### Case 2

      Input                                                                    Output
      rooms = 3                                                                maximum meeting room = 1
      meetings = [[1, 20], [3, 5], [6, 8], [2, 10], [4, 9]


Since there are three rooms indexed 0, 1 and 2. We will create a table and check the number of meetings in each specific room.
| Room Number | Meetings | Total Meetings |
|-|-|-|
| 0 | {1, 20} | 1 |
| 1 | {3, 5} , {4, 9} | 2 |
| 2 | {2, 10} , {6, 8} | 2 |


Thus, the lowest index room with maximum meetings is 1.

### Case 3

      Input                                                                    Output
      rooms = 4                                                                maximum meeting room = 2
      meetings = [[18, 19], [3, 12], [17, 19], [2, 13], [7, 10]

Since there are four rooms indexed 0, 1, 2 and 3. We will create a table and check the number of meetings in each specific room.
| Room Number | Meetings | Total Meetings |
|-|-|-|
| 0 | {2, 13} | 1 |
| 1 | {3, 12} | 1 |
| 2 | {7, 10} , {17, 19} | 2 |
| 3 | {18, 19} | 1 |


Thus, the lowest index room with maximum meetings is 2.


------

## ${ Code, \space Implementation \space and Complexity }$

***Link*** [here](https://github.com/VishuKalier2003/Maximum-Meeting-Room/blob/main/Meetings.java)

## ${Ciphered \space By}$
***Vishu Kalier***











