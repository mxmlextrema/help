# Source specification

Sources are specified by recursive directories referred to as *source paths*. A source path is not taken as a source unless the respective MXMLShare manifest `source` element sets `include` to true.

## Include directive

ActionScript files that are loaded from an `include` directive must always contain an `.include.as` extension.

The following is an example ActionScript 3 program demonstrating the case:

```as3
// src/bath.as
package
{
    public function bath():void
    {
        include "./bathLog.include.as";
    }
}

// src/bathLog.include.as
trace("taking a bath");
```