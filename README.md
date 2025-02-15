# tag-lex
Corpus-based lexical statistics of Tagalog

## About
These lexical statistics of the Tagalog language are used by the Neuroscience of Language Lab in research on word processing in the mind/brain. This collection of resources includes:
- token ngram lists. Created with NLTK (Loper & Bird 2002)
- stem frequency lists
- morph frequency lists
- phonemic (graphemic) surprisal values: contains multiple values per word. A value representing surprisal/prediction error (see Hale 2001) is calculated for each phoneme in the word (using the formula from Gwilliams & Marantz 2015). Ngrams used as the input for this were created with SLRIM (Stolcke 2002)
- stem:whole word transition probability: contains one value per multimorphemic word  (see Lewis, Solomyak, and Marantz 2011)

## Format
Ngram lists are formatted into comma-separated columns as follows:

> ngram , frequency , /newline

Stem and morph frequency lists are formatted into comma-separated columns as follows:

> stem/morph , frequency , /newline

Surprisal lists are formatted into comma-separated columns as follows (with '...' representing repeated string and surprisal pairs throughout the word):

> word , grapheme string , surprisal , ... grapheme string , surprisal /newline

Stem:whole word transition probability (TP) is formatted as follows:

> word , frequency of stem , frequency of whole word , TP , /newline

## Data Sources
The corpus source was Tagalog Wikipedia, and is available thanks to the following:

Nathaniel Oco and Rachel Edita Roxas. 2012. Pattern Matching Refinements to Dictionary-based Code-switching Point Detection. In Proceedings of the 26th Pacific Asia Conference on Language, Information, and Computation (Bali, Indonesia. November 07-10, 2012). Published by the Faculty of Computer Science, Universitas Indonesia, pp 229-236. ISBN: 978-979-1421-17-1.

The tags used to determine part of speech in counting the morphs of the corpus were propagated from the tags in:

Manguilimotan, E. and Matsumoto, Y., 2011, December. Dependency-based Analysis for Tagalog Sentences. In Proceedings of the 25th Pacific Asia Conference on Language, Information and Computation (pp. 343-352).
