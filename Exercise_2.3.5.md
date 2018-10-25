## Exercise_2.3.5 :

#### The relational-algebra operation R(A,B) ⊲⊳ B<C S(C,D) produces all tuples (a, b, c, d) such that tuple (a, b) is in relation R, tuple (c, d) is in S, and b < c. Give a MapReduce implementation of this operation, assuming R and S are sets.

### solution :

##### MAP:    take Key-Value ((c,d),V) and (a,b) then return ((b,c,d),V);
##### REDUCE: for each ((b,c,d),k) ,if b<c return (a,b,c,d).
