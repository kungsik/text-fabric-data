---
title: rela
---

**relation**


The linguistic relation between the object and its context.

This feature is present on objects of type [*clause*, *phrase(_atom)*, and *subphrase*](otype).

# Subphrase


---|---|---
`ADJ`|`adj`|Adjunct
`ATR`|`atr`|Attribute
`DEM`|`dem`|Demonstrative
`MOD`|`mod`|Modifier
`PAR`|`par`|Parallel
`REG`|`rec`|Regens

The kind of relationship between the object (daughter) and its mother.
In case of the regens/rectum relation, the mother is not a subphrase, but a word.
The upper case values apply to the mother subphrase and the lower case values apply to the daughter subphrase.
See [mother](mother).

##### Note
> In MQL the feature applies to the *daughter* only; the mother has the value `NA`.

##### Note
> Consider leaving out the uppercase values, since they do not occur in MQL.
Examples needed.

Explain why is this a useful feature. Examples needed.

# Phrase_atom


---|---
`Appo`|Apposition
`Sfxs`|Suffix specification
`Link`|Conjunction
`Spec`|Specification
`Para`|Parallel

This feature expresses the way a phrase atom is used in building a complex phrase.

##### Note
> I prefer a more informative definition.

Explain why is this a useful feature? Examples needed.


# Phrase


---|---
`PrAd`|Predicative adjunct
`Resu`|Resumption

This feature expresses how phrases refer to each other.
The value for *rela* has been derived from the value of phrase [function](function) of the daughter
(`PrAd` yields `PrAd`)
or the mother (`Frnt` yields `Resu`).
See [mother](mother).
The mother of a resumption can be a clause, namely when the constituent in question resumes a casus pendens clause.

##### Note
> The remarks about `PrAd`, `Frnt` and `Resu` are too terse to be understood.
Is the object in question (the one carrying the *rela* feature), the mother or the daughter?

I prefer a more informative definition.

Explain why is this a useful feature? Examples needed.

# Clause


---|---
`Adju`|Adjunctive clause
`Attr`|Attributive clause
`Cmpl`|Complement clause
`Coor`|Coordinated clause
`Objc`|Object clause
`PrAd`|Predicative adjunct clause
`PreC`|Predicative complement clause
`ReVo`|Referral to the vocative
`Resu`|Resumptive clause
`RgRc`|Regens/rectum connection
`Spec`|Specification clause
`Subj`|Subject clause

For *clause*-like objects this feature is also called *clause constituent relation*;
it indicates the syntactic function of the clause.

## Example
I will use Gen 20:1 and Gen 20:7 as an example since it is an easy text. Basically, there are two different levels of clause relations:
### 1. Syntactical relation
**A.** Syntactical relations have to be specified at the moment where a dependent clause (daughter) is encountered. If there is a dependent clause found two questions have to be answered. These dependent clauses are usually detectable on the basis of the clause initiative conjunction (like KJ, >CR, etc.).
![alt text] (https://ydmp2g-dm2305.files.1drv.com/y3m7ofpTlo91bJpxtFSb-IB4CtfBtCFswYEerkGleOJZK5YgjOJocTZcHEuSR6DYZrjtb0k9Ng_QPLG64ttSDYXVF9p2_uBc0BfZA5luvNGeFf1rBltDQHdbeY3-6DHew7JGHUiPJN0roYtM2RN1ltKvZofoQOc6-QL2mWeYfLydKk/Gen20_07_ctt.png?psid=1 "Gen 20:7 ctt snapshot")
**A.i.** What type of relational nature the dependent clause has (e.g. attributive, adjunct, object, etc.) can be found under the feature `rela` or column 2.55 in the QDF files.  

**A.ii.** What mother clause a dependent clause has (mother-daughter relation) and where this mother clause is can be identified in column 2.51/2.52 and 2.56/2.57 in the QDF file or with the help of the features `dist_unit`, `dist`, and `mother_object_type` in a MQL query.
In case of ClA-no36/1838 the objective clause atom “that you will surely die” has as its mother ClA-no35/1837. How do we know that? If you go to 2.57 it will tell you that the distance to that mother is measured by ClA-nos. In 2.56 it says that you have to go -1 unit (of ClA-nos) backward (that’s why it is “-“). This will bring you to ClA-no35/1837.
In case of the attributive ClA-no37/1839 2.57 tells you that the distance to the mother is measured by the Word#s. In 2.56 it says that you have to go -2 units (of Word-nos) backward. Since the last word of ClA-no37 is Word-no9398 we arrive at Word-no9396 which is part of the ClA-no36/no1838. The distance of attributive clause atoms is usually measured by words# or phrase_atom# so that one can be very specific about the participant the attributive clause is referred to. 2.52 clarifies the functional role of any clause (if it relates functionally to other clauses). Therefore, ClA-no1839 receives the code 10. The first digit “1” stands for the conjunction >CR while the second digit “0” says that the clause_atom does not contain a tense word. ClA-no1838 is a postulational clause since it receives the code 513. Again, the first digit tells us something about the conjunction class to which KJ belongs, the second digit informs us about the tense of the daughter (imperfect) and the third digit tells us about the tense of the mother clause (imperative). 2.51 counts the number of ClAs it has to go back in order to find the mother clause. Thus, the numbers of 2.51 and 2.56+57 should always lead to the same mother clause.
![alt text] (https://ydms2g-dm2305.files.1drv.com/y3mmQffj6X729AmiRE8dsOIeU1Z12403-XY95UeDnIJ7Ur6eaYxosaCZSocLlKZ6OZiOqe1Uo1RuwvxAiBGp-bxanGKXvZrr2kOVEmQ5sn_b7_0RSl-JZj4rV2o7Pww6BjrNyw2bkIDW-v_Qt_8iTVRx6d2fhZacaypQemG1AeW2xw/Gen20_07_qdf.png?psid=1 "Gen 20:7 qdf snapshot") 
**B.** In addition to the necessary syntactical relation between independent and dependent clause we have also syntactical relation between two independent clauses since on a functional level (motive, conditional, parallel, final, etc.) the relate to each other.
![alt text] (https://ydmb2g-dm2305.files.1drv.com/y3mJVYGg9o6nb1EQOrQs32Az_r8G5QY42eDyQOAGlnykwQ3VdVX3e_bviNwcLGTOYG5J-RDRwxCqFax3PcuLa7q17UEmOsR4vOWALJ-ZUMw9YzGwWx-G3wE7A1XCPPtVQMJC-aTpa7FX8M3hg_Tfeb10zrCUHIzbjhFjzavPsDVGqA/Gen20_07_ctt_no2.png?psid=1 "Gen 20:7 ctt snapshot") 
As we see above, with ClA-no34 we have a condtional clause (no30 “return the woman…” => no34 “if you don’t return her”). In 2.52 you find the information for these functional clause relation. The code provided in this particular case is 663. The first digit tells you that the initial conjunction >M belongs to the conjunction group 600. The second digit tells you that clause #34 contains a participle tense (6). The third digit tells you that the mother clause contains an imperative tense (3). How do we know where the mother is? While we know who the mother is (it must be an imperative clause), we do not yet know where it is. Here we have to go to QDF column2.51 where we are informed to go back -4 ClA-nos.
![alt text] (https://ynmu2g-dm2305.files.1drv.com/y3m7TY5J5d32TDdC8HGTLX_qan_xHDFhYvTy1gP5EH8Li70yW0IkBqq2v4Ix2Wl1ObEMwrUbVFPQtfpSFsP-8IPSg-jViIWyg-9upTp0nP4SZYdKwSs_Q5Dr5gdoRC6Q8-vWb0zO4iF7SqlQ2ADhmeSvn6BYJRr_mVqu5_EseSxpkk/Gen20_07_qdf_no2.png?psid=1 "Gen 20:7 qdf snapshot") 
**C.** All the information needed in order to calculate clause_atom relations, i.e. syntactical relations, can be found in columns 2.51-2.57 in the QDF file and can be calculated by means of the features `dist_unit`, `dist`, and `mother_object_type` in an MQL query. The following SHEBANQ/MQL query searches for all cases in which God is characterized by means of an attributive clause
```
select all objects where
[sentence  
	[  
	[clause FOCUS   
		[clause as motherClause  
			[word lex = 'JHWH/' or lex = '>LHJM/' or lex = '>L/']  
		]  
	]  
	..  
	[clause FOCUS rela = Attr AND mother = motherClause.self]  
	]  
	OR  
	[  
	[clause FOCUS     
		[clause as motherClauseG  
			[word lex = 'JHWH/' or lex = '>LHJM/' or lex = '>L/']  
		]  
	]  
	..  
	[gap   
		[clause FOCUS rela = Attr AND mother = motherClauseG.self]  
	]  
	]  
]  
OR  
[sentence  
	[  
	[clause  
		[phrase FOCUS  
			[phrase as motherPhrase  
				[word lex = 'JHWH/' or lex = '>LHJM/' or lex = '>L/']  
			]  
		]  
	]  
	..  
	[clause FOCUS rela = Attr AND mother = motherPhrase.self]  
	]  
	OR  
	[  
	[clause  
		[phrase FOCUS  
			[phrase as motherPhraseG  
				[word lex = 'JHWH/' or lex = '>LHJM/' or lex = '>L/']  
			]  
		]  
	]  
	..  
	[gap  
		[clause FOCUS rela = Attr AND mother = motherPhraseG.self]  
	]  
	]  
]  
OR  
[sentence  
	[  
	[clause   
		[word FOCUS  
			[word as motherWord  
				[word lex = 'JHWH/' or lex = '>LHJM/' or lex = '>L/']  
			]  
		]  
	]  
	..  
	[clause FOCUS rela = Attr AND mother = motherWord.self]  
	]  
	OR  
	[  
	[clause 
		[word FOCUS  
			[word as motherWordG  
				[word lex = 'JHWH/' or lex = '>LHJM/' or lex = '>L/']  
			]  
		]  
	]  
	..  
	[gap  
		[clause FOCUS rela = Attr AND mother = motherWordG.self]  
	]  
	]  
] 
```
See this query (with results) on [SHEBANQ](https://shebanq.ancient-data.org/hebrew/query?version=4b&id=1504).
Note that the data version used on SHEBANQ is **4b**, while this documentation is for version **4c**.  

### 2. Text-grammatical relations
**A.** Text-grammar does not clarify the grammatical structure of a clause or how an independent clause relates to a dependent clause etc.. Text-grammar explores how all clauses of a given text relate on a textual instead of on clausal level. E.g. whether a clause is narrative or discursive and whether a WayX clause is part of the main line of narration or delivering just some narrative background information for the main line narration are questions dealt with in Text-grammar. The ETCBC provides columns in the QDF file that suggest the grammar of the text, that is the texture of the text on the basis of formal criteria (so it is not based upon subjective literary analysis). 
![alt text] (https://ynmt2g-dm2305.files.1drv.com/y3mXFJG45D1CG5PgsDra7DxLBKkbnWseylib_QbPkWBeGBWm0VzSAtSmC0QpTFX_sP1MFJaygTIUb1E-KBOe1_-BxVs4yOAcU9EaD5fmpV5TUBl8iu-d9qtpzemQmT2QVFNfo7rdwmxrGOv8WGVMTh7V4Mt9OdbC6huf9KoovoevUQ/Gen20_01_ctt_no2.png?psid=1 "Gen 20:1 ctt snapshot") 
**B.** QDF column 2.61 is a good start as it clarifies whether a clause is text-hierarchically embedded in another clause (NQ means that we have a clause that belongs to a direct speech (Q) that itself is imbedded in a narration (N); NQQ would be a direct speech clause embedded in another direct speech clause that itself is part of a narration (e.g.: Tom went to school and he said to Steven: “Mum told me: “don’t be late!””).
**C.** From a text-grammatical perspective the first clause of a chapter (here the mediaeval chapter divisions are often problematic) is always the mother of the text and therefore on the 0 position of indentations (cf. ClA-no1). This is, however, the mother on the textual level not on a clause-syntactical level. It is not possible that any following clause pushes the first clause from its 0 position (except the first clause is in casus pendens). What is possible is that new clauses can move to the 0 level when certain formal criteria are fulfilled. E.g. ClA-no4 is also a WayX clause with the same subject (Abraham) and is therefore has the same text-grammatical characteristics as ClA-no1. It thus is put in parallel by bringing the indentation to the 0 line. QDF column 2.58 delivers the information of the indentation for each clause_atom. If you follow the indentation (see CTT files) you will get a clear picture of the text-grammatical structure of the text. QDF column 2.51 and 2.52 gives you the information about the location and the nature of the mother clause and of what nature the daughter clause is. QDF column 2.51-52 are already know from the syntax level. But now the syntax information is combined with columns 2.58 and 2.61 in order to develop a complete textual hierarchy.
![alt text] (https://ydmc2g-dm2305.files.1drv.com/y3mCiBBMU6EiZGesbeAJVnoMLkesuHUAFJxVMVNc9XuHkdg_82X8tu1OfaeKaQ3T2FRK1W0Sx_U4KqlB7KDKhIZ-SQSnjCPcZYDr5OywtEoZJAl-FTtpjfNyHkAzbzIvOPMXGyRXyXsqR_869MR6B0NVre-Dzg6LPJRJdMoCgM9Qzw/Gen20_01_qdf.png?psid=1 "Gen 20:1 ctt snapshot") 
**D.** The following SHEBANQ/MQL query searches for all cases in which a speaker is repeatedly referred to in two subsequent narrative speech intorductions (e.g. "And Abimelech [speaker] spoke to Abraham") despite the fact that the addressee did not respond (e.g. "And Abraham answered" would be missing): 
See this query (with results) on [SHEBANQ](https://shebanq.ancient-data.org/hebrew/query?version=4b&id=491).
Note that the data version used on SHEBANQ is **4b**, while this documentation is for version **4c**.


##### Note
> I prefer a more informative definition.

Explain why is this a useful feature? Examples needed.

