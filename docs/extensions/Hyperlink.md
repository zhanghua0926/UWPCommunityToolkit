# Hyperlink

The **Hyperlink** allows for a Hyperlink element to invoke the execute method on a bound [ICommand](https://msdn.microsoft.com/en-us/library/system.windows.input.icommand.aspx) instance when clicked.

## Example

```xml
	// Use Hyperlink in a wrapped TextBlock with text either side and ensure it executes a command when
	// clicked passing the current data context as the command parameter.
	<TextBlock>
	    <Run>Some leading text with a</Run>
	     <Hyperlink extensions:Hyperlink.Command="{Binding HyperlinkClicked}"
			        extensions:Hyperlink.CommandParameter="{Binding}">hyperlink</Hyperlink>
	    <Run>in the middle.</Run>
	</TextBlock>
```

## Requirements (Windows 10 Device Family)

| [Device family](http://go.microsoft.com/fwlink/p/?LinkID=526370) | Universal, 10.0.10586.0 or higher |
| --- | --- |
| Namespace | Microsoft.Toolkit.Uwp.Extensions |

## API

* [Hyperlink source code](https://github.com/Microsoft/UWPCommunityToolkit/blob/dev/Microsoft.Toolkit.Uwp.UI/Extensions/Hyperlink)

