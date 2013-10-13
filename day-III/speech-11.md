BUILD YRSELF CLEAN - NICK FISCHER
---------------------------------

from source to browser, making it fast

contact: @spadgos

www2.warneeeerbroc.com/spacejam/movie/

2004 - Google produce Gmail

If you dont know what to uglify is, you are a simpleton.

Modular code:
-------------

- requirejs, browserfy
- better tools for builds: r.js

Optimisation:
-------------

- improve network & runtime performance

Technics:
---------

* asset hashing
 - ise an identigying hash
 - checksum of content, git commit shad, whatever
 - simplifies cachnig: cache forever!
 - multiple versions side by side
 
Find and rewrite 
----------------

- helper function __ASSET()
- ...

Qcuick difression: ASTs
- abstract syntax trees

AST Manipulation
----------------

```
var imgpath = __ASSERT('imgages/..jpg)
var ast = Uglify.parse(filecontent);
ast.transform(
  Uglify.Treetransformer(function (node){
    if )node instance Uglify.AST_Call)

```
 
A small downside:
-----------------

no dynamic naming

Bucketing scripts
-----------------

* parallel loading
* more effective caching

Domain sharing
--------------

Per domaing connection limits
-----------------------------

- chrome, ff, sata, opera - 6 per domain
- is - 8 per domain 

Split assets aross multiple domains
-----------------------------------

Number from 3 to 4 uniq domains

Asset rewriting
---------------

__ASSET('file.jpg) // => //a2.site.om/asdasdasd.jpg

AST transormation again
- step1: find all: foo = require ('bar') remote
- step2: replace with a delayed and cached call

Targetted builds
----------------

- jquery - 2 versions
- lo-dash / underscore 

Choose your envoroument
- mobile, legacy, modern...

Variables can be set at built time

Dead code automatically remove during minification

Page specific packages
----------------------

What? - split modules into 'core' and 'page specific'
- core - run on all page
- specyfic - run only under current page

When?
- when your total size is getting to large
- when low traffic pages contain a lot of unique code

How?
... i dont cath it ;/

http://spadgos.github.com/rupy13

- use source maps

