# js-object-composer
Object composer creates objects from other objects. The returned object doesn't inherit their functionality in a ''classical'' way of thinking. It just borrows it.

WARNING: PRE-ALPHA version. If yoou are interested in the functionalaty this project is intended to provide in the future I recomend you to use [stampit](https://github.com/stampit-org/stampit) which is stable and it's ben tested in lots of production projects.

## Composition over inheritance in javascript
I like composition much more tha inheritance when trying to reuse code. While trying to understand prototypal inheritance deeper I found a talk given by Eric Elliot talking a project of his, stampit. It sounded very well and I remember having a look at the source code and not understanding almost anything. But I thought I could try to replicate the functionality and use the exercise to learn more about it.

The initial objective for this mini-library is to help create objects and borrow functions from other ones in the way a usually do it, sing constructor functions and forgetting inheritance is there at all. 
The constructors I build only put instance data on the object itself (as owned properties). The rest (methods and shared data betwen objects of the same type) goes in the delegate prototype. 

TODO: Include an object example showing the prototype chain

TODO: Explain how to build an object composing other three: one data object and two behaviours

TODO: Include images of the original objects and how the information gets copied to different prototype levels

TODO: Try to avoid classical inheritance terms and expressions in the explanations

TODO: Explain why I think it's better to use flattened prototype chains instead of compose inheriting one prototype after another -> mutability of the prototype chain -> you don't loose anithing, you can compose again to update the changed methods and shared data.


## Intended features
- [x] Allow composing objects by borrowing functionallity or extending with data
- [x] Produce objects and/or constructor functions for those objects
- [ ] Introduce TDD in the dev workflow (Have to learn TDD first)
- [ ] Figure out what to do about circular references. At least for typical use cases like linked lists or trees. Are they a problem?
- [ ] Allow decomposing (is it possible in all cases?). I don't see why it would be useful but I want to check it out
- [ ] Allow composing constructor functions (as stampit does)
- [ ] Stabilize at leas the most important API methods (Need to find the right terms for each operation)
 
