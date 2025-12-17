---
layout: essay
type: essay
title: "Designing against failure"
# All dates must be YYYY-MM-DD format!
date: 2025-12-04
published: false
labels:
  - Software Engineering
  - Design
---

<img width="500px" class="rounded float-start pe-4" src="../img/banana.jpg">

As I was walking through the town of NowhereVille, I stumbled across a farm of banana trees. I found the banana trees very yummy, but over time, I found that I wanted something more exotic to eat, like dragonfruit. Fortunately, thanks to my handy design pattern toolkit, I was able to use the factor design pattern to allow myself to instantiate different fruit trees based on my needs. Papaya, Coconut, the possibilities were endless.

## The beauty

Design patterns are beautiful; they allow us to take blueprints to approach and solve a variety of problems in software engineering, letting us gain more efficiencies within our systems. For example, take the following Python Code:

```python
cart = ShoppingCart(PayPalPayment())
cart.add_item(50)
cart.add_item(20)
cart.checkout()   # Paid 70 using PayPal.

# Change strategy at runtime
cart.payment_strategy = CryptoPayment()
cart.checkout()   # Paid 70 using Crypto.
```

Although not everyone uses the same payment method, by implementing the Strategy pattern, we can use different algorithms and functions within different code bases dynamically. This flexibility means we aren’t locked into rigid behaviors. Instead, we can swap logic in and out as our needs evolve. It’s almost like giving our code a set of interchangeable tools rather than forcing it to use a single one for every job. As our applications grow in complexity, this kind of adaptability becomes even more valuable, making our systems easier to maintain, test, and extend.

## What about us?

For our software engineering project, we have included a variety of design patterns. First of all, we have included the Adapter structural design pattern. This has allowed me to use a non-compatible React component to return data within a React Form component. Additionally, we also use the Decorator design pattern in which we give our website dynamic behavior, such as automated resizing to fit any screen while maintaining proper design ratios. Since we are using React, a lot of our code also uses the Observer strategy, in which components watch states and re-render whenever that state is changed.

I am still learning a lot about design patterns and structure, but one thing I know for certain is that without them, our project would be weeks behind. 

## AI used to generate Python code.
