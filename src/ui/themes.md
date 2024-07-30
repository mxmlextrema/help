# User interface themes

The MX framework supports linking cascading style sheet files against a mx.themes.Theme subclass.

- The `PropertyReference(name)` CSS calls resolve to a property within the mx.themes.Theme subclass scope, whether it is a static property or an instance property.

```as3
package
{
    import mx.themes.*;

    [Theme(source = "style.css")]
    public class RockTheme extends Theme
    {
    }
}
```