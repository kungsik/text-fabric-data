# Features (by category)

## Introduction
This is the key to the meaning of the features of the
[etcbc4c dataset](/ETCBC/hebrew/etcbc4c/home).

There are several
[types of objects](otype.md),
which specify what features such objects have.

We organize the object types as follows:

* [sectional](#sectional-features)
* [word](#word-features)
* [linguistic](#linguistic-features)

## Grid features

---|---|---
[otype](otype.md) | node type | `book` `verse` `clause` `phrase` `word`
[oslots](oslots.md) | slot containment | `1` `1-11` `2010-2015,2020-2030`
[otext](otext.md) | textapi | *no data, only specifications*  

## Sectional features

---|---|---
[book](book.md) | name of Bible book | `Genesis` `Psalmi` `Amos`
[chapter](chapter.md) | number if chapter within book | `3`
[verse](verse.md) | number of verse within chapter | `4`
[label](label.md) | passage indicator | `AMOS 03,04`
[half_verse](half_verse.md) | key for part within verse | `A` `B` `C`

## Word features

## Orthography

---|---|---|---|---
[g_cons](g_cons.md) | word | consonantal | transliterated | `>CR`
[g_cons_utf8](g_cons_utf8.md) | word | consonantal | hebrew | `אשׁר`
[g_word](g_word.md) | word | pointed | transliterated | `>:ACER&`
[g_word_utf8](g_word_utf8.md) | word | pointed | hebrew | `אֲשֶׁר`
[ketiv](ketiv.md) | word (ketiv) | consonantal | hebrew | `אֲשֶׁר`
[g_qere_utf8](g_qere_utf8.md) | word (qere) | pointed | hebrew | `אֲשֶׁר`
[trailer_utf8](trailer_utf8.md) | after-word | pointed | hebrew | `׃ ׆̇`
[qtrailer_utf8](trailer_utf8.md) | after-word (qere) | pointed | hebrew | `׃ ׆̇`
[phono](phono.md) | word | full | phonetic | `dāvˈār`
[phono_sep](phono.md) | after-word | full | phonetic | `.`

### Lexical

---|---|---|---|---
[lex](lex.md) | word | consonantal | transliterated | `>MR[`
[lex_utf8](lex_utf8.md) | word | consonantal | hebrew | `אמר[`
[g_lex](g_lex.md) | word | pointed | transliterated | `>MER`
[g_lex_utf8](g_lex_utf8.md) | word | pointed | hebrew | `אמֶר`

---|---|---|---
[language](language.md) | language | `Hebrew` `Aramaic`
[sp](sp.md) | part of speech | `verb` `subs`
[pdp](pdp.md) | phrase dependent part of speech | `verb` `subs`
[ls](ls.md) | lexical set | `quot` `ques`
[nametype](nametype.md) | type of named entity | `pers` `topo`

### Morphology

---|---|---
[gn](gn.md) | gender | `m` `f`
[nu](nu.md) | number | `sg` `pl` `du`
[ps](ps.md) | person | `p1` `p2` `p3`
[st](st.md) | state | `a` `c` `e`
[vs](vs.md) | verbal stem | `qal` `piel` `nif` `hif`
[vt](vt.md) | verbal tense | `perf` `impf` `wayq`

### Morphemes

---|---|---|---|---
[nme](nme.md) | [g_nme](g_nme.md) | [g_nme_utf8](g_nme_utf8.md) | nominal ending | `/` `/IJM` `/@H`
[pfm](pfm.md) | [g_pfm](g_pfm.md) | [g_pfm_utf8](g_pfm_utf8.md) | preformative | `!!` `!J.I!` `!TI!`
[prs](prs.md) | [g_prs](g_prs.md) | [g_prs_utf8](g_prs_utf8.md) | pronominal suffix | `+OW` `+IJ` `+HEM`
[uvf](uvf.md) | [g_uvf](g_uvf.md) | [g_uvf_utf8](g_uvf_utf8.md) | univalent final | `~@H` `~IJ` `~OW`
[vbe](vbe.md) | [g_vbe](g_vbe.md) | [g_vbe_utf8](g_vbe_utf8.md) | verbal ending | `[` `[W.` `[T.IJ`
[vbs](vbs.md) | [g_vbs](g_vbs.md) | [g_vbs_utf8](g_vbs_utf8.md) | root formation | `]]` `]NI]` `]HA]`

### Statistics

---|---
[freq_lex](freq_lex.md) | frequency of lexeme
[freq_occ](freq_occ) | frequency of word occurrence
[rank_lex](rank_lex) | rank of lexeme
[rank_occ](rank_occ) | rank of word occurrence

## Linguistic features

### Sentence(-atom) features

Nothing specific, just a generic `number` feature.

### Clause(-atom) features

---|---|---
[typ](typ) | clause type | `AjCl` `WayX` `WXQt` `ZImX`
[kind](kind) | rough clause type | `VC` `NC` `WP`
[rela](rela) | clause constituent relation | `Adju` `Attr` `Coor`
[domain](domain) | text type ?? | `Q` `N` `D`
[txt](txt) | text type | `NQ` `NQQ` `QNQQ` `NQND`
[code](code) | clause atom relation | `200` `477` `999`
[is_root](is_root) | ??
[tab](tab) | hierarchical tabulation | `0` `3` `10` `29`
[pargr](pargr) | paragraph number | `1` `1.2` `2.3.4`
[instruction](instruction) | instruction | `.q` `.d` `..` `ve`

### Phrase(-atom) features

---|---|---
[typ](typ) | phrase type | `VP` `NP` `PP` `AdjP` `AdvP`
[rela](rela) | phrase atom relation | `Appo` `Para` `Resu`
[function](function) | phrase function | `Pred` `Subj`
[det](det) | determination | `det` `und`

## Generic features

---|---|---
[number](number) | sequence number in context | `123`
[dist](dist) | distance to mother | `-10` `0`  `1` `8`
[dist_unit](dist_unit) | unit of measuring distance to mother | `clause_atoms` `phrase_atoms` `words`
[mother_object_type](mother_object_type) | object type of mother | `clause` `phrase` `subphrase` `word`
