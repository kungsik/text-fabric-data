# clause_kind

**clause kind**

This feature is present on objects of type *clause*.

**NB:**
In version 4b this feature is called [kind](kind).

This feature divides the clauses into three types: *verbal*, *nominal* and *without predication*.
It is related to the feature [typ](typ) on clauses, in the sense that each of the values of `clause_kind` 
corresponnds to a set of values of `typ`.

So, this is essentially a feature for convenience: it leads to more concise queries of which the intention is also clearer.

value | meaning | correspondence with `typ` values
---|---|---
`VC` | Verbal clauses | `InfA` `InfC` `Ptcp` `Way0` `WayX`
`NC` | Nominal clauses |
`WP` | Clauses without predication |

