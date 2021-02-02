## MDCCVRP

The *Multi Depot Cumulative Capacitated Vehicle Routing Problem* (*MDCCVRP*) is a variation of the *Cumulative Capacitated Vehicle Routing Problem* (*CCVRP*), with the addition of multiple depots that serve as starting points of the routes. Its objective is to minimize the sum of arrival times at customers. This problem also implies that every customer is visited and served only once, and that every vehicle available has a capacity that can't be surpassed.

The *MDCCVRP* can be applied in multiple contexts, but one that can be very helpful with is in disaster responses. For example, planning the ambulance routing, where they depart from different hospitals and have to aid groups of patients in an emergency situation, as Talarico et al. proposed in his paper [[1](#Talarico)].

### Instances

In this repository we present different instances that have been tested in multiple papers. The first of them were proposed by
Cordeau et al. [[2](#Cordeau)] for the *Multi Depot Vehicle Routing Problem* (*MD-VRP*), but can be applied to the *MDCCVRP*. The second set of instances was proposed by Lalla et al. [[3](#Lalla)], which are small and medium size instances based on the ones given by Cordeau et al. [[2](#Cordeau)].

These instances were not only used by Lalla et al. [[3](#Lalla)] in their *POPMUSIC* approach to the *MDCCVRP*, but also Wang et al. [[4](#Wang)] in their paper used them to compare the results obtained.

### File Format 

This is the file format:

```
50 # n number of customers
4  # t number of depots
80 # Q vehicle capacity

37.000000 52.000000 # Description of V: Dots in the plane. There are  n+t 
49.000000 49.000000
52.000000 64.000000
...
50.000000 30.000000
60.000000 50.000000
   # blank line
7.000000 # Demands for each customer. There are n+t entries
30.000000 
16.000000
9.000000
...
18.000000
10.000000
0.000000   # The last 4 are zeros corresponding to the depots
0.000000
0.000000
0.000000
```

### References

<a name="Talarico"></a> 1. Talarico, L., Meisel, F., Sörensen, K.: Ambulance routing for disaster response with patient groups.
Comput. Oper. Res. 56, 120–133 (2015)

<a name="Cordeau"></a> 2. Cordeau, J.F., Gendreau, M., Laporte, G.: A tabu search heuristic for periodic and multi-depot vehicle
routing problems. Networks 30(2), 105–119 (1997)

<a name="Lalla"></a> 3. E. Lalla-Ruiz and S. Voß, “A popmusic approach for the multi-depot cumulative ca-pacitated vehicle routing problem,”Optimization Letters, vol. 14, pp. 671–691, 42020.

<a name="Wang"></a> 4. X. Wang, T. M. Choi, Z. Li, and S. Shao, “An effective local search algorithm for themultidepot cumulative capacitated vehicle routing problem,”IEEE Transactions onSystems, Man, and Cybernetics: Systems, vol. 50, no. 12, pp. 4948–4958, 2020.
