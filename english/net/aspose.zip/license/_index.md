---
title: Class License
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.License class. Provides methods to license the component
type: docs
weight: 420
url: /net/aspose.zip/license/
---
## License class

Provides methods to license the component.

```csharp
public sealed class License
```

## Constructors

| Name | Description |
| --- | --- |
| [License](license/)() | Initializes a new instance of the `License` class. |

## Methods

| Name | Description |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | Licenses the component. |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | Licenses the component. |

## Examples

In this example, an attempt will be made to find a license file named MyLicense.lic in the folder that contains  the component, in the folder that contains the calling assembly, in the folder of the entry assembly and then in the embedded resources of the calling assembly.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

the component jar file:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### See Also

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


