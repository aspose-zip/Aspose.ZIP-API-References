---
title: Class License
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.License clase. Proporciona métodos para licenciar el componente.
type: docs
weight: 260
url: /es/net/aspose.zip/license/
---
## License class

Proporciona métodos para licenciar el componente.

```csharp
public class License
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [License](license/)() | Inicializa una nueva instancia del`License` clase. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | Licencia el componente. |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | Licencia el componente. |

### Ejemplos

En este ejemplo, se intentará encontrar un archivo de licencia llamado MyLicense.lic en la carpeta que contiene  el componente, en la carpeta que contiene el ensamblado que llama, en la carpeta del ensamblado de entrada y luego en los recursos incrustados del ensamblado que llama.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

el archivo jar del componente:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Ver también

* espacio de nombres [Aspose.Zip](../../aspose.zip/)
* asamblea [Aspose.Zip](../../)


