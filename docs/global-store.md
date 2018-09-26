# Global store
{:#global-store}


We define a "global store", which is a store (an associative array which is modifiable without a reference, as defined by `NewStore()`) defined globally. It is accessible with `GlobalStore()`, and we provide intrinsics to modify and query it directly.

This is mainly useful for debugging. Specifically it allows us to save values from within the Magma debugger, and retrieve them from the normal prompt.

<a id="GlobalStore"></a><a id="GlobalStore--noargs"></a>
> **GlobalStore** ()
> 
> -> Any
> {:.ret}
{:.intrinsic}

The global store.


<a id="GlobalStoreClear"></a><a id="GlobalStoreClear--noargs"></a>
> **GlobalStoreClear** ()
{:.intrinsic}

Clears the global store.


<a id="GlobalStoreGet"></a><a id="GlobalStoreGet--MonStgElt"></a>
> **GlobalStoreGet** (field :: *MonStgElt*)
> 
> -> Any
> {:.ret}
{:.intrinsic}

The value of the given `field` in the global store.


<a id="GlobalStoreIsDefined"></a><a id="GlobalStoreIsDefined--MonStgElt"></a>
> **GlobalStoreIsDefined** (field :: *MonStgElt*)
> 
> -> *BoolElt*, Any
> {:.ret}
{:.intrinsic}

True if the `field` is defined in the global store. If so, also returns the value.


<a id="GlobalStoreKeys"></a><a id="GlobalStoreKeys--noargs"></a>
> **GlobalStoreKeys** ()
> 
> -> {}
> {:.ret}
{:.intrinsic}

The set of field names defined in the global store.


<a id="GlobalStoreRemove"></a><a id="GlobalStoreRemove--MonStgElt"></a>
> **GlobalStoreRemove** (field :: *MonStgElt*)
{:.intrinsic}

Removes the given `field` from the global store.


<a id="GlobalStoreSet"></a><a id="GlobalStoreSet--MonStgElt--etc"></a><a id="GlobalStoreSet--MonStgElt--any"></a>
> **GlobalStoreSet** (field :: *MonStgElt*, value)
{:.intrinsic}

Sets the `field` to the given `value` in the global store.


