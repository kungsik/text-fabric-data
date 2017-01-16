---
title: Strong features
feat: false
---

The **strong** module provides one feature, [strong](strong).

It is defined for word occurrences.

It has been constructed by means of the  
[strong notebook](https://github.com/ETCBC/text-fabric/blob/master/Versions/strong.ipynb),
where you can find documentation on the way the Strongs have been obtained.

This module also provides a new text representation to Text-Fabric
(see the [otext@strong](/ETCBC/text-fabric-data/hebrew/strong/4c/otext@strong.tf) file).
When this module is loaded into Text-Fabric, you can get text in strong representation
as follows

# Discussion

It is not easy to connect Strong numbers to the ETCBC dataset.
For an overview of factors that affect the consistency of the assignment of Strong numbers
to ETCBC lexemes, see
[Stephen Ku's remarks](https://docs.google.com/document/d/1VawfTAi-b_NV4Ullxy0d2HrMiIOdkNdaxxx7q8Lrvy8/edit?usp=sharing)
(work in progress).

For a discussion on Strong numbers in general, see
[A New Numbering System for Greek New Testament Lexemes](https://www.academia.edu/19660777/A_New_Numbering_System_for_Greek_New_Testament_Lexemes_2006_)
by James Tauber and Ulrik Sandborg-Petersen.

```python
T.text(nodes, fmt='lex-strong-plain')
```
