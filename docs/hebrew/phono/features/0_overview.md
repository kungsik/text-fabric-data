# Phono module

The **phono** module provides two features, `phono` and `phono_trailer`.

They are defined for all word occurrences.

They have been constructed by means of the  
[phono notebook](https://rawgit.com/ETCBC/text-fabric/master/phono/phonoTf.html)
which shows and documents the way this representation has been obtained.

This module also provides a text representation to text-fabric.
See the [otext@phono](/ETCBC/text-fabric-data/hebrew/phono/otext@phono.tf) file.

When this module is loaded into Text-Fabric, you can get text in phonetic representation
by calling

```python
T.text(nodes, fmt='text-phono-full')
```

# Features

## phono
Contains a phonetic representatiton of a word.
Although it gives the phonetics per word,
its computation has been dependent on the immediate context and even on the wider context of the corpus as a whole.

This is because the know grammatical rules to arrive at the proper pronunciation of Biblical Hebrew
are insufficient and inconsistent.
Many of the problems could be resolved by looking at other occurrences of the same word in the corpus.

It is very well possible that there the phono feature exhibits faulty values.
Feedback is welcome:
[shebanq](mailto:shebanq@ancient-data.org)

## phono_trailer
Contains a representation of the material that follows a word.
