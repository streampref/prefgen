**Table of Contents**

- [Introduction](#introduction)
- [Command Line](#command-line)

# Introduction

PrefGen is a dataset generator with conditional preferences for [StreamPref](http://streampref.github.io) DSMS prototype.
PrefGen generates the relations, queries and auxiliary files for the execution of experiments with StreamPref.
The experiments parameters must be updated directly in the source code.
The parameters are the following:
- **ATT**: Number of attributes;
  - **ATTRIBUTE_LIST**: List with variation on parameter **ATT**;
  - **ATTRIBUTE_DEFAULT**: Default value for parameter **ATT**; 
- **TUP**: Number of initial tuples;
  - **TUPLE_LIST**: List with variation on parameter **ATT**;
  - **TUPLE_DEFAULT**: Default value for parameter **ATT**; 
- **DEL**: Number of deletions per instant;
  - **DELETION_LIST**: List with variation on parameter **ATT**;
  - **DELETION_DEFAULT**: Default value for parameter **ATT**; 
- **INS**: Number of insertions per instant;
  - **INSERTION_LIST**: List with variation on parameter **ATT**;
  - **INSERTION_DEFAULT**: Default value for parameter **ATT**; 
- **RUL**: Number of rules;
  - **RULE_LIST**: List with variation on parameter **ATT**;
  - **RULE_DEFAULT**: Default value for parameter **ATT**; 
- **LEV**: Maximum preference level;
  - **LEVEL_LIST**: List with variation on parameter **ATT**;
  - **LEVEL_DEFAULT**: Default value for parameter **ATT**; 
- **IND**: Number of indifferent attributes;
  - **INDIFF_LIST**: List with variation on parameter **ATT**;
  - **INDIFF_DEFAULT**: Default value for parameter **ATT**; 
- **TOP**: Number of top-k tuples to be returned.
  - **TOPK_LIST**: List with variation on parameter **ATT**;
  - **TOPK_DEFAULT**: Default value for parameter **ATT**; 

The relations are composed of integer attributes.
At every instant, **INS** tuples are inserted and **DEL** tuples are deleted.
The number of iterations are controlled by the variable **ITERATION_DEFAULT**.


# Command Line

- -g/--gen: Generate files
- -r/--run: Run experiments
- -s/--summarize: Summarize experiments results
