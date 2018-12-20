# Assignment 7: Basics of Scheduling

## Question 1


>**1. Scheduling -- Process:**   
>Selection When discussing "When to Schedule" in class, it was mentioned that sometimes scheduling could be improved if an important process could play a role in selecting the next process to run when it blocks. Give a situation where this could be used and explain how.

In a situation, where it is neccesary that something/someone has to be verifyed. 

_____
## Question 2

>**2.Minimizing Turn Around Time:**  
 Imagine the following list of processes in ready state:

|          Process         | A | B | C  | D  | E  | F  | G | H  |
|:------------------------:|:-:|:-:|:--:|:--:|:--:|:--:|:-:|:--:|
|       Run Time (msec)    | 8 | 5 | 16 | 12 | 55 | 21 | 2 | 34 |

>How should a scheduler order these processes to minimize average turn around time? What is the minimal average turn around time in the optimal order you found?

### sort:

|          Process         | G | B | A | D  | C  | F  | H  | E  |
|:------------------------:|:-:|:-:|:-:|:--:|:--:|:--:|:--:|:--:|
|       Run Time (msec)    | 2 | 5 | 8 | 12 | 16 | 21 | 34 | 55 |

#### sum:
        2 + (2+5) + (7+8) + (15+12) + (27+16) + (43+21) + (64+34) + (98+55) = **409 msec**

#### average: 
        avg= 409 / 8 =  51.125 msec

_____
## Question 3

>**3. Round-Robin Scheduler:**  
Discussion Round-robin schedulers normally maintain a list of all runnable processes, with each process occurring exactly once in the list. What would happen if a process occurred twice in the list?

All processes in the ready queue are given equal time units. CPU time is divided equally among the processes. 
So if a process was listed twice, it would get twice the CPU time of the other processes.