---
title: Phono features
feat: false
---

The **phono** module provides two features, 
[phono](phono) and 
[phono_trailer](phono_trailer).

They are defined for all word occurrences.

They have been constructed by means of the  
[phono notebook](https://rawgit.com/ETCBC/text-fabric/master/phono/phonoTf.html)
where you can find documentation on the way this representation has been obtained.

This module also provides a text representation to Text-Fabric.
See the [otext@phono](/ETCBC/text-fabric-data/hebrew/phono/otext@phono.tf) file.

When this module is loaded into Text-Fabric, you can get text in phonetic representation
as follows

```python
T.text(nodes, fmt='text-phono-full')
```

