---
title: License.License
second_title: Referencia de la API de Aspose.ZIP para .NET
description: License constructor. Inicializa una nueva instancia delLicense clase.
type: docs
weight: 10
url: /es/net/aspose.zip/license/license/
---
## License constructor

Inicializa una nueva instancia del[`License`](../) clase.

```csharp
public License()
```

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

* class [License](../)
* espacio de nombres [Aspose.Zip](../../license/)
* asamblea [Aspose.Zip](../../../)


