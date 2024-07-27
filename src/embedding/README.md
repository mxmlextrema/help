# Embedding

There are several ways of embedding static media in ActionScript 3 programs. Both ActionScript 3, MXML and CSS have a way of embedding static media.

- ActionScript 3 uses the `[Embed]` meta data either in classes or variables.
- CSS uses the `Embed()` function.
- CSS uses `@font-face` statements that embed a local or system font.

## Embed meta-data

The `[Embed]` ActionScript 3 meta-data is used in two different ways.

It may appear in a class definition:

```as3
package
{
    import flash.utils.*;

    [Embed(...)]
    public class CustomFont extends ByteArray
    {
    }
}
```

It may appear in a variable definition:

```as3
package
{
    public class StaticFonts
    {
        [Embed(...)]
        public static const custom:Class;
    }
}
```