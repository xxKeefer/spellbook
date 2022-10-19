[*SOURCE: Bartosz Milewski | Category Theory 1.2: What is a category?*][ https://www.youtube.com/watch?v=p54Hd7AmVFU&list=PLbgaMIhjbmEnaH_LTkxLI7FMa2HsnawM_&index=2]

![[what-is-a-caegory.png]]
It is kind of like a Graph but may have infinitely many edges and infinitely many nodes

## Composition
![[Composition.png]]
Is a property such that if you have objects *A, B and C* and there exists a edge **f** from A->B  and a edge **g** from B->C. Then there must also be an edge **g⚬f** (g after f) from A->C

### Note:
- edges, also known as arrows or morphisms 
- in Functional Programming the vehicle for a morphism is a function
- in Functironal Programming the category objects are types

## Identity
![[Identity.png]]
For every object i na category there is one edge, know as Identity that just points at itself.
It has the property of **id⚬f** = **f** = **f⚬id**

## Associativity
![[associativity.png]]
There may be many ways to compose morphisms but if two compositions with the same morphisms  in differing orders end at the same value, they are considered equivolent. 
ie: **h⚬(g⚬f) === (h⚬g)⚬f**

