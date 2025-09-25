---
layout: essay
type: essay
title: "ESlint: My Digital Mother"
# All dates must be YYYY-MM-DD format!
date: 2025-09-25
published: true
labels:
  - Programming
  - JavaScript
  - ESLint
---

<img width="320px" class="rounded float-start pe-4" src="../img/messyroom.jpg">

# A long time ago, in a galaxy not so far away...

Many moons ago, humans began inventing our ultimate form of communication: language. Perhaps it started off as a simple "ooga booga", but eventually, from ancient civilizations, all modern languages we have today sprang. Most of us have taken English and literature classes, so we all understand how to structure and organize essays and paragraphs. My personal favorite structure is the persuasive essay structure, where I begin with an introduction, then transition into main points, counter any opposing points, and conclude gracefully. However, what if we had no structure in our literature? Imagine how much time we would be spending trying to understand messy essays and literature. Fortunately, we all understand how to structure information.

## Introducing ESLint.

The ultimate structuring tool for any TypeScript project. You may be asking yourself about the connection between my mini history lesson and modern programming. There are many similarities; for example, TypeScript is a language used by humans to communicate with computers and tell them what to do. Now, imagine we used TypeScript without any structure, such as the code below.

```ts
let x=10
const foo = () => {
var y = 20
    if(x>5){
console.log("x is greater than 5")
        }
        else{
            console.log("x is less or equal to 5")
    }
var unused = "I do nothing"
return y
}

foo()
function BAR(){
let z:number
z=5
if(z==5){
    console.log("z is 5")
}else{
console.log("z is not 5")
  }
}
BAR()
```

I'm not talking about code with bad syntax and code grammar, but rather, unstructured, pure chaotic code. Although the computer itself might have no problem reading and compiling this code, there are other humans who may still have to read and maintain this code. This not only makes software engineers' lives painful trying to read this, but it also wastes precious time for everyone. Time is money, and thus, by writing code like this, you are comparable to a cash thief. A bit of an exaggeration, but it's not far-fetched to say that writing code like this should be a crime.

## Just like my mother

ESLint helps software engineers and developers keep their code organized and structured, similar to somebody's mom yelling at them to keep their room clean. Although a bit annoying initially, ESLint makes your code professional and saves time for everyone. I also find that some of ESLint's feedback not only helps me write neat code, but also makes my code practically safe. Code that doesn't use extra unneeded memory, and code that is memory safe, so although ESLint likes to nitpick many tiny things and details, I find it a very useful tool.

*AI Used to generate messy code
