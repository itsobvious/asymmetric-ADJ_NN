# asymmetric-ADJ_NN

This repository contains data samples for the study described in [1]. The adjective-noun pairs stem from in a number of German tree banks: Wikipedia 2017 and Wikipedia 2018 [2] and
decow16ax [3], [4].

File "asymmetry-topP1.txt" contains 600 adjective-noun pairs with high deltaP1 values. File "asymmetry-topP2.txt" contains 600 adjective-noun pairs with high deltaP2 values. The structure of the files is as follows:

* column "phrase": adjective-noun pair
* column "raw_frequency": absolute frequency of the adjective-noun phrase in the underlying data 
* column "dp1": deltaP1 value 
* column "dp2": deltaP2 value 
* column "logDice": logDice value
* column "label": idiomatic status of the phrase (ne - named entity, term - technical term, free - free phrase, collocation - collocation, cliche - cliché) based on the classification descibed in [1]
* column "compound-nn": whether the noun in the pair is a compound (0 - no, 1 - yes)
* column "compound-adj": whether the adjective in the pair is a compound (0 - no, 1 - yes)

File "asymmetry-attributes" contains the same 1.200 pairs from the two files described above. The phases are additionally annotated with attributes (as defined in [1]). 

If you use this data, please, cite [1].

[1]  Strakatova, Yana (2025): Lexical-Semantic Modeling of Adjectve-Noun Co-occurrences. Ph.D. Dissertation. Tübingen

[2] Daniël de Kok and Sebastian Pütz. 2019. Stylebook for the Tübingen Treebank of Dependency-parsed German (TüBa-D/DP). Seminar für Sprachwissenschaft, Universität Tübingen, Tübingen, Germany.

[3] Roland Schäfer. 2015. Processing and querying large web corpora with the COW14 architecture. In Proceedings of Challenges in the Management of Large Corpora 3 (CMLC-3), Lancaster. UCREL, IDS.

[4] Roland Schäfer and Felix Bildhauer. 2012. Building large corpora from the web using a new efficient tool chain. In Proceedings of the Eight International Conference on Language Resources and Evaluation (LREC’12), pages 486–493, Istanbul, Turkey. European Language Resources Association (ELRA).
