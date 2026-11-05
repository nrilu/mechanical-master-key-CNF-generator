# Usage

Run ``` ./lockchart_to_cnf.py```

Optional flags:

```-l <1..INTMAX> ``` Number of locks (default: L=50) \
```-r <0..1> ``` Probablity for the randomized lock-charts. Per default the lock-charts are structured (default: r=0) \
```-p <1..INTMAX>``` Number of dent positions per key (default: P=8) \
```-d <1..INTMAX>``` Number of depths per key position (default: D=4) 

The outputs files are automatically stored in ```results/``` with following naming convention

```
results/lockchart-L{L}-K{K}-p{P}d{D}j{J}-t{T}
L = Number of locks
K = Number of keys
P = Number of dent positions per lock
D = Number of depth layers
J = Max jump in depth between neighbouring positions
T = Timetag of generation 
```
# mechanical-master-key-CNF-generator

A generator for Mechanical Master-Key Problems as CNF SAT formulas. Heavily based on Radomír Černochs ["Lock-chart solving"](https://github.com/cernoch/mks-dis/blob/master/LockChartSolvingWeb.pdf) (2017) and Martin Hořeňovskýs [Performance analysis of a
master-key system solver](https://codingnest.com/files/thesis.pdf) (2018).

Submitted to the Benchmark Submissions of the [SAT Competition 2025.](https://satcompetition.github.io/2025/)

