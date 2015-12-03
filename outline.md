# Outline
### Abstract
* Humans
* Ceasar
* secrecy
 
### Motivation

* Symmetric Key
  * History?
    * War
    * WWII
* Public Key Cryptosystems
  * 

### Mathematics
* Modular Artithmatic
  * Congruences
    * for n\in\N, a,b,k\in\Z
      * a = b (mod n) iff a=b+kn
      * alt, if \frac{a-b}{n}=k\in\Z
    * ie, numbers can be said to "loop around" a modulus n.
    * Example: time. 2hrs and 220 minutes is congruent to 5 hrs and 40 minutes, because minutes are counted mod 60.
  * something something
  * Euler's Phi Function - Should this be in Number Theory?
    * OK, Euler is great.
    * 
* Number Theory?

### The RSA Algorithm
* Here it goes
  * Bob picks two primes p, and q
  * n = pq
  * Bob chooses e
  * Bob sends n and e to Alice
  * Alice encrypts her message m by c=m^e (mod n)
  * Meanwhile, Bob computes de = 1 (mod (p-1)(q-1))
  * Alice sends c back to Bob.
  * Alice's message m=c^d (mod n).
* Why does it work?
  * Part 1: Why can Bob recover Alice's message?
    * Apply modular arithmetic
    * if x=y (mod \phi(n)), then a^x=a^y (mod n)
    * ie, c^d = (m^e)^d = m^de = m^1 = m (mod n)
    * bc de = 1 (mod \phi(n))
  * Part 2: Why is it difficult for Eve to do so?
    * It's all about \phi(n).  It is very hard to find, as the algorithm depends upon the factors of n.
    * Given a big number....














