# Link.Expunge

This function is intended as a replacement for the system
function `⎕EX` in tools that manage code. It removes an item from the workspace and also deletes the corresponding source file.

If you manually `⎕EX` or `)ERASE` items, you can subsequently call Expunge to maintain synchronisation.

#### Arguments

- APL item name(s)

#### Result

- Simple Boolean vector with one element per name in Y.

   >The value of an element of the result is 1 if the corresponding name is now available for use.  This does not necessarily mean that the existing value was erased for that name.  A value of  0 is returned for an ill-formed name or for a distinguished name in the argument.


