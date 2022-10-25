[_SOURCE: Bartosz Milewski | # Category Theory 2.1: Functions, epimorphisms_][ https://www.youtube.com/watch?v=o2lzkr-aaqk&list=plbgamihjbmenah_ltkxli7fma2hsnawm_&index=3]

## Functions

- functions must be pure and total
- a function is pure when you can memoize it
- the categories in FP are sets and functions between sets
- functions have a direction.
- it is ok for multiple values from the domain to map to a single value in the range
- it is not ok for a single value from the domain to map to multiple values on the range
  ![[func-direction.png]]
- The original set = Domain
- the target set = Codomain
- the subset of the Codomain the function targets = Image
  ![[jargon.png]]
- functions are not symmetric, they go one way and doesn't necessarily inverse, usually it does not inverse
- invertible is defined as if there are functions **_f :: a -> b_** and **_g :: b -> a_** AND **f⚬g** === **id.a** AND **g⚬f** === **id.b**, then it is invertible
- invertible functions are also known as isomorphisms
  ![[isomorphism-1.png]]![[isomorphism-2.png]]
- a function is not a isomorphism when the function collapses, ie: when to values in the domain map to a single value in the codomain
- a function is not a isomorphism when the image it makes on the codomain is only a subset of the codomains values, which means there will be some values of the codomain that don't map back to the domain. thus making it not possible to invert
  ![[not-isomorphism.png]]
- a function collapse is a process of abstraction, ie: isEven() goes from number to boolean. but not the other way
- a function mapping to a subset of the codomain is a process of modelling. we might not keep track of every real life detail of a car, but we might store in a DB {make, model, year, etc...} which is enough to work with
- a function that does not collapse, is **INJECTIVE**. that is it maps to every point to an individual point in the codomain _(or monic / monomorphism in greek)_
  ![[injective.png]]
- when a function maps all points in the codomain, it is known as **SURJECTIVE** _(or epic / epimorphism in greek)_
- category theorists like greek over latin
- a function that is both Surjective and Injective is an Isomorphism and can be inverted
