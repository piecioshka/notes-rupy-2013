INTRODUCING ERLANG - BOB IPPOLITO
=================================

What do I know?
---------------

- erlang user sicne 2006
- ericsson language

Agner Krarup Erlang

Raison date
-----------

- came from ericsson r&d in the 80s
- telecom shifting to packet switch ing
- multi-service networks
- improve developoemtn of telephony apps
- scalable, distrubutted

Domain 

Apps 
- netoworking
- messaging (sms, mms, im) services
- distributed systems
- web services
- simulation
- game servers

Erlang solution
- conference
- training
- certification
- consulting
- support

advertising
- mochi media
- adroll 
- openx
- adgear
- AOL

Cloud / Data center automation

Moile / VoIP

Media:
- the boston blabe
- the huffinmang post

Games:
- spilgames
- wooga
- muchdifferent

Money:
- klarna 
- smarkets

Open source
- riak 
- couch db
- ejabberd
- rabbit

Not good for:
- client side app GUI
- but web0bases UI work well
- number crunching

Ancestry
- syntax mostl form prolog
- list compregensions from Miranga (like haskell)
- pattern matching like ML

Key feature
- declarative
 - descrive the problem, not the solution
 - great suntax for this (but not C-like)
 - convenient bit syntax for parsing binary data

Concurernt
----------

- RAM footprint per unit of concurrency (approx)
- per-process heads
 - no sharing 
 - gc is per-process, and not 'stop the world'
 - process references do not prevent GC
 - explicity hibernate idle processes for compaction
- RPC with a Counter process
- multi-core
 - one scheduler per core, scales well to 32+cores
 - better scalability to more cores is in-progress
 - schedulers understand IO (disk, network call)
 - no impicit synchronization

Distributed
- buit-in distributed computing support
- easy to get started 'no configuration'
- same syntax, similar semantics, wharhe local on not
- necessary for true fault tolerant systems

Robust
- OTP - framework encodes these best practices
- versatile
 - upgrade/fix live systems with hot code loading
 - debug/profile live system with tracing
- functional
 - no mutable data structures
 - linked list
- modules
 - flat namespace
 - explicit export of public functions
 - referenced by name (atom)
 - compiled to '.beam' file
 - can be reloaded in a running system

More info
---------

- erlang.org
- erlang-central.org
- erlang-factory.com
- learnyousome...

slides: http://bob.ippoli.ro/intro-to-erlang-2013/
sources http://github.com/etrepum/intro-to-erlang-2013/ 
@etrepum

