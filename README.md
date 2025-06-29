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

