# Creating a theme

The MX framework supports linking  acascading style sheet file against a class that extends mx.themes.Theme.

- The `PropertyReference(name)` CSS calls resolve to a property within the mx.themes.Theme subclass scope, whether it is a static property or an instance property.

```as3
package
{
    import mx.themes.*;

    [Theme(file = "style.css")]
    public class RockTheme extends Theme
    {
    }
}
```