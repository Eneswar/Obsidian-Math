---
tags: 
title: Obsidian mathJax cheatsheet
---

# Obsidian Mathjax cheatsheet and references

If you notice anything out of place, a mistake somewhere or if you think something is missing, please reach out to me and let me know.
## Basics

To get started, obsidian is using something called [MathJax](https://docs.mathjax.org/en/latest/basic/mathjax.html), which is an open-source JavaScript display engine, to display mathematical formulas when you enclose them with the dollar signs. You can do this in two ways, either inline by enclosing your formula or equation with a single dollar sign like so `$5+5=10$` which will display it as $5+5=10$ or you can use double dollar sign which will display it as it its own full line like so `$$5+5=10$$` which becomes like this:

$$5+5=10$$

You will notice as you write formulas and equations that the inline math will sometimes display some symbols differently then in a full math block, it will look mushed in together. Compare these inline equations, `$\sum_{i=1}^{n}f(x)$` $\sum_{i=1}^{n}f(x)$ and `$\lim_{ n \to \infty }f(x)$` $\lim_{ n \to \infty }f(x)$, and now look at the same equations in a math block which will render them "properly":

$$\sum_{i=1}^{n}f(x) \text{ and }\lim_{ n \to \infty }f(x)$$

By enclosing your equation or the symbol with `\displaystyle` you can force the inline block to render it fully like so `$\displaystyle{\sum_{i=1}^{n}f(x)}$` $\displaystyle{\sum_{i=1}^{n}f(x)}$, although you will notice that the line will look slightly bigger when you do this so you may want to stick with the mushed in version.

For superscripts and subscripts you want to use `^` and `_`. Keep in mind that these scripts only affects the next single item, for example lets say you want to use $x$ and superscript $n+1$ to it, notice how only the first item will get scripted $x^n+1$. If you want to super- or subscript longer then one item you need to enclose it with curly brackets like so `$x^{n+1}$` $x^{n+1}$ or `$x_{n+1}$` $x_{n+1}$.

That is also why you need to escape the curly brackets if you want to show them in your formulas `$\{5+5\}$` $\{5+5\}$ otherwise they will not be shown `${5+5}$` ${5+5}$. Other parentheses works normally without the need to use escapes.

One thing I want to add regarding parentheses and brackets, when you add them part of a fraction, sums or integral you will notice that the parentheses looks smaller than the rest of the formula, here are some examples:

$$x=( \frac{10}{5}),\quad \sqrt{ 2^{2}+(\frac{3}{2}})$$

If you instead add `\left` before the left bracket and `\right` before the right bracket, you will notice that they will be scaled up to the size of the formula that they are enclosing.

$$x=\left( \frac{10}{5}\right),\quad \sqrt{ 2^{2}+\left( \frac{3}{2} \right)}$$

This works for all kinds of brackets, so give it a try yourself.

## Greek letters and fonts

To write Greek letters simply write `\alpha`, `\beta`, `\sigma`, and for uppercase just uppercase the first letter `\Sigma`.

> [!info]- Greek letters
> 
> | Letters                     | Code                      |
> | --------------------------- | ------------------------- |
> | $\alpha, A$                 | \alpha, A                 |
> | $\beta, B$                  | \beta, B                  |
> | $\gamma, \Gamma$            | \gamma, \Gamma            |
> | $\delta, \Delta$            | \delta, \Delta            |
> | $\epsilon, \varepsilon, E$  | \epsilon, \varepsilon, E  |
> | $\zeta, Z$                  | \zeta, Z                  |
> | $\eta, H$                   | \eta, H                   |
> | $\theta, \vartheta, \Theta$ | \theta, \vartheta, \Theta |
> | $\iota, I$                  | \iota, I                  |
> | $\kappa, K$                 | \kappa, K                 |
> | $\lambda, \Lambda$          | \lambda, \Lambda          |
> | $\mu, M$                    | \mu, M                    |
> | $\nu, N$                    | \nu, N                    |
> | $\xi, \Xi$                  | \xi, \Xi                  |
> | $o, O$                      | o, O                      |
> | $\pi, \Pi$                  | \pi, \Pi                  |
> | $\rho, \varrho, P$          | \rho, \varrho, P          |
> | $\sigma, \Sigma$            | \sigma, \Sigma            |
> | $\tau, T$                   | \tau, T                   |
> | $\upsilon, \Upsilon$        | \upsilon, \Upsilon        |
> | $\phi, \varphi, \Phi$       | \phi, \varphi, \Phi       |
> | $\chi, X$                   | \chi, X                   |
> | $\psi, \Psi$                | \psi, \Psi                |
> | $\omega, \Omega$            | \omega, \Omega            |

Below here I will go slightly deeper into each type.

## Fractions

Fractions can be written in two ways, for very simple fractions such as $x=\frac 12$ you can simply just write `\frac 12`. For more complicated fractions you need to wrap each numerator and denominator in curly brackets $x=\frac{5^{2}+5+10}{1+4}$ `x=\frac{5^{2}+5+10}{1+4}`, which pretty much applies to most, if not all, types of equations. Curly brackets is your friend.

## Sums and integrals

Sums and integrals follows the same rules mentioned above. including the curly brackets and sub/superscript.
...
## Limits

...
## Aligning

...
## Symbols

...
## Matrices

...
## Arrays

...
## Manipulations

...
## Environments

...
## Tagging

...
## Examples

...
