# Preface

This book was conceived after working on other book projects whose aims were to teach programming via fun an interesting narratives. While several programming languages have fun books like that, to my knowledge (then, in 2015, as well as now, in 2023) there is no book in that vein that teaches the basics of distributed systems.

This seemed like a huge hole in the world of books, stories, and programming -- so after some thought, I sketched out a way of teaching these materials in the context of creating game with the reader, an interactive text adventure built upon principles of distributed systems. This would, of course, mean that when done, the reader would be able to let their friends (or anyone on the planet with a computer and an internet connection) join the game to play and chat in a world of their own creation! How exciting for a new (or old) programmer!

With these thoughts on paper and in hand, I wrote to my favourite book publisher. They loved the idea but were concerned the market was too small and asked if I would be interested in writing a similar book for a more mainstream programming language. My love for LFE was too strong, though! I had hoped one day to write this book, and now that it is happening, let me share with you part of what I sent the publisher.

----

The vision of The Dimension of LFE is that of a high-technology book which takes the reader from the coastal plains of Hello World, through the dense forests of Functional Programming and Immutable Data, climbing the foothills of Multi-user Access, wandering under the mountains into the Lost Caves of Message Passing, delivering them at long last to their journey's secret goal: the Shangri-la of Distributed Applications. In the spirit of _Casting SPELs in Lisp_ and _Realm of Racket_, the common theme running through the book will be the creation of an adventure game, culminating in reader's pride and joy: a Multi-User Dimension (MUD)[^1] they can share with friends — in more ways than one! (Or two!) 

We live in a world of seemingly unbounded communications — we are surrounded by phones, social media, blogs, websites, just to name a few. The technology to efficiently power these continues to evolve, but for the most part grows more difficult to understand and can take years to teach. The Erlang programming language made great advances in this area, allowing individual programmers to more easily create robust distributed applications — once they learned the rather archane syntax.

Lisp Flavored Erlang provides the same capability for creating fault-tolerant services as Erlang itself (being compatible with and running atop Erlang), while offering the learner an easier path to discovery, as well as more features (most significantly, Lisp macros and in-REPL function, record, and macro definitions). Students who have previously encountered Scheme or Lisp, or who have been exposed to algebra's parentheses and order of operations, will find the transition to LFE comfortable and familiar. 

Having established that comfort in the first few pages, the reader will be whisked into an adventure of the best learning experience of all: creating a new world. Starting in bits and pieces, we will move from basic concepts to a working game. Through guided tasks that serve to not merely add flavor to their creation, but introduce concepts and programming techniques which allow them to reinvent their game to progressively better suit more compelling contexts. In short, the content of _The Dimension of LFE_ will be presented one step at a time in a natural and thematic way, leading through the challenging concepts of distributed systems with clarifying insights, practical demonstrations, and guided coding all of which will make the game more fun to play! 

As each concept will entail the best practices for building software using the Erlang VM and the Open Telecom Platform, not only will the new programmer be equipped for a whole new world of distributed systems through practical examples, but the experienced programmer will have a hands-on reference of material rarely found in the world of Lisp. 

--- 

#### Notes

[^1] Also called "Multi-User Dungeon" a la "Dungeons & Dragons"; for more history and context, see https://en.wikipedia.org/wiki/Multi-user_dungeon
