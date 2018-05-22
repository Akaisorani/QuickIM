# QuickIM

QuickIM is a fast algorithm to find top k most influential vertices on a large scale Network.

## Files

`QuickIM` is built under linux gcc 4.8.4

`QuickIM.exe` is built under win10 gcc 5.3.0

## How to use

### Graph data format

QuickIM accepts **directed** graph with probability on the edge.

The first line of the graph data should be `N M` where **N** is the total node number and **M** is the total edge number.

Then the followed M lines are the M directed edges. Each line is `u v p` that means there is an edge from node **u** to node **v** and the probability that **u** influence **v** is **p**. (0<=**u, v**<N)

---
### Execution

The Execution format is
```bash
./QuickIM <data_filename> <k>
```

**For example**
```bash
./QuickIM ./data/DBLP_wc.txt 10
```
---
### Output result

QuickIM use standard output stream to output result. The result include QuickIM algorithm elapsed time, top k nodes.
