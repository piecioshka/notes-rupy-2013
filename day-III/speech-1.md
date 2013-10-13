HARD DRUGS, ROCKSTAR PROGRAMMERS, AND C++ - JAMES GOLICK
========================================================

> a lot of code examples

method resolution is slowly
uint - unsigned integer

Global method cache
-------------------

if you have above 2048 method names theres land to global cache

Cache invalidation
------------------

Thins that bust the cache
- defined met
- aliasing met
- remove met
- extendint a module
- using a refinement
- garbage collcting a class
- garbage collecting a module
- changeing the visibility of a constt
- autoload
- buiilt-in non blocking I/O

Summary
-------

- method resolutions are cached in two places
- istruction cahces are structs attache to the send instruction
- the global method cache is a hash table fixed at 2048 entries with no
collision
- method cache invalidation is always global and happends frequenyl in
most ruby code
- both types of method cache entries now only need...
- method caches are invalidaed by assingin a new sequence valie to a
klass
- when cahanges are made to a klass we traverse all of its descendents
and assign them new sequence values
- his traversal is unfortunately a variable time algorithm and anbe
quite expensive
- entries are valid if theis filled entry sequence is the...

Numbers
-------

> 3.jamesgolick method caching
> 4.rvm install jamesgolick

Dat patch
---------

- top-down class hierarchy tracking
- class#subclasses 
- module#include_in
- possible future bug fixes
- hierarchucal method cache invaliddtion
- method cache instrumentation

