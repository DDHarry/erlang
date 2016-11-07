# Programming Style Guide for [mweet.me](http://mweet.me)


## Conventions used for this style guide

>$ for the *nix Shell

>\> for the Erlang Shell

>*\>\> the result*


## Table of content

1. [Compiling greetings.erl] (#compiling)

2. [Types](#types)



## 1. [Compiling](#compiling)

### [1.1](#compiling--nix-shell) Compiling and Running in the *nix Shell
The Hello World program :

```erlang
-module(greetings).
-export([hello/0, hello/1]).

hello() ->
  io:format("Hello the World ~n").

hello(Someone) ->
  T = [Someone],
  io:format("Hello ~ts~n", [Someone]).
  
```

>$ erlc greetings.erl

>$ erl -noshell -s greetings hello -s init stop

>*\>\> Hello the world!*

Now with an input name :

>$ erl -noshell -s greetings hello Bob -s init stop

>*\>\> Hello 'Bob'!*

**[ &#8679; Back to the top](#table-of-content)**


## [1.2](#compiling--erlang-shell) Compiling and Running in the Erlang Shell
$ erl

> \> c(greetings).

>\> greetings:hello('Bob').

>\>\> Hello Bob

**[&#8679; Back to the top](#table-of-content)**




#2. Types
##[2.1](#types--atom)atom

An atom is 
*atom*


here

**[ &#8679; Back to the top](#table-of-content)**



