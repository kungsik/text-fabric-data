---
title: Strong features
feat: false
---

The **strong** module provides one feature, [strong](strong).

They are defined for all word occurrences.

They have been constructed by means of the  
[strong notebook](https://github.com/ETCBC/text-fabric/blob/master/Versions/strong.ipynb).
where you can find documentation on the way this representation has been obtained.

This module also provides a text representation to Text-Fabric.
See the [otext@strong](/ETCBC/text-fabric-data/hebrew/strong/4c/otext@strong.tf) file.

When this module is loaded into Text-Fabric, you can get text in strong representation
as follows

```python
T.text(nodes, fmt='lex-strong-full')
```