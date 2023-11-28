### A. Find the top 5 nodes with the highest outdegree and find the count of the number of outgoing edges in each
```
outDeg = epinionsGraph.outDegrees
outDeg.orderBy(desc("outDegree")).show(5, truncate=False)
```
#### Answer: 
```
+-----+---------+
|id   |outDegree|
+-----+---------+
|645  |1801     |
|763  |1669     |
|634  |1621     |
|71399|1128     |
|3924 |976      |
+-----+---------+
only showing top 5 rows
```

---

### B. Find the top 5 nodes with the highest indegree and find the count of the number of incoming edges in each
```
inDeg = epinionsGraph.inDegrees
inDeg.orderBy(desc("inDegree")).show(5, truncate = False)
```
#### Answer: 
```
+---+--------+
|id |inDegree|
+---+--------+
|18 |3035    |
|143|1521    |
|737|1317    |
|790|1284    |
|136|1180    |
+---+--------+
only showing top 5 rows
```

---

### C. Calculate PageRank for each of the nodes and output the top 5 nodes with the highest PageRank values. You are free to define any suitable parameters.
```
ranks = epinionsGraph.pageRank(resetProbability=0.15, maxIter=10)
ranks.vertices.orderBy(desc("pagerank")).select("id", "pagerank").show(5)
```
#### Answer: 
```
+----+------------------+
|  id|          pagerank|
+----+------------------+
|  18|345.13733694778057|
| 737|240.25396712965642|
| 118|162.02085699786338|
|1719| 158.8534560750275|
| 136|151.67122319877475|
+----+------------------+
only showing top 5 rows
```

### D. Run the connected components algorithm on it and find the top 5 components with the largest number of nodes.
```
scc = epinionsGraph.stronglyConnectedComponents(maxIter=3)
scc.show(5)
```
#### Answer: 
```
+---------+-----+
|component|count|
+---------+-----+
|        0|32223|
|    47210|   15|
|    33367|    9|
|      515|    9|
|    35011|    8|
+---------+-----+
only showing top 5 rows

```
### E. Run the triangle counts algorithm on each of the vertices and output the top 5 vertices with the largest triangle count. In case of ties, you can randomly select the top 5 vertices.

```
tc = epinionsGraph.triangleCount()
tc.orderBy(desc("count")).show(5, truncate=False)
```

#### Answer
```
+-----+---+
|count|id |
+-----+---+
|48674|645|
|47203|18 |
|25817|27 |
|25230|634|
|24752|44 |
+-----+---+
only showing top 5 rows

```
