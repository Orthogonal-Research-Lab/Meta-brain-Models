Google n-gram 

* viewer (English) [link](https://books.google.com/ngrams)

* open dataset [English n-grams](http://storage.googleapis.com/books/ngrams/books/datasetsv2.html)

In computational linguistics, [n-grams](https://en.wikipedia.org/wiki/N-gram) are _n_ letter fragments (where _n_ > 1) of a word. These n-grams consist of letter that are adjacent to one another in the word, can co-occur across words, and occur at a certain frequency in a collection of words (or vocabulary). Due to linguistic redundancy, some n-grams (such as "ary") is quite common across a large number of words. 

For example, the word "ostentatious" can be broken down into -- n-grams. This approach is similar to "bag of words" approaches used in NLP, except that n-grams (transformed into syllabic nodes) will be mapped to a CGS space. 

The transformation of n-grams into syllabic nodes allows us to construct a network that traces between n-grams to form existing words. If we consider a vocabulary of 10<sup>4</sup> words, we can use string decomposition to derive a large number of n-grams and a large network of possible connections between n-grams. This further allows us to construct new words using the linguistic rules of the sampled language but not included in the original vocabulary. Complete words form a distionary that is then classified by the CGS kernel. Some notes on implementation (for a genetic algortihmic approach):

* use a fitness function independent of word length (treat n-grams of equal length and n-grams of unequal length as special cases).

* represent the fitness function as either a [Levenshtein distance](https://en.wikipedia.org/wiki/Levenshtein_distance) or with [K-L divergence](https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence).

* a good strategy is to break the full problem into subproblems so that you solve locally but seek a global solution.

* schema and building blocks are workable tools.

* there is a tradeoff between mutation rate and fiding a global solution. When the mutation rate is too high, you can escape local maxima but also eascape global maximum.

* evolutionary optimiztion as a tree. 
