# Aggregates
{:#aggregates}

<a id="AssociativeArrayToMap"></a><a id="AssociativeArrayToMap--Assoc--etc"></a><a id="AssociativeArrayToMap--Assoc--any"></a>
> **AssociativeArrayToMap** (xs :: *Assoc*, codomain)
> 
> -> *Map*
> {:.ret}
{:.intrinsic}

The map from Keys(`xs`) to `codomain` implied by `xs`.


<a id="AssociativeArrayToMap-2"></a><a id="AssociativeArrayToMap--Assoc"></a>
> **AssociativeArrayToMap** (xs :: *Assoc*)
> 
> -> *Map*
> {:.ret}
{:.intrinsic}

The map from Keys(`xs`) to Universe(Values(`xs`)) implies by `xs`.


<a id="GroupBy"></a><a id="GroupBy--seq--etc"></a><a id="GroupBy--seq--UserProgram"></a><a id="GroupBy--seq--any"></a><a id="GroupBy--set--etc"></a><a id="GroupBy--set--UserProgram"></a><a id="GroupBy--set--any"></a>
> **GroupBy** (xs :: [], key :: *UserProgram*)
> 
> **GroupBy** (xs :: [], key)
> 
> **GroupBy** (xs :: {}, key :: *UserProgram*)
> 
> **GroupBy** (xs :: {}, key)
> 
> -> *Assoc*
> {:.ret}
{:.intrinsic}

The associative array whose keys are the unique values of `key(x)` over `x` in `xs`, and whose values are the subset of corresponding `x`.








<a id="ItemsList"></a><a id="ItemsList--Assoc"></a>
> **ItemsList** (xs :: *Assoc*)
> 
> -> *List*
> {:.ret}
{:.intrinsic}

Key-value pairs.


<a id="Items"></a><a id="Items--seq"></a><a id="Items--Assoc"></a>
> **Items** (xs :: [])
> 
> **Items** (xs :: *Assoc*)
> 
> -> []
> {:.ret}
{:.intrinsic}

Key-value pairs.




<a id="ItemsToAssociativeArray"></a><a id="ItemsToAssociativeArray--any"></a>
> **ItemsToAssociativeArray** (items)
> 
> -> *Assoc*
> {:.ret}
{:.intrinsic}

The associative array such that `items`[i][2] is the value at key `items`[i][1].


<a id="KeyFunction"></a><a id="KeyFunction--set-seq-seq--etc"></a><a id="KeyFunction--set-seq-seq--RngIntElt"></a><a id="KeyFunction--set-seq-Tup--etc"></a><a id="KeyFunction--set-seq-Tup--RngIntElt"></a><a id="KeyFunction--set-seq-List--etc"></a><a id="KeyFunction--set-seq-List--RngIntElt"></a><a id="KeyFunction--set-seq-Rec--etc"></a><a id="KeyFunction--set-seq-Rec--MonStgElt"></a><a id="KeyFunction--set-seq-Assoc--etc"></a><a id="KeyFunction--set-seq-Assoc--any"></a>
> **KeyFunction** (U :: {[[]]}, i :: *RngIntElt*)
> 
> **KeyFunction** (U :: {[*Tup*]}, i :: *RngIntElt*)
> 
> **KeyFunction** (U :: {[*List*]}, i :: *RngIntElt*)
> 
> **KeyFunction** (U :: {[*Rec*]}, i :: *MonStgElt*)
> 
> **KeyFunction** (U :: {[*Assoc*]}, i)
> 
> -> *UserProgram*
> {:.ret}
{:.intrinsic}

The function retrieving the `i`th entry of an element of `U`.










<a id="KeyFunction-2"></a><a id="KeyFunction--set-seq--etc"></a><a id="KeyFunction--set-seq--Map"></a>
> **KeyFunction** (U :: {[]}, i :: *Map*)
> 
> -> *UserProgram*
> {:.ret}
{:.intrinsic}

The map as a function.


<a id="KeyFunction-3"></a><a id="KeyFunction--set-seq--etc-2"></a><a id="KeyFunction--set-seq--Intrinsic"></a>
> **KeyFunction** (U :: {[]}, i :: *Intrinsic*)
> 
> -> *UserProgram*
> {:.ret}
{:.intrinsic}

The intrinsic as a function.


<a id="Keys"></a><a id="Keys--seq"></a>
> **Keys** (xs :: [])
> 
> -> {}
> {:.ret}
{:.intrinsic}

The indices of defined entries of `xs`.


<a id="RandomSubset"></a><a id="RandomSubset--Str--etc"></a><a id="RandomSubset--Str--RngIntElt"></a><a id="RandomSubset--seq--etc"></a><a id="RandomSubset--seq--RngIntElt"></a>
> **RandomSubset** (X :: *Str*, n :: *RngIntElt*)
> 
> **RandomSubset** (X :: [], n :: *RngIntElt*)
> 
> -> {}
> {:.ret}
{:.intrinsic}

A random set of `n` distinct elements of `X`.




<a id="Shuffle"></a><a id="Shuffle--seq--etc"></a><a id="Shuffle--seq--RngIntElt"></a>
> **Shuffle** (X :: [], n :: *RngIntElt*)
> 
> -> []
> {:.ret}
{:.intrinsic}

A copy of the first `n` elements of `X` in a random order.


<a id="Shuffle-2"></a><a id="Shuffle--seq"></a><a id="Shuffle--List"></a><a id="Shuffle--iset"></a><a id="Shuffle--set"></a>
> **Shuffle** (X :: [])
> 
> -> []
> {:.ret}
> 
> **Shuffle** (X :: *List*)
> 
> -> *List*
> {:.ret}
> 
> **Shuffle** (X :: {@@})
> 
> **Shuffle** (X :: {})
> 
> -> {@@}
> {:.ret}
{:.intrinsic}

A copy of `X` in a random order.








<a id="SortBy"></a><a id="SortBy--seq--etc"></a><a id="SortBy--seq--UserProgram--any"></a><a id="SortBy--seq--any"></a>
> **SortBy** (~xs :: [], key :: *UserProgram*, ~permut)
> 
> **SortBy** (~xs :: [], key)
{:.intrinsic}

Sorts the sequence `xs` in place according to the given `key`.




<a id="SortBy-2"></a><a id="SortBy--seq--etc-2"></a><a id="SortBy--seq--any-2"></a>
> **SortBy** (xs :: [], key)
> 
> -> [], *GrpPermElt*
> {:.ret}
{:.intrinsic}

Sorts the sequence according to the given `key`. Also returns the corresponding permutation.


<a id="SortBy-3"></a><a id="SortBy--seq--etc-3"></a><a id="SortBy--seq--any--any"></a>
> **SortBy** (~xs :: [], key, ~permut)
{:.intrinsic}

Sorts the sequence `xs` in place by the `key`'th entry.


<a id="ToIndexedSet"></a><a id="ToIndexedSet--any"></a><a id="ToIndexedSet--iset"></a><a id="ToIndexedSet--set"></a>
> **ToIndexedSet** (xs)
> 
> **ToIndexedSet** (xs :: {@@})
> 
> **ToIndexedSet** (xs :: {})
> 
> -> {@@}
> {:.ret}
{:.intrinsic}

Converts `xs` to an indexed set.






<a id="ToList"></a><a id="ToList--any"></a><a id="ToList--List"></a><a id="ToList--Tup"></a><a id="ToList--seq"></a>
> **ToList** (xs)
> 
> **ToList** (xs :: *List*)
> 
> **ToList** (xs :: *Tup*)
> 
> **ToList** (xs :: [])
> 
> -> *List*
> {:.ret}
{:.intrinsic}

Converts `xs` to a list.








<a id="ToMultiset"></a><a id="ToMultiset--any"></a><a id="ToMultiset--mset"></a><a id="ToMultiset--set"></a><a id="ToMultiset--seq"></a>
> **ToMultiset** (xs)
> 
> **ToMultiset** (xs :: {**})
> 
> **ToMultiset** (xs :: {})
> 
> **ToMultiset** (xs :: [])
> 
> -> {**}
> {:.ret}
{:.intrinsic}

Converts `xs` to a multiset.








<a id="ToSequence"></a><a id="ToSequence--any"></a><a id="ToSequence--seq"></a><a id="ToSequence--set"></a><a id="ToSequence--mset"></a><a id="ToSequence--iset"></a>
> **ToSequence** (xs)
> 
> **ToSequence** (xs :: [])
> 
> **ToSequence** (xs :: {})
> 
> **ToSequence** (xs :: {**})
> 
> **ToSequence** (xs :: {@@})
> 
> -> []
> {:.ret}
{:.intrinsic}

Converts `xs` to a sequence.










<a id="ToSet"></a><a id="ToSet--any"></a><a id="ToSet--set"></a><a id="ToSet--seq"></a><a id="ToSet--mset"></a><a id="ToSet--iset"></a>
> **ToSet** (xs)
> 
> **ToSet** (xs :: {})
> 
> **ToSet** (xs :: [])
> 
> **ToSet** (xs :: {**})
> 
> **ToSet** (xs :: {@@})
> 
> -> {}
> {:.ret}
{:.intrinsic}

Converts `xs` to a set.










<a id="ToTuple"></a><a id="ToTuple--any"></a><a id="ToTuple--Tup"></a>
> **ToTuple** (xs)
> 
> **ToTuple** (xs :: *Tup*)
> 
> -> *Tup*
> {:.ret}
{:.intrinsic}

Converts `xs` to a tuple.




<a id="Unzip"></a><a id="Unzip--seq-Tup"></a>
> **Unzip** (pairs :: [*Tup*])
> 
> -> [], []
> {:.ret}
{:.intrinsic}

The first and second of each pair in `pairs`.


<a id="Unzip3"></a><a id="Unzip3--seq-Tup"></a>
> **Unzip3** (triples :: [*Tup*])
> 
> -> [], [], []
> {:.ret}
{:.intrinsic}

The first, second and third of each triple in `triples`.


<a id="ValuesList"></a><a id="ValuesList--Assoc"></a>
> **ValuesList** (xs :: *Assoc*)
> 
> -> *List*
> {:.ret}
{:.intrinsic}

The defined values of `xs`.


<a id="Values"></a><a id="Values--seq"></a><a id="Values--Assoc"></a>
> **Values** (xs :: [])
> 
> **Values** (xs :: *Assoc*)
> 
> -> []
> {:.ret}
{:.intrinsic}

The defined values of `xs`.




<a id="Zip"></a><a id="Zip--seq--etc"></a><a id="Zip--seq--seq"></a>
> **Zip** (xs :: [], ys :: [])
> 
> -> []
> {:.ret}
{:.intrinsic}

The corresponding pairs from each list, where both are defined.


<a id="Zip-2"></a><a id="Zip--seq--etc-2"></a><a id="Zip--seq--seq--seq"></a>
> **Zip** (xs :: [], ys :: [], zs :: [])
> 
> -> []
> {:.ret}
{:.intrinsic}

The corresponding triples from each list, where all are defined.


