---
layout: page
title: Užovka
description: A simple imperative language interpreter written in Haskell
img: assets/img/snake.jpg
importance: 2
category: work
---

As a part of the course on *Declarative Programming*, I wrote an interpreter for a simple procedural language I called *Užovka* (Czech for *grass snake*).
Užovka is a simple imperative language with support for variables, and nested loops and conditionals. The keywords are in Czech.
The programs are read and interpreted from text files.

Here is an example of a program that computes the factorial numbers up to 50:

```python
Nechť n je 50;
Nechť faktorial je 1;
Nechť i je 0;

Dokud i < n
{
    Nechť i je i + 1; 
    Nechť faktorial je faktorial * i;
    Vypiš i + "! = " + faktorial;
}
```

And another example for the quadratic formula:

```python
Nechť a je 10.0;
Nechť b je 5.0;
Nechť c je -4.0;

Nechť d je ((b*b) - (4*a*c));

Pokud (d < 0) {
    Vypiš "No real roots";
}
Jinak {
    Pokud d == 0 {
        Vypiš "x = " + ((-b) / (2 * a));
    }
    Jinak {
        Nechť x1 je (((-b) + odmocnina d) / (2 * a));
        Nechť x2 je (((-b) - odmocnina d) / (2 * a));
    
        Vypiš "x1 = " + x1;
        Vypiš "x2 = " + x2;
    }
}
```

The code for this interpreter is available on our university's [GitLab](https://gitlab.mff.cuni.cz/bronecja/nprg005-ls2122-zapoctak).


