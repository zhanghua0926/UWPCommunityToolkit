# Visual Tree Extensions

The **VisualTree** extensions provide a collection of extensions methods for UI controls.

It provides [DependencyObject][1] extensions to aid in using the [VisualTreeHelper][2] class.
The official [VisualTreeHelper][2] documentation best explains reasons for walking the Visual Tree.

See also [LogicalTree Extensions](LogicalTree.md).

## Example

```csharp

	// Include namespace to access extensions.
	using Microsoft.Toolkit.Uwp.UI;

	// Find visual descendant control using its name.
	var control = uiElement.FindDescendantByName("MyTextBox");

	// Find first visual descendant control of a specified type.
	control = uiElement.FindDescendant<ListView>();

	// Find first visual ascendant control using its name.
	control = uiElement.FindAscendantByName("MyScrollViewer");

	// Find first visual ascendant control of a specified type.
	control = uiElement.FindAscendant<ScrollViewer>();
```

## Requirements (Windows 10 Device Family)

| [Device family](http://go.microsoft.com/fwlink/p/?LinkID=526370) | Universal, 10.0.10586.0 or higher |
| --- | --- |
| Namespace | Microsoft.Toolkit.Uwp.UI.Extensions |

## API

* [VisualTree extensions source code](https://github.com/Microsoft/UWPCommunityToolkit/blob/master/Microsoft.Toolkit.Uwp.UI/Extensions/Tree/VisualTree.cs)

[1]:https://docs.microsoft.com/en-us/uwp/api/Windows.UI.Xaml.DependencyObject
[2]:https://docs.microsoft.com/en-us/uwp/api/Windows.UI.Xaml.Media.VisualTreeHelper
