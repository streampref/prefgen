# Table of Contents

- [Introduction](#introduction)
- [Command Line](#command-line)

# Introduction

PrefGen is a dataset generator with conditional preferences for [StreamPref](http://streampref.github.io) DSMS prototype.
PrefGen generates the relations, queries and auxiliary files for the execution of experiments with StreamPref.
The experiments parameters must be updated directly in the source code.
The parameters are the following:
- __ATT__: Number of attributes;
  - __ATTRIBUTE_LIST__: List with variation on parameter __ATT__;
  - __ATTRIBUTE_DEFAULT__: Default value for parameter __ATT__; 
- __TUP__: Number of initial tuples;
  - __TUPLE_LIST__: List with variation on parameter __ATT__;
  - __TUPLE_DEFAULT__: Default value for parameter __ATT__; 
- __DEL__: Number of deletions per instant;
  - __DELETION_LIST__: List with variation on parameter __ATT__;
  - __DELETION_DEFAULT__: Default value for parameter __ATT__; 
- __INS__: Number of insertions per instant;
  - __INSERTION_LIST__: List with variation on parameter __ATT__;
  - __INSERTION_DEFAULT__: Default value for parameter __ATT__; 
- __RUL__: Number of rules;
  - __RULE_LIST__: List with variation on parameter __ATT__;
  - __RULE_DEFAULT__: Default value for parameter __ATT__; 
- __LEV__: Maximum preference level;
  - __LEVEL_LIST__: List with variation on parameter __ATT__;
  - __LEVEL_DEFAULT__: Default value for parameter __ATT__; 
- __IND__: Number of indifferent attributes;
  - __INDIFF_LIST__: List with variation on parameter __ATT__;
  - __INDIFF_DEFAULT__: Default value for parameter __ATT__; 
- __TOP__: Number of top-k tuples to be returned.
  - __TOPK_LIST__: List with variation on parameter __ATT__;
  - __TOPK_DEFAULT__: Default value for parameter __ATT__; 

The relations are composed of integer attributes.
At every instant, __INS__ tuples are inserted and __DEL__ tuples are deleted.
The number of iterations are controlled by the variable __ITERATION_DEFAULT__.
Please see the related publications for more information.

# Command Line

```
prefgen.py [-h] [-g] [-r] [-s]:
    -h/--help: display help message
    -g/--gen: Generate files
    -r/--run: Run experiments
    -s/--summarize: Summarize experiments results
```
