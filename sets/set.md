A set is a collection of distinct objects. The are usually denoted by capitalized letters and we have various ways of interacting with sets.

For example, a member of a set A, the following symbol usage is apt:
$$
a \in A \land (a \not\in A \implies \downarrow)
$$
We also have symbols for classifying if sets are subsets, that is if all the elements of one set can be found inside another.
$$
A \subset B \implies \forall a_{i} \in A : a_{i} \in B
$$
To specify a set we can if the objects are numerable and few use the following notation:
$$
A = \{ a, b, c \}
$$
But we also have set builder notation for more complex sets, these apply an enclosing set, a property of that set that the members of our new set must satisfy to produce our new set. Take for example:
$$
A = \{ x \in R \ | \ x < 10 \}
$$
This would mean 10 is not in $A$ but 9 and 9.5 is.
Given these groundworks, there are also certain quick forms for builder notation such as union and intersection.
$$
A \cup B = \{ x \in A \lor x \in B \ | \ x \not\in A \cup B \}
$$
$$
A \cap B = \{ x \in A \ | \ x \in B\}
$$
The last bit intersection introduces an interesting conundrum, what happens if two sets have no objects in common. In other words, they have no intersection, is it undefined?
No, we define it as the set of no objects, the empty set, a special set.
Some properties of this set are obvious such that no object can be a part of it. However, what about inclusion?
Well when we defined it we used the for all operator and if there are no objects to try the property for then it must be necessarily true as it is only false if there exists an object that does not satisfy the property.
Consequently, we know the empty set must be included in each set.