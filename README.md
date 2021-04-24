# RopeLike-Text-Buffer
**This will record the process of completing the final project RopeLike Text Buffer**  
Team member: Jirong Yi, Chongzheng Guo
Data structure and algorithm - 593 - 2021 S - final project

Introduction:  
In computer programming, a rope is a data structure composed of smaller strings, which is used to efficiently store and process very long strings. For example, when used to hold text, ropes are used to insert large strings faster than a string.Our goal is to create an object that can manipulate large (100MB+) strings rapidly and compare speed to traditional strings.  

Abstract:  
A rope is a type of binary tree i.e. each node can have maximum of 2 children at the maximum, where every leaf node holds a String or a Substring and the length of the same(Also known as the "weight" for the corresponding leaf node) and every following parent node holds the total sum of the weights of the leaf nodes in its left subtree, which in turn is described as the weight of the said node. In a more simpler form, the weight of a node is the sum of all the leaf nodes that sprout from its immediate left child node. Create a tree with degree k. You will try k=2, k=4, k=16. For example, with degree 4, each node has 4 children. At the lowest level, the nodes contain 4 strings, each of which is a string for a line. Implement all the same methods described above and compare the Ropelike data structure speed to the original string implementation. In order to insert a string at a given position, we will split it at the index from which to insert, and then first concatenate the first half of the string we split and the new string followed by concatenating the result and the other split off part of the original string.   
Reference:  
1."Ropes: an Alternative to Strings"Boehm, Hans-J; Atkinson, Russ; Plass, Michael;Xerox PARC, 3333 Coyote Hill Rd., Palo Alto, CA 94304, U.S.A(https://citeseer.ist.psu.edu/viewdoc/download?doi=10.1.1.14.9450&rep=rep1&type=pdf)  
2.SGI extensions(https://web.archive.org/web/20121225183151/http://www.sgi.com/tech/stl/Rope.html)  
3.Rope: the Data Structure used by text editors to handle large strings(https://iq.opengenus.org/rope-data-structure/)  
4.Ropes Data Structure (Fast String Concatenation)(https://www.geeksforgeeks.org/ropes-data-structure-fast-string-concatenation/)  
5.Ropes Data Structure (https://medium.com/underrated-data-structures-and-algorithms/rope-data-structure-e623d7862137)  
