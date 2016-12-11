# rela

**relation**


The linguistic relation between the object and its context.

This feature is present on objects of type *clause*, *phrase(_atom)*, and *subphrase*.

## Subphrase


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

**NB:**
In MQL the feature applies to the *daughter* only; the mother has the value `NA`.

**NB:**
Consider leaving out the uppercase values, since they do not occur in MQL.
Examples needed.

Explain why is this a useful feature. Examples needed.

## Phrase_atom


---|---
`Appo`|Apposition
`Sfxs`|Suffix specification
`Link`|Conjunction
`Spec`|Specification
`Para`|Parallel

This feature expresses the way a phrase atom is used in building a complex phrase.

**NB:**
I prefer a more informative definition.

Explain why is this a useful feature? Examples needed.


## Phrase


---|---
`PrAd`|Predicative adjunct
`Resu`|Resumption

This feature expresses how phrases refer to each other.
The value for *rela* has been derived from the value of phrase [function](function) of the daughter
(`PrAd` yields `PrAd`)
or the mother (`Frnt` yields `Resu`).
See [mother](mother).
The mother of a resumption can be a clause, namely when the constituent in question resumes a casus pendens clause.

**NB:**
The remarks about `PrAd`, `Frnt` and `Resu` are too terse to be understood.
Is the object in question (the one carrying the *rela* feature), the mother or the daughter?

I prefer a more informative definition.

Explain why is this a useful feature? Examples needed.

## Clause


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

**NB:**
I prefer a more informative definition.

Explain why is this a useful feature? Examples needed.

