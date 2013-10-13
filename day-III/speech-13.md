NOBODY KNOWS RUST - STEVE KLABNIK
=================================

Rust is a really interesting new programming language.
Rust is a good choice when youd'd chooce C++. And maybe other times.

Origins

Rust was written by Graydon Hoare. Mozilla has taken stewardship.
Mozilla writes lots of C++, and feels tha pain.

Usage for Rust 
--------------

Rust is written in Rust.
Mozilla is developing Serve in Rust as well.

Servo
-----

Serve is a web rendering engine. Think Gecko or WebKit.
There are no plans ro replace Gecko. It is focused on mobile.
Massively paralell.

Stability
---------

Rust is currently at version 0.8
Snapshots, not backwards compatible.
1.0 is coming soon.

The ten gifts of #rustlang
--------------------------

* Functions
 fn main() {
   println('ad')
 }
 fn foo(i: int) -> int {
   5;
 }
* Variables
 fn main() {
    let num = 1; 
    let mut num = 1;
    let mut nut :int = 1;
 }
* Vector
 let nums = [1, 2];
* Mutation
  let mut 
* Cosures
 let double = |x: int| -> int { x * 2 };
 let x = double (5);
* Iteration
 let mut odds = nums.iter().map(|&x| x * 2 - 1);
* Tasks
  for num in odds {
    do spawn { 
      printl("{:s} says...");
    }
  }
* Generics
* Traits
* Pointers
  let x: ~int = ~5;
  println((*x + 5).to_str());
  
Tasks and ARC
-------------

Bonus! Match
------------

Introductions
-------------

- the officail tutorial
- rust for rubists


Discussion Fora
---------------

- the rus-dev mailing list
- /r/rust
- #rust on irc.mozilla.orf
- This Week in Rust

Code
----

http://github.com/mozilla/rust

