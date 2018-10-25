## Exercise_2.3.4 :

#### Selection can also be performed on bags. Give a map-reduce implementation that produces the proper number of copies of each tuple t that passes the selection condition. That is, produce key-value pairs from which the correct result of the selection can be obtained easily from the values.
### solution :

##### MAP:    for any satisfactory tuple a,return a key-value as (a , V);
##### REDUCE: for each the same key,create key-value (a , [V,V,..,V]) and return (a , sum[V,...,V]).
