[_SOURCE: Bartosz Milewski | Category Theory 1.2: What is a category?_][ https://www.youtube.com/watch?v=p54hd7amvfu&list=plbgamihjbmenah_ltkxli7fma2hsnawm_&index=2]

![[what-is-a-category.png]]
It is kind of like a Graph but may have infinitely many edges and infinitely many nodes

## Composition

![[Composition.png]]
Is a property such that if you have objects _A, B and C_ and there exists a edge **f** from A->B and a edge **g** from B->C. Then there must also be an edge **g⚬f** (g after f) from A->C

### Note:

- edges, also known as arrows or morphisms
- in Functional Programming the vehicle for a morphism is a function
- in Functional Programming the category objects are types

## Identity

![[Identity.png]]
For every object i na category there is one edge, know as Identity that just points at itself.
It has the property of **id⚬f** = **f** = **f⚬id**

## Associativity

![[associativity.png]]
There may be many ways to compose morphisms but if two compositions with the same morphisms in differing orders end at the same value, they are considered equivalent.
ie: **h⚬(g⚬f) === (h⚬g)⚬f**
