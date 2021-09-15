# Gradual-Milk-Blending-Instances
Instances of Gradual Milk Blending (GMB) problem

The file format is a CPLEX-like input format.

First item (set Nodes: =) lists the whole set of nodes: The first one (Id = 1000) is the depot.
Second item (set I: =) lists the set of farms. It excludes the depot.
Third item (set K: =) lists the available trucks.
Fourth item (param Q: =) lists the capacity of trucks
Fifth item (param D: =) lists the total milk produced to collect (A, B, and C)
Sixth item (param V: =) lists the revenue per liter of milk collected depending on its final grade (A, B, and C)
Seventh item (param U: =) lists the number of somatic cells that determine the grades of combined milk (A, B, and C)
Eighth item (param qu: =) lists the id, the total production, the type of milk, and the number of somatic cells of each node (1 = milk A, 2 = milk B, and 3 = milk C). For the depot, it only shows the identifier and total production.
Ninth item (param cap: =) lists the capacity of each collection center. In some locations, there is possible to allocate collection centers of any type. In these cases, one line per milk type can be found in this list.
Last item (param c [,]) shows the distance matrix between nodes. The first line shows the ids of nodes. In all the following lines, the first column shows the id of the corresponding node. Id = 1000 is reserved for the depot.
