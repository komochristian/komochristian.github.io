---
layout: essay
type: essay
title: "The Type of Mess TypeScript is"
# All dates must be YYYY-MM-DD format!
date: 2025-09-09
published: true
labels:
  - Programming
---

TypeScript is really one of the most chaotic and unreadable languages in the world. Sure, catching errors before runtime saves a lot of fire, having type definitions in my IDE saves lots of time and hassle, and explicit type definitions save hundreds of emails from other developers, but at the end of the day, Typescript has taken away the fundamental simplicity that a high-level language, like JavaScript, was supposed to provide originally. 

While many of you may be sending angry messages to me on LinkedIn, take, for example, the following code:

 ‘’’javascript

type Callback<T> = (error: Error | null, result?: T) => void;

function fetchData<T extends object>(

  url: string,

  options?: { headers?: Record<string, string>; timeout?: number }

): Promise<T> & {

  cancel: () => void;

} {

  let canceled = false;

//...

‘’’

Understandably, for most of you, who are obviously full-stack and 10x developers, this may be quite a trivial piece of TypeScript. However, for those who spend time with other languages, this looks like a complete heap of messy words. What happened to the simple syntax of high level languages?? What happened to a simple print() statement like Python? 

##  MY TYPE OF TESTIMONY

Take me back to when I started learning React with zero JavaScript or web development knowledge. Although the functional syntax, structure, and system of .jsx code was intimidating and hard to dive into initially, as I researched, YouTube’d, and ChatGPT’d, I gained more and more knowledge of JavaScript till I was a pro. The simplicity of JavaScript is messy, yet it allows for a fairly easy visual learning process.

##  FORGIVE ME TYPESCRIPT

Despite my sins of blaspheming against Typescript and its holy online church, Typescript sure has its ways with project development. Instead of going through 400 lines of code in my project trying to see how to format my JSON object in JavaScript, Typescript allows me to immediately eliminate 15 minutes of debugging run-time errors, the seamless integration with my IDE allows me to crank code faster, and it’s compilation into Javascript is extremely useful. Typescript, definitely a weird type of combination of different languages, but a useful one.



