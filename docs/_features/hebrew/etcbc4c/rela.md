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
1.a. Syntactical relations have to be specified at the moment where a dependent clause (daughter) is encountered. If there is a dependent clause found two questions have to be answered. These dependent clauses are usually detectable on the basis of the clause initiative conjunction (like KJ, >CR, etc.).
![alt text] (https://ydmp2g-dm2305.files.1drv.com/y3mgujV7W56q51jnJ8NaW-lhtajQjXpHM_alnoZCUYuRNlUC06RcjrK7I7e0Yut9PigaSvQ3WnN3MbSWH0i3rMYfY67DwPSjC-Y4aqhezpDQqvxbqGGPXw765EfTHALX0OM2Nbm9v0Dfci6WpqcEjTywT2lJJdGCShnJHqZVcFWrEg/Gen20_07_ctt.png?psid=1 "Gen 20:7 ctt snapshot")
What type of relational nature the dependent clause has (e.g. attributive, adjunct, object, etc.) can be found under the feature `rela` or column 2.55 in the QDF files.
### 2. Text-grammatical relations

##### Note
> I prefer a more informative definition.

Explain why is this a useful feature? Examples needed.

