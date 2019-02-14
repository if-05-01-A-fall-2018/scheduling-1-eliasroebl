 ## **if.05.01 TINF**

 # **Assignment 8: Scheduling 2**

 ##  <u>_1. Multiple Queues:_</u>

 ### Aufgabe:
    Multiple Queues A process on a system with Multiple Queues Scheduling needs 30 quanta to complete. How many times must it be swapped in, including the very first time (before it has run at all)?

### Lösung: 
| | | | | | |
|-|-|-|-|-|-|
|__Run__| 1 | 2 | 3 | 4 | 5 |
| __Q__ | 1 | 2 | 4 | 8 | 15 |
|__Acc__| _1_ | _3_ | _7_ | _15_ | _30_|

    Wie wir sehen ist bei Run 5 die Acc über 30. Somit muss es mal geswapped werden.

<br/>

## <u>_2.Shortest Process Next_</u>

### Aufgabe:
    A scheduler working with the {\em Shortest Process Next} Strategy has two processes in ready state and has to schedule one of these:

   | Process Name | 1st run | 2nd run | 3rd run | 4th run |
| -- | -- | -- | -- | -- |
A | 50 msec | 150 msec | 300 msec | 85 msec |
B | 300 msec | 150 msec | 85 msec | 50 msec

### Lösung:

#### Formel:
>$$T_0/8 + T_1/8 + T_2/4 + T_3/2$$

#### Anwendung auf unser Bsp

> __A:__ &nbsp;$\frac{50}{8}$ + $\frac{150}{8}$ + $\frac{300}{4}$ + $\frac{85}{2}$ = _142.5_  
>
>__B:__ &nbsp;$\frac{300}{8}$ + $\frac{150}{8}$ + $\frac{85}{4}$ + $\frac{50}{2}$ = _102.5_

#### Lösung:
>Wie wir [hier](#anwendung-auf-unser-bsp) gezeigt haben ist Process __B__ der Kürzere.

<br/>

## <u>_3.CPU-bound and I/O-bound Processes_</u>

#### CPU Bound & I/O Bound
- __CPU Bound__ means the rate at which process progresses is limited by the speed of the CPU.
    
    - A task that performs calculations on a small set of numbers, for example multiplying small matrices, is likely to be CPU bound.

    - A program is CPU bound if it would go faster if the CPU were faster.

- __I/O Bound__ means the rate at which a process progresses is limited by the speed of the I/O subsystem.

    - A task that processes data from disk, for example, counting the number of lines in a file is likely to be I/O bound.

    - A program is I/O bound if it would go faster if the I/O subsystem was faster.


## <u>_4.Real Time Schedulable_</u>

#### Lösung:

>0,95 + $\frac{x}{250}$ <= 1 /&nbsp;-0,95  
>$\frac{x}{250}$ <= 0,05/ *250  
>x <= __12,5__

    The largest value for $x$ for which the system is schedulable is 12,5


<br>

##
> Elias Röbl, TINF HÜ, 13.02.2019, 3AHIF, 18/19


    



