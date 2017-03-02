---
title: Dataset extrabiblical
feat: false
---

# About

Extra biblical text material, coded by Janet Dyk, Martijn Naaijer at the
[Eep Talstra Centre for Bible and Computer](http://www.godgeleerdheid.vu.nl/en/research/institutes-and-centres/eep-talstra-centre-for-bible-and-computer/index.aspx),
for the 
[SYNVAR project](http://www.nwo.nl/en/research-and-results/research-projects/i/30/9930.html),
exported to MQL by Constantijn Sikkel and then to
[Text-Fabric](https://github.com/ETCBC/text-fabric/wiki).
by Dirk Roorda
[Data Archiving and Networked Services](https://dans.knaw.nl/en/front-page?set_language=en).

The conversion from MQL to TF has been done by
[tfFromMql](https://github.com/ETCBC/text-fabric/blob/master/exercises/tfFromMql.py).

# License

This work is licensed under a
[Attribution-NonCommercial 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
That means:

* You may download the data and use it: process, copy, modify;
* You may use the data to create new software applications;
* You may use the data for research and publish any amount of results;
* When you publish this data or results you obtained from them, you have to comply with the following:
  * give proper attribution to the data when you use it in new applications,
    by citing this persistent identifier:
    [10.17026/dans-z6y-skyh](http://dx.doi.org/10.17026%2Fdans-z6y-skyh).
  * when you have modified the data, indicate the changes without 
    claiming that the ETCBC has endorsed the modifications.

# Contents

This dataset contains the following writings:

* 1QM
* 1QS
* Ajrud
* Arad
* Balaam
* Ketef Hinnom
* Lachish
* Mesha
* Mesad Hashavyahu
* Siloam

# How to use

This data can be processed by 
[Text-Fabric](https://github.com/ETCBC/text-fabric/wiki), see this
[extra tutorial](https://github.com/ETCBC/text-fabric/blob/master/exercises/ExtraBiblical.ipynb)
to get started.

# Features

This data contains some but not all of the linguistic features documented for the
[etcbc4c dataset of the Hebrew Bible](https://etcbc.github.io/text-fabric-data/features/hebrew/etcbc4c/0_overview.html).
There are little deviations in the contents though.
Using Text-Fabric, it is easy to explore the details, e.g. with `F.`*feature*.`freqList()`.

See also 
[tutorial (Hebrew)](https://github.com/etcbc/text-fabric/blob/master/docs/tutorial.ipynb)
and
[tutorial (search)](https://github.com/etcbc/text-fabric/blob/master/docs/searchTutorial.ipynb).
