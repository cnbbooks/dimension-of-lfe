# Introduction

This is a book about programming in _Lisp Flavoured Erlang (LFE)_, a dialect of the Erlang programming language family (_BEAM_ languages). In particular, it is a book that teaches the reader to create basic distributed systems applications. Furthermore, it does so in the context of creating a multi-user text-based exploration and adventure game.

In two very meaningful senses, this is a book of adventuring: the joy of learning something new and completely differnt and the excitment of writing a journey for your reader or creating a world for your player. Text-based adventure games were the original "Choose Your Own Adventure" book, in digital form before the concept made its way to print. What you will do in this book takes that idea a step further: not only are you choosing, you creating the choices for you and others to choose when your game is played. This can be anything you want, any narrative you wish to share. You don't have to tell the same story we do when we're sharing the code with you -- make it your own.

And remember, Adventure is Out There!

## Between The Covers

_The LFE Dimension_ is composed of severl major sections with a collection of chapters in each section. These sections have a broad scope of furthering the game and exploring deeper programming topics, guiding the reader into and through the territory of distributed systems.

After this introduction, the following sections with their main topics unfold:

* **Ground** - Getting up and running with Erlang and LFE
* **Trunk** - Wiring the core code that the rest of our adventure will ground around and upon
* **Branch 1** - The early beginnings of a world with narrative, navigation, and basic interaction
* **Branch 2** - More complex interactions, customising the game with commands, creating in-game events
* **Branch 3** - Databases, logging, game self-modifcation, a custom game shell
* **Branch 4** - Users, players, and Letting your friends log in, and chatting with them in-game
* **Branch 5** - Debugging, safety, integrating the game with a web app, and creating a client
* **Forest** - From one world to many, connecting your game to your friends' games

## Why This Book Was Written

For details on the backstory of this book, be sure to read the Preface! The summary, though, is a two-part answer: there are very few interesting books on learning about distributed systems and there are almost no (possibly zero) books on learning distributed systems by creating a fun game built using the core principles of that programming discipline.

While distributed systems are hard to think about and create, they are also a lot of fun! Core products at Google and other "big tech" companies would not exist without this tecnology. The WhatsApp text and voice chat application was written in Erlang and is an exmplare distributed systems product. Where are the fun books that teach people how to write their own WhatsApp?

## Who This Book Is For

The intended audience for this book is two-fold. First, the motivated and curious young readers wishing to learn the programming skills necessary to create multi-user applications that don't fail under load — but wants to have fun while learning these skills. Second, a less-young version of the population, who in their maturity, remember what it was like to program when everything was an adventure and every keystroke felt like magic.

### Assumptions

_The Dimension of LFE_ makes the following assumptions about tools and technical familiarity with one's operating system:

* The reader knows how to use a terminal, moving easily between multiple tasks running in different windows.
* The reader knows how to install software using the preferred package management tool for the given operating system.
* The reader is familiar with command line tools such as make and git.
* The reader knows what it means to program and either has some knowledge of a programming language, or wants LFE to be their first language.[^1]

### This This for Me?

The next question to answer, as you stand in the virtual bookstore of the LFE website, thumbing through the first pages of this book: is it something for me?

If you want to know more about how to create systems with incredible up-times, to learn the basics of a system that will let you write applications millions of people can access simultaneously,[^2] or to learn a language that will let you pass messages between embedded, clustered devices then you're going to want to carry this book up to the virtual cash register, give them no money (because the book is free), and then take it home with you.

You might not be here for the distributed systems allure, but for the Lisp: you may want to learn a dialect of the second-oldest surviving programming language, but want to do it on a modern virtual machine built for high-concurrency. You may want to see for yourself what all this talk of “Lisp macros” is, what _meta-programming_ can do for you, and find out what it really means for code to be _self-modifying_.

Finally, if you are interested in _Functional Programming_, in learning a language that from its early days described itself as a _functional concurrent language_, then you may want to read on. If you have a taste for small and growing communities that have a friendly culture to go hand-in-hand with your studies in functional programming, then you have come to the right place.

## What This Book Will Do

_The Dimension of LFE_ has several goals:

1. Bring the reader up to speed on the basics of a Lisp programming language, where a wealth of parentheses is feared no more than the ubiquitous curly brace.
1. Provide learning material that will support the reader as they re-imagine programming from the perspective of systems that need to stay up, stay in touch, and be available for the uncountable masses.
1. Create a new world, populated with things that exchange useful or engaging information using Erlang's model or communicating processes. 
1. Have an enormous amount of fun.

What this book will do, then, is guide you, the reader, on a learning adventure of a very practical nature – learning LFE – while at the same time weaving throughout the narrative and examples themes and highlights which reenforce the book's goals. These will give you a foundation in functional programming for systems of the future, providing you with the knowledge and skills necessary to make the next leap on your journey.

In his book _Introducing Erlang_, Simon St. Laurent says the following about how Erlang
will change the reader:

> “...You should know that working in Erlang may irrevocably change the way you look at programs. Its combination of functional code, process- orientation, and distributed development may seem alien at first. However, once it sinks in, Erlang can transform the way you solve problems...”

The same applies to the LFE programmer, and maybe even more so -- given its Lisp heritage.[^3] If you are successful in learning LFE, it _will_ transform the way you think about and solve problems. When features like message-passing, fault-tolerance, and high-concurrency are baked into a language, the resulting design patterns are incredibly well-suited to a vast domain of real-world communications problems. So well-suited, in fact, that once you do use them, their elegance and simplicity will cast long shadows on the arduous mechanisms which other languages require in order to accomplish the same thing.

This book will open the door to a future full of these vistas, and many more like it.

## How To Read This Book

This book is not a reference, it holds within its pages a narrative of incremental knowledge and the gaining of useful experience as one writes the code for each chapter. As such, one should not skip about but rather follow the story that is laid out for the reader in sequential steps. 

## Terms and Glossary

_The Dimension of LFE_ contains a great deal of new terminology. It contains so many new words and phrases that we have provided a glossary at the end of the book. When a glossary term is used for the first time, it is formatted with italics. For more context on these words, be sure to check their entries in glossary!.

## Formatting Conventions

The following typographical and formatting conventions are used in this book:

* _Italic_ – This is how we indicate new terms. Anything in italics will have a corresponding entry in the book's glossary. Note that italics are also used for book titles and emphasis; as such, words in italics will have to be examined in context to determine the likelihood of it being a glossary term.
* [example.com]() – This is how we indicate that the text represents a URL which can be entered in a web browser.
* `Fixed-width` – This is used for code within text, such as function names or executable binary files. It is also used for program listings. Note that LFE program listings will also be signified by coloured syntax-highlighting.
* **`Fixed-width bold`** – This is used when we wish to indicate code or commands that should be typed by the reader. Note that commands often include the prompt appropriate for the context (e.g., `$` for Bash, `#` for tcsh, and `lfe>` for LFE). These prompts are _not_ to be typed by the reader when entering the commands.
* `<Bracketed fixed-width>` – This is used for placeholder code which should be replaced by the user, for instance `(set name <your name>)`. The reader should replace the brackets and the text they enclose with the indicated value.

### Messages to the Reader

From time to time you will see call-out boxes, aimed at drawing your attention to something of note. There are four differnt types of these:

* ones that share useful info (blue)
* ones that highlight something of a momentus nature (green)
* ones that offer warnings to tred carefully (orange)
* ones that beg you not to follow a particular path (red)

These messages will take the following forms:

<div class="alert alert-info">
  <h4 class="alert-heading">
    <i class="fa fa-info-circle" aria-hidden="true"></i>
    Information
  </h4>
  <p class="mb-0">
    Here you will see a message of general interest that could have a useful or even positive impact on your experience in programming LFE.

The icon associated with this type of message is the "i" in a circle.
  </p>
</div>

<br/>

<div class="alert alert-success">
  <h4 class="alert-heading">
    <i class="fa fa-smile-o" aria-hidden="true"/></i>
    Amazing!
  </h4>
  <p class="mb-0">
    Here you will see a message of general celebration for sitations that warrant it, above and beyond the general celebration you will feel writing programs in a distributed Lisp.

The icon assocated with this type of message is a smile emoji.
  </p>
</div>

<br/>

<div class="alert alert-warning">
  <h4 class="alert-heading">
    <i class="fa fa-exclamation-triangle" aria-hidden="true"></i>
    Warning!
  </h4>
  <p class="mb-0">
    Here you will see a message indicating a known isssue or practice you should avoid if possible.

The icon assocated with this type of message is the "!" in a caution triangle.
  </p>
</div>

<br/>

<div class="alert alert-danger">
  <h4 class="alert-heading">
    <i class="fa fa-minus-circle" aria-hidden="true"></i>
    Danger!
  </h4>
  <p class="mb-0">
    Here you will see a message indicating something that could endanger the proper function of an LFE system or threaten the very existence of the universe itself.

The icon assocated with this type of message is "do not enter".
  </p>
</div>


----

#### Notes

[^1] If tis is your first language, you may want to read the early chapters of [The LFE Manual](https://lfe.io/book/chinenual), walk through [The LFE Tutorial](https://lfe.io/books/tutorial/), and maybe even play with [Casting SPELs with LFE](https://lfe.io/books/casting-spels/).

[^2] WhatsApp, the company acquired by Facebook for 19 billion USD, wrote the backend for their famous chat application using the Erlang VM. At the time of the purchase, WhatsApp had 450 million users. A the time this book was conceived (2015) the userbase had grown to 700 million active monthly users with over 30 billion messages been sent on a daily basis. Now, eight years later, who knows how many more users WhatsApp supports? 

[^3] A language where mind-bending concepts such as self-modification are elevated to nearly the status of an ethos.
