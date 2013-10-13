BUILDING RUBY IN PYTHON - ALEX GAYNOR
-------------------------------------

why?
a story...

'Ruby is slow'
'CRuby is slow'

'I want rails to be faster'

Bad response
------------
 
- our app is IO bound 
- we make it up with programmer productivity
- if we need to make it fast we'll just rewrite in c, scal...

Why is CRuby slow?
------------------

the compiler doesn know the types therefor use

Consequences
------------

- all function call are indirect
- all containers are of "Object"
- instance variable lookups arent fixed memory offsets 

Lets design a fast Ruby!
------------------------

RPython - programming language
- statically typed + type interefence 
- garbade collected
- syntax is the same as python
- JIT compiler generator
- useful primitivies

Tracing JITs
------------

- observer for frequntly run code
- write down exacty what that code doeas
- generate ...

Key insight:
------------

- -maybe-
- -probably-
- almost certainly

The primitives RPython give us

@jit.elidable

jit.promote(x)

http://topazruby.com

- very fast
- incomplete
- cant run much real ruby code

feature
- run more ruby code (eg, gem, rails)
- interoperability with python

