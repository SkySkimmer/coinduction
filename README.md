# Coinduction

A library for doing proofs by (enhanced) coinduction.

It is based on the notion of 'companion' from the paper
Coinduction All the Way Up. Damien Pous. In Proc. LICS, 2016.

It contains:
 - enhancements of the coinductive proof method
 - second order coinduction reasonning about enhancements
 - parametrised coinduction, as proposed by Hur et al.
 - powerful symmetry arguments
 - compatibility and respectfulness
As well as examples for using the library: 
 - a formalisation of Hur et al's toy example on divergence 
 - a formalisation of Rutten's stream calculus
 - a formalisation of Milner's calculus of communicating systems (CCS)
 
## Modules
 + `lattice.v`     : complete lattices, monotone functions in such lattices
 + `coinduction.v` : abstract theory of coinduction in complete lattices, companion
 + `rel.v`         : tools for the complete lattice of binary relations
 + `divergence.v`  : Hur et al's example on divergence 
 + `streams.v`     : Rutten's stream calculus 
 + `ccs.v`         : Milner's CCS 

## Meta

- Author(s):
  - Damien Pous (initial)
- Coq-community maintainer(s):
  - Damien Pous ([**@damien-pous**](https://github.com/damien-pous))
- License: [GNU LGPL](LICENSE)
- Compatible Coq versions: 8.13 or later
- Additional dependencies:
- Coq namespace: `Coinduction`
- Related publication(s):
  - [Coinduction All the Way Up](https://hal.archives-ouvertes.fr/hal-01259622) doi:[10.1145/2933575.2934564](http://dx.doi.org/10.1145/2933575.2934564)

## Building and installation instructions

The easiest way to install the latest released version of Graph Theory
is via [OPAM](https://opam.ocaml.org/doc/Install.html):

```shell
opam repo add coq-released https://coq.inria.fr/opam/released
opam install coq-coinduction
```

To instead build and install manually, do:

``` shell
git clone https://github.com/damien-pous/coinduction.git
cd coinduction
make
make install
```