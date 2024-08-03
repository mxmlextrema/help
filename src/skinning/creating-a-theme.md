# Creating a theme

The Chief framework supports linking  acascading style sheet file against a class that extends chief.themes.Theme.

- The `PropertyReference(name)` CSS calls resolve to a property within the chief.themes.Theme subclass scope, whether it is a static property or an instance property.

```as3
package
{
    import chief.skins.*;

    [SkinSheet(source="style.css")]
    public class RockTheme extends Theme
    {
    }
}
```