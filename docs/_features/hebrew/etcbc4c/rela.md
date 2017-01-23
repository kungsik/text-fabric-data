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
A. Syntactical relations have to be specified at the moment where a dependent clause (daughter) is encountered. If there is a dependent clause found two questions have to be answered. These dependent clauses are usually detectable on the basis of the clause initiative conjunction (like KJ, >CR, etc.).
![alt text] (https://ydmp2g-dm2305.files.1drv.com/y3mgujV7W56q51jnJ8NaW-lhtajQjXpHM_alnoZCUYuRNlUC06RcjrK7I7e0Yut9PigaSvQ3WnN3MbSWH0i3rMYfY67DwPSjC-Y4aqhezpDQqvxbqGGPXw765EfTHALX0OM2Nbm9v0Dfci6WpqcEjTywT2lJJdGCShnJHqZVcFWrEg/Gen20_07_ctt.png?psid=1 "Gen 20:7 ctt snapshot")
A.i. What type of relational nature the dependent clause has (e.g. attributive, adjunct, object, etc.) can be found under the feature `rela` or column 2.55 in the QDF files.  

A.ii. What mother clause a dependent clause has (mother-daughter relation) and where this mother clause is can be identified in column 2.51/2.52 and 2.56/2.57 in the QDF file or with the help of the features `dist_unit`, `dist`, and `mother_object_type` in an MQL query.
In case of ClA-no36/1838 the objective clause atom “that you will surely die” has as its mother ClA-no35/1837. How do we know that? If you go to 2.57 it will tell you that the distance to that mother is measured by ClA-nos. In 2.56 it says that you have to go -1 unit (of ClA-nos) backward (that’s why it is “-“). This will bring you to ClA-no35/1837.
In case of the attributive ClA-no37/1839 2.57 tells you that the distance to the mother is measured by the Word#s. In 2.56 it says that you have to go -2 units (of Word-nos) backward. Since the last word of ClA-no37 is Word-no9398 we arrive at Word-no9396 which is part of the ClA-no36/no1838. The distance of attributive clause atoms is usually measured by words# or phrase_atom# so that one can be very specific about the participant the attributive clause is referred to. 2.52 clarifies the functional role of any clause (if it relates functionally to other clauses). Therefore, ClA-no1839 receives the code 10. The first digit “1” stands for the conjunction >CR while the second digit “0” says that the clause_atom does not contain a tense word. ClA-no1838 is a postulational clause since it receives the code 513. Again, the first digit tells us something about the conjunction class to which KJ belongs, the second digit informs us about the tense of the daughter (imperfect) and the third digit tells us about the tense of the mother clause (imperative). 2.51 counts the number of ClAs it has to go back in order to find the mother clause. Thus, the numbers of 2.51 and 2.56+57 should always lead to the same mother clause.
![alt text] (https://1drv.ms/i/s!Al0u8U0ZQlv3hJg6iXOX1GjwqAHSKQ "Gen 20:7 qdf snapshot") 
B. In addition to the necessary syntactical relation between independent and dependent clause we have also syntactical relation between two independent clauses since on a functional level (motive, conditional, parallel, final, etc.) the relate to each other. E.g. with ClA-no34 we have a condtional clause (no30 “return the woman…” => no34 “if you don’t return her”). In 2.52 you find the information for these functional clause relation. The code provided in this particular case is 663. The first digit tells you that the initial conjunction >M belongs to the conjunction group 600. The second digit tells you that clause no34 contains a participle tense (6). The third digit tells you that the mother clause contains the an imperative tense (3). How do we know where the mother is? We know who the mother is (it must be an imperative clause). But we do not yet know where it is. Here we have to go to 2.51 where we are informed to go back -4 ClAs.
C. All the information needed in order to calculate clause_atom relations, i.e. syntactical relations, can be found in 2.51-2.57.

### 2. Text-grammatical relations

##### Note
> I prefer a more informative definition.

Explain why is this a useful feature? Examples needed.

