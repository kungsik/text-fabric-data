# rank_lex

**rank-lexeme**

The rank of a lexeme, a measure related to its frequency.

This feature is present on objects of type *word*.

The rank of an item is the number of items that have a higher frequency.
So items with rank 0 have the highest frequency.
If two or more items have identical frequency, they have the same rank, but the rank immediately below is not one lower, but *n* lower,
where *n* is the amount of items with that same frequency.

**NB:**
The ETCBC lexicon makes distinctions between homonyms, i.e. distinct lexemes that are spelled identically.
This feature respects that distinction.

**Hint:**
The measures *frequency* and *rank* have been computed for *lexemes* and *occurrences*.
    
This feature has been added to the database in a later stage as package called `lexicon`.

You can use it in SHEBANQ queries.

If you want to use it in LAF-Fabric, you have to load `lexicon` as *annox*.
Consult the [LAF-Fabric API reference on annoxes](http://laf-fabric.readthedocs.io/en/latest/texts/API-reference.html#extra-annotation-packages).

See also:
 
* [freq_lex](freq_lex)
* [rank_lex](rank_lex)
* [freq_occ](freq_occ)
* [rank_occ](rank_occ)

