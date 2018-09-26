# Triangular numbers
{:#triangular-numbers}


Triangular numbers (of dimension 2) are defined by `T(n) = T(n;2) = n(n+1)/2 = Binomial(n+1,2)`.

More generally, triangular numbers of dimension 1 are `T(n;1) = n = Binomial(n,1)` and triangular numbers of dimension `d+1` are `T(n;d+1) = T(1;d) + ... + T(n;d) = Binomial(n+d-1,d)`.

<a id="TriangularNumber"></a><a id="TriangularNumber--RngIntElt--etc"></a><a id="TriangularNumber--RngIntElt--RngIntElt"></a>
> **TriangularNumber** (n :: *RngIntElt*, d :: *RngIntElt*)
> 
> -> *RngIntElt*
> {:.ret}
{:.intrinsic}

The `n`th triangular number in dimension `d`. Equal to `Binomial(n+d-1,d)`.


<a id="TriangularNumber-2"></a><a id="TriangularNumber--RngIntElt"></a>
> **TriangularNumber** (n :: *RngIntElt*)
> 
> -> *RngIntElt*
> {:.ret}
{:.intrinsic}

The `n`th triangular number. Equal to `Binomial(n+1,2) = n*(n+1)/2`.


<a id="LinearToTriangularIndex"></a><a id="LinearToTriangularIndex--RngIntElt--etc"></a><a id="LinearToTriangularIndex--RngIntElt--RngIntElt"></a>
> **LinearToTriangularIndex** (i :: *RngIntElt*, d :: *RngIntElt*)
> 
> -> []
> {:.ret}
{:.intrinsic}

Converts from linear to triangular indexing in dimension `d`. That is, returns the `i`th array `[i1,i2,...,id]` lexicographically with `i1 ge i2 ge ... ge id ge 1`.


<a id="LinearToTriangularIndex-2"></a><a id="LinearToTriangularIndex--RngIntElt"></a>
> **LinearToTriangularIndex** (i :: *RngIntElt*)
> 
> -> []
> {:.ret}
{:.intrinsic}

Converts from linear to triangular indexing. That is, returns the `i`th array `[i1,i2]` lexicographically with `i1 ge i2 ge 1`.


<a id="TriangularToLinearIndex"></a><a id="TriangularToLinearIndex--seq-RngIntElt--etc"></a><a id="TriangularToLinearIndex--seq-RngIntElt--RngIntElt"></a>
> **TriangularToLinearIndex** (idx :: [*RngIntElt*], d :: *RngIntElt*)
> 
> -> *RngIntElt*
> {:.ret}
{:.intrinsic}

Converts from triangular indexing in dimension `d` to linear.


<a id="TriangularToLinearIndex-2"></a><a id="TriangularToLinearIndex--seq-RngIntElt"></a>
> **TriangularToLinearIndex** (idx :: [*RngIntElt*])
> 
> -> *RngIntElt*
> {:.ret}
{:.intrinsic}

Converts from triangular indexing to linear.


