# Interface Double Linked List for C
This is an interface to work with double list in C. It's tested on Linux operating systems, specifically, Arch linux. 
The interface is generic, so the nodes can have any type data.
## Functions of the interface
```C
createDoubleList() /*Create an intance of double list*/
```
```C
insertOrderedDN(nodeD *q, doubleList *ls, int (*fn)(void *a, void *b)) 
  /*Insert node q at the location specified by fn (this function must define it the user)*/
```
```C
newNodeD() /*Reserve memory for the one nodeD (Double node)*/
```
```C
pushDN(nodeD *q, doubleList *ls) /*Insert the node q at the last position*/
```
```C
unshiftDN(nodeD *q, doubleList *ls) /*Insert the node q at the first position*/
```
```C
shiftDN(doubleList *ls) /*Delete the first node the list*/
```
```C
popDN(doubleList *ls) /*Delete the last node of list*/
```
```C
*getNextNodeD(nodeD *p) /*Get next node of the p and return it*/
```
```C
*getPreviousNodeD(nodeD *p) /*Get previous node of the p and return it*/
```
```C
deleteALL(doubleList *ls) /*Delete all nodes of the list and free memory*/
```
```C
travelListNatural(doubleList *dl, void (*fn)(void *e))
  /*Travel natural: travel from the first node. You must define the funcion fn to display the datas*/
```
```C
travelListUnnatural(doubleList *dl, void (*fn)(void *e))
  /*Travel unnatural: travel from the last node. You must define the funcion fn to display the datas*/
```
