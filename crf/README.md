This directory contains a very simple (and, when it comes to feature computation, very inefficient) C++ program to learn the parameters of a linear chain CRF model using [automatic differentiation](http://en.wikipedia.org/wiki/Automatic_differentiation).

The classical forward algorithm is used to compute the CRF training objective, and rather than explicitly writing the backward algorithm to compute the derivatives, I rely on the adept autodifferentiation library.

To build this code, you need:

 * A C++11 compiler
 * The [Adept (Automatic Differentiation using Expression Templates) library](http://www.met.reading.ac.uk/clouds/adept/) installed

To compile and run this code:

    make
    ./cref sample.conll
