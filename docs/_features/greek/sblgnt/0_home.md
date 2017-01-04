---
title: Dataset sblgnt
feat: false
---

# About

Greek New Testament Dataset, treebanks with full text, compiled by
Randall Tan, Jonathan Robie, and 
Andi Wu as part of the [biblicalhumanities group](https://github.com/biblicalhumanities). The source materials, documentation and licence conditions can be found
at the
[SBLGNT treebanks](https://github.com/biblicalhumanities/greek-new-testament/tree/master/syntax-trees/sblgnt)
github repo.

The conversion of this dataset to
[Text-Fabric](/ETCBC/text-fabric/wiki)
has been carried out by Cody Kingham and Dirk Roorda.
The source has been taken on 2017-01-03
(commit [1b4242c1ac6ae3012b751d00f735556710a0d21a](https://github.com/biblicalhumanities/greek-new-testament/commit/1b4242c1ac6ae3012b751d00f735556710a0d21a))

The conversion has preserved all information present in the `<Node>`-elements of the treebanks.
All attributes have been faithfully translated to individual Text-Fabric features.
The attribute `Cat` has been used, together with the fact whether a `<Node>` appears as root or as leaf,
to determine an object type, such as *sentence*, *clause*, *phrase*, *word*.

The result has 137794 word nodes (*slots*), and 428430 nodes in total.

We have added the names of the input files as book names and destilled the book, chapter, verse information
that is present in each `<node>` identifier into Text-Fabric node types `book`, `chapter`, `verse`, with
features that give their sequence numbers. 

We have added some statistical features: frequencies and ranks of word occurrences and lexemes.

The input xml representation consists of 27 files with a collective size of 64 MB.

The converted Text-Fabric resource consists of 34 files with a collective size of 31 MB.

# License

This work is licensed under a
[Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).
That means:

* You may download the data and use it: process, copy, modify;
* You may use the data to create new software applications;
* You may use the data for research and publish any amount of results;
* When you publish this data or results you obtained from them, you have to comply with the following:
  * give proper attribution to the data when you use it in new applications,
    by citing
    [SBLGNT treebanks](https://github.com/biblicalhumanities/greek-new-testament/tree/master/syntax-trees/sblgnt)
  * If you remix, transform, or build upon the material, you must distribute your contributions under this same license.

# How to use

This data can be processed by 
[Text-Fabric](https://github.com/ETCBC/text-fabric/wiki).
