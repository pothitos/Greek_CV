# Source Code for a Greek CV [![Build Status](https://travis-ci.org/pothitos/Greek_CV.svg?branch=master)](https://travis-ci.org/pothitos/Greek_CV)

 - From the LaTeX source code a
   [__PDF__](http://di.uoa.gr/~pothitos/KomninouCV.pdf) is
   automatically produced.

## Hyphenation for Combined English and Greek

 - We attempt to use both English and Greek words without
   explicitly declaring their language, e.g. by using the
   annoying commands `\textlatin{english words}`,
   `\selectlanguage{greek}`, etc.
 - To do so, we use the Unicode character encoding, which is
   LuaLaTeX's default.
 - However, the hyphenation rules require an explicit
   language declaration to apply.
 - To overcome this, we use the language `dumylang` and
   combine in it the English and Greek hyphenation rules.
 - See [`.travis.yml`](.travis.yml) and the relevant [Stack
   Exchange answer](https://tex.stackexchange.com/a/325899)
   for more :wink:
