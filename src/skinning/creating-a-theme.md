# Creating a theme

The Chief framework supports linking a cascading style sheet file against a class that extends chief.skins.Theme.

- The `PropertyReference(name)` CSS calls resolve to a property within the chief.skins.Theme subclass scope, whether it is a static property or an instance property.

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