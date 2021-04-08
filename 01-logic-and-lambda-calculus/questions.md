## Questions

#### Extending the grammar
The confusion was triggered by the two statements _'no man gives a bone to __a__ dog'_ and _'no man gives a bone to __the__ dog'_. 
Two members of the group believed that "the dog" means "exactly one [known] dog" [[1]](https://doi.org/10.1007/BF01052730), therefore, the grammar of "the" would be : `Det[NUM=sg, SEM=<\P Q. exists x.(P(x) & all y.(P(y) -> x=y) & Q(x)) >] -> 'the'`.
Whereas the two other members believed that "the dog" that there is a specific dog that no man gives a bone to, but it is still possible that no man gives a bone to another dog as well. Therefore, they believe that the grammar of 'the' and 'a' should be the same. i.e., `Det[SEM=<\P Q.exists x.(P(x) & Q(x))>] -> 'a' | 'the'
`.


In addition, for the statements 3, 4 and 5, we get the answer without β-reduction, in other words, λx and λQ are included and the statement is not simplified. We don't know what exactly is causing it and how it can be fixed.

## Alternative Solutions

#### Predicate logic without quantifiers
The statement: _"Lydia likes herself and so does George"_ has two different interpretations, thus two possible solutions.
We decided to interpret it as `like(Lydia,Lydia) ∧ like(George,George)` but another possible solution is `like(Lydia,Lydia) ∧ like(George,George)`.

#### First order logic with quantifiers
Similarly, the statement _"Exactly one musician plays everything Alex wrote"_ has two possible solutions as it doesn't specify whether the musican plays what Alex wrote exclusively or can play other pieces as well.
Therefore, we decided to go with the latter `∃x. ∀y. (write(Alex, y) ∧ musician(x) → play(x, y)) ∧ (∀z. ∀y. (write(Alex, y) ∧ musician(z) → play(z, y)) → x=z)` where another possible solution can also be `∃x. ∀y. (write(Alex, y) ∧ musician(x) ∧ play(x, y)) ∧ (∀z. ∀y. (write(Alex, y) ∧ musician(z) ∧ play(z, y)) → x=z)`




## References
[1] Ludlow, P. (1995). The logical form of determiners. Journal of Philosophical Logic, 24(1), 47-69.
[2] Partee, B. (2005). Lecture 2 . Lambda abstraction , NP semantics , and a Fragment of English. MGU.

