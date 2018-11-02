## Exercise_5.1.3:

## Exercise 5.1.3 : Suppose the Web consists of a clique (set of nodes with all possible arcs from one to another) of n nodes and a single additional node that is the successor of each of the n nodes in the clique. Figure 5.8 shows this graph for the case n = 4. Determine the PageRank of each page, as a function of n and β.

## Sulotion:

### -We know that each node links to n-1 other nodes;
### -By deleting dead nodes, each node links to n-2 other nodes;
### -So we have n node and V vector is:
### V_(0) = [ 1/n
              1/n
               .
               .
               .  
              1/n ];
          
### Note: V vector is n*1;
### -M = 
         |   0      1/n-2     ...     1/n-2 |
         | 1/n-2      0       ...     1/n-2 |
         |   .             .            .   |
         |   .                  .       .   |
         |   .                      .   .   |
         | 1/n-2     ...      1/n-2     0   |
          
### -Note:M is a matrix n*n and All elements main diameter of M matrix is zero;

### V′(i)=βMV(i)+((1−β)e/n);

### V′_(i)=
            | (n-1)/(n(n-2)) |
            |       .        |
            |       .        |
            |       .        |
            | (n-1)/(n(n-2)) |;
