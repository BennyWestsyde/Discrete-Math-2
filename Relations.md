***
## Relations
***

#### Summary:

Relations describe the connections between elements of sets. Equivalence relations and partial orders are two important types of relations.

#### Definitions:

- **Relation**
: A set of ordered pairs (a, b) where a and b are elements of two sets.
- **Equivalence Relation**
: A relation that satisfies reflexivity, symmetry, and transitivity.
- **Partial Order**
: A relation that satisfies reflexivity, antisymmetry, and transitivity.

#### Example:

An example of an equivalence relation: Let R be a relation on the set of integers where $(a, b) ∈ R$ if a and b have the same remainder when divided by 3.

#### Tricky Things to Remember:

- Equivalence relations and partial orders have different properties.
- Not all relations are equivalence relations or partial orders.

---
### Equivalence Relations

#### Summary:

An equivalence relation is a relation that is reflexive, symmetric, and transitive. It is used to partition a set into equivalence classes.

#### Definitions:

- **Reflexive**
: For all x, (x, x) is in the relation.
- **Symmetric**
: For all x and y, if (x, y) is in the relation, then (y, x) is in the relation.
- **Transitive**
: For all x, y, and z, if (x, y) and (y, z) are in the relation, then (x, z) is in the relation.

#### Example:

Let R be a relation on the set of integers where (a, b) ∈ R if a and b have the same remainder when divided by 3.

This is an equivalence relation. The equivalence classes are:

- [0] = {..., -6, -3, 0, 3, 6, ...}
- [1] = {..., -5, -2, 1, 4, 7, ...}
- [2] = {..., -4, -1, 2, 5, 8, ...}

#### Tricky Things to Remember:

- An equivalence relation partitions a set into disjoint equivalence classes.
- Equivalence classes are unique and non-overlapping.

---
### Equivalence Classes

#### Summary:
Equivalence classes are a fundamental concept in mathematics used to partition sets into subsets with related elements. In other words, the equivalence classes group together elements that are related in some way, forming a new set.

#### Definitions:
- **Partition**
: A partition of a set is a collection of non-empty subsets of the set that are mutually exclusive and whose union is equal to the original set.
- **Equivalence class**
: Given an equivalence relation on a set, the equivalence class of an element `a` is the set of all elements that are related to `a`.

#### Example:
Consider the set of integers `Z` and the equivalence relation "having the same remainder when divided by 3." The equivalence classes of this relation are:
- `[0]`: The set of integers that are divisible by 3.
- `[1]`: The set of integers that leave a remainder of 1 when divided by 3.
- `[2]`: The set of integers that leave a remainder of 2 when divided by 3.
```asc
  [0]: {..., -6, -3, 0, 3, 6, ...}
  [1]: {..., -5, -2, 1, 4, 7, ...}
  [2]: {..., -4, -1, 2, 5, 8, ...}
```
In this example, the set of integers `Z` is partitioned into three subsets (the equivalence classes) based on their remainder when divided by 3.

#### Tricky Things to Remember:
- It's important to note that different equivalence relations can result in different partitionings of a set into equivalence classes.
- Equivalence classes can be represented by any element in the class, but it's common to use the element that generates the class (i.e., the element that is used to define the equivalence relation).

<br><br><br><br>

***
# Orders
***

### Partial Orders

#### Summary:

A partial order is a relation that is reflexive, antisymmetric, and transitive. It is used to represent a partial ordering among elements of a set.

#### Definitions:

- **Reflexive**
: Same as the definition for equivalence relations.
- **Antisymmetric**
: For all x and y, if (x, y) and (y, x) are in the relation, then x = y.
- **Transitive**
: Same as the definition for equivalence relations.
- **Hasse Diagram**
: A graphical representation of a partial order.
- **Total Order**
: A partial order where every pair of elements is comparable.

#### Example:

Let R be a relation on the set {a, b, c, d} where (a, b) ∈ R, (a, c) ∈ R, (b, d) ∈ R, and (a, d) ∈ R.

This is a partial order. The Hasse diagram is:

```
    d
   /
  /
  b     c
   \   /
    \ /
     a
```

#### Tricky Things to Remember:

- A total order is a special case of a partial order.
- Hasse diagrams do not have loops or arrows, and they eliminate transitive edges.
---
### Total Orders

#### Summary:
A total order is a binary relation that is reflexive, antisymmetric, transitive, and total. In a totally ordered set, every pair of elements is comparable.

#### Definitions:
- **Binary relation**
: A binary relation on a set is a collection of ordered pairs of elements from the set.
- **Reflexive relation**
: A reflexive relation on a set is a relation where every element in the set is related to itself.
- **Antisymmetric relation**
: An antisymmetric relation on a set is a relation where, if `a` is related to `b` and `b` is related to `a`, then `a` and `b` are equal.
- **Transitive relation**
: A transitive relation on a set is a relation where, if `a` is related to `b` and `b` is related to `c`, then `a` is related to `c`.
- **Total order**
: A total order on a set is a binary relation that is reflexive, antisymmetric, transitive, and total.
- **Comparable**
: Two elements `a` and `b` in a set are comparable if either `a` is related to `b` or `b` is related to `a`.

#### Example:
Consider the set of integers `Z` with the total order relation "less than or equal to." In this total order, every pair of elements is comparable. For example, `1` and `3` are comparable because either `1 ≤ 3` or `3 ≤ 1` is true. Similarly, `-1` and `3` are also comparable because either `-1 ≤ 3` or `3 ≤ -1` is true.

#### Tricky Things to Remember:
- In a total order, every pair of elements is comparable.
- A total order is a more restrictive concept than a partial order.

---
### Hasse Diagrams

#### Summary:
Hasse diagrams are graphical representations of partially ordered sets. They provide a way to visualize the relationships between elements in a partially ordered set, making it easier to understand the structure of the set.

#### Definitions:
- **Partially ordered set**
: A partially ordered set (or poset) is a set equipped with a binary relation that is reflexive, antisymmetric, and transitive.
- **Upper bound**
: An element `b` in a poset is an upper bound of a subset `S` if `b` is greater than or equal to every element in `S`.
- **Lower bound**
: An element `b` in a poset is a lower bound of a subset `S` if `b` is less than or equal to every element in `S`.
- **Hasse diagram**
: A Hasse diagram is a graphical representation of a poset, where each element in the set is represented by a point or node, and the relationships between the elements are represented by lines or edges.

#### Example:
Consider the set of divisors of 12, partially ordered by the relation "divides." The Hasse diagram for this poset is:

<br>

```
         12
      /     \
     6       4
   /   \    /
  3      2
   \   /
     1
```

In this diagram, each node represents an element in the poset, and the lines represent the partial order relation between the elements. For example, the node labeled "6" is connected by an upward line to the node labeled "12" because 6 divides 12. The diagram is drawn in such a way that every node is above all the nodes it is greater than, and every line is drawn upwards to show the partial order relationship.

#### Tricky Things to Remember:
- Hasse diagrams can be a useful tool for visualizing the structure of a poset, but they can be difficult to draw accurately for large or complex posets.
- Hasse diagrams do not show all the details of the partial order relation, only the essential information needed to understand the structure of the poset.

---
### Topological Sort


#### Summary:
Topological sort is an algorithm used to put the elements of a partially ordered set (also called a directed acyclic graph) into a linear order. The linear order respects the partial order relation of the set, meaning that if `a` precedes `b` in the linear order, then there is no directed path from `b` to `a` in the graph.

#### Definitions:
- **Directed acyclic graph (DAG)**
: A directed acyclic graph is a graph that is directed (i.e., each edge has a direction) and acyclic (i.e., it has no cycles).
- **Partially ordered set**
: A partially ordered set (or poset) is a set equipped with a binary relation that is reflexive, antisymmetric, and transitive.
- **Topological sort**
: A topological sort of a directed acyclic graph is a linear ordering of its vertices such that for every directed edge `(u, v)`, vertex `u` comes before vertex `v` in the ordering.
- **Source vertex**
: A source vertex in a directed acyclic graph is a vertex with no incoming edges.

#### Example:
Consider the directed acyclic graph shown below:
<br><br><br><br>
```
     2    3
     |    |
     v    v
1 -> 4 -> 5
```

This graph can be represented by the partial order `{(1, 4), (1, 5), (4, 5), (2, 4), (3, 5)}`. A topological sort of this graph is `[1, 2, 3, 4, 5]`.

#### Tricky Things to Remember:
- A directed acyclic graph can have multiple topological sorts.
- If a directed acyclic graph has no source vertex, then it cannot be topologically sorted.

---
### Minimum, Maximum, Minimal, and Maximal

#### Summary:
In partially ordered sets, the terms "minimum," "maximum," "minimal," and "maximal" are used to describe the properties of elements with respect to the partial order relation.

#### Definitions:
- **Partially ordered set**
: A partially ordered set (or poset) is a set equipped with a binary relation that is reflexive, antisymmetric, and transitive.
- **Minimum element**
: An element `m` in a poset is a minimum element if it is less than or equal to every other element in the poset.
- **Maximum element**
: An element `M` in a poset is a maximum element if it is greater than or equal to every other element in the poset.
- **Minimal element**
: An element `m` in a poset is a minimal element if there is no other element `x` in the poset such that `x` is less than `m`.
- **Maximal element**
: An element `M` in a poset is a maximal element if there is no other element `x` in the poset such that `x` is greater than `M`.

#### Example:
Consider the set of integers `Z` with the partial order relation "less than or equal to." In this poset, the minimum element is `-∞` (negative infinity), and the maximum element is `∞` (infinity), because they are respectively less than or equal to and greater than or equal to all other elements in `Z`. However, there are no minimal or maximal elements in `Z`, because for any element `x` in `Z`, there is always another element `y` such that `y < x` or `y > x`.

#### Tricky Things to Remember:
- The terms "minimum" and "maximum" are used to describe unique elements in a poset (if they exist), whereas "minimal" and "maximal" describe a property of an element that may not be unique.
- A minimum or maximum element, if it exists, is always unique.
- A minimal or maximal element, if it exists, may not be unique, but every minimal (maximal) element is greater than or equal to (less than or equal to) every other minimal (maximal) element.

---
### Comparable Elements

#### Summary:
In partially ordered sets, two elements are said to be "comparable" if one is less than or equal to the other, or if the other is less than or equal to the one. Elements that are not comparable are said to be "incomparable."

#### Definitions:
- **Partially ordered set**
: A partially ordered set (or poset) is a set equipped with a binary relation that is reflexive, antisymmetric, and transitive.
- **Comparable elements**
: Two elements `a` and `b` in a poset are comparable if either `a` is less than or equal to `b`, or `b` is less than or equal to `a`.
- **Incomparable elements**
: Two elements `a` and `b` in a poset are incomparable if neither `a` is less than or equal to `b`, nor `b` is less than or equal to `a`.

#### Example:
Consider the set of integers `Z` with the partial order relation "less than or equal to." In this poset, any two distinct elements are either comparable or incomparable. For example, `1` and `3` are incomparable because neither `1 ≤ 3` nor `3 ≤ 1` is true. On the other hand, `1` and `-1` are comparable because `1 ≤ -1` is false, but `-1 ≤ 1` is true.

#### Tricky Things to Remember:
- Not all elements in a poset are comparable. Some pairs of elements may be incomparable.
- The concept of comparability is important because it allows us to define minimum and maximum elements in a poset, and it is also used in algorithms such as topological sorting.

---
## Principle of Inclusion/Exclusion

### Summary
The Principle of Inclusion/Exclusion is a counting technique used to calculate the size of a set formed by the union of several other sets. It provides a way to avoid over-counting elements that belong to more than one set in the union.

### Definitions
- **Union of sets**
: The union of two or more sets is the set of all elements that belong to at least one of the sets.
- **Intersection of sets**
: The intersection of two or more sets is the set of all elements that belong to all of the sets.
- **Cardinality of a set**
: The cardinality of a set is the number of elements in the set.
- **Principle of Inclusion/Exclusion**
: The Principle of Inclusion/Exclusion states that the size of the union of two or more sets can be calculated by adding the cardinalities of the individual sets, subtracting the cardinalities of the pairwise intersections of the sets, adding the cardinalities of the triple intersections of the sets, subtracting the cardinalities of the quadruple intersections of the sets, and so on, until the cardinality of the entire intersection of all the sets is added.

### Example
Consider the sets `A = {1, 2, 3, 4, 5}`, `B = {2, 4, 6, 8, 10}`, and `C = {3, 6, 9, 12, 15}`. The size of the union of these sets can be calculated using the Principle of Inclusion/Exclusion as follows:

$
|A ∪ B ∪ C|
$<br>
$
= |A| + |B| + |C| - |A ∩ B| - |A ∩ C| - |B ∩ C| + |A ∩ B ∩ C|
$<br>
$
= 5 + 5 + 5 - 2 - 1 - 1 + 0
$<br>
$
= 11
$

Therefore, the union of `A`, `B`, and `C` contains 11 elements.

### Tricky things to remember
- The Principle of Inclusion/Exclusion can be extended to any finite number of sets.
- When applying the Principle of Inclusion/Exclusion, it is important to take care not to over-count elements that belong to more than one set in the union.
