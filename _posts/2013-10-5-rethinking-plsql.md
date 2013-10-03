---
layout: default
title: Rethinking PLSQL
---

#Rethinking PLSQL

Early in my career as a programmer, I learned to dislike PLSQL. I couldn’t stand the convention of all caps, the mess that even the simplest procedures and functions turn into and the syntax that made me feel like I was in some sort of strange programming paradox.

That is, until I thought about it more. The things that I was really annoyed about concerning PLSQL weren’t actually issues with PLSQL itself, but instead the conventions people tended to follow. It’s almost as if once they dropped from Java, or any other language, all the best practices and years of collective knowledge about separating concerns, maintainability and readability went out the window, and that was seemingly ok.

Instead, I propose a new system, one in which takes the best practices that we all know and love and applies them in a meaningful way on the database side. 

## 1. Don't use all caps
This cannot be stressed enough. Study after study has proven that using all caps reduces comprehension and speed of the reader, plus it’s just plain rude by today’s standards. Instead, use either camelCase or under_score.

## 2. Use meaningful names
I’ve seen too many examples where a pseudo-hungarian notation model is followed, usually for things like v_ for variable or pkg_ for packages. PLSQL has fine namespacing, and the code should never be long enough where you forget which things are variables, packages, triggers, etc. Instead, use meaningful names, just like you would in any other language.

## 3. Separate your concerns
Every programmer worth his or her salt will separate the concerns of the code, and PLSQL is no different. Follow some sort of logical structure, whether that is a business logic layer on top of your data access layer, or something else, just don’t stick everything under the sun in one procedure, it just leads to more hassle than it’s worth.
