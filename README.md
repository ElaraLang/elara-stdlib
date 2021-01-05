The Official Standard Library of the Elara Language

This repository includes the standard library for the Elara Language. This library is required at runtime and a program written in Elara will not function without it.


## Want to Contribute?

Great! We don't have a specific policy at the moment, but here are a few guidelines:
* Different parts should be in specific packages. For example, utilities for working with strings will be in the `elara/std` namespace, but in a subdirectory named `strings` or `text`. Packages are more open ended than Java's packages, so don't feel like you should be too specific.
* Bear in mind that all syntax is not finalized and may be adjusted.




## Collections
The current plan for collections is as follows:
* Collection Literals for lists and maps
* Persistent Data Structure implementations (these are a type of data structure that can be copied quickly but are immutable. Linked Lists are a simple example, as are trees)
* For data structures with specific semantics (eg a Hash Set), add extension functions to the basic List and Map types. 
For example 
```
  extend List<T> {
    let to-set => Set<T>(blah)
  }
```
