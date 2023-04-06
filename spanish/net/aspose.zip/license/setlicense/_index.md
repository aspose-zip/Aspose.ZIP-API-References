---
title: License.SetLicense
second_title: Referencia de la API de Aspose.ZIP para .NET
description: License método. Licencia el componente.
type: docs
weight: 20
url: /es/net/aspose.zip/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licencia el componente.

```csharp
public void SetLicense(string licenseName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| licenseName | String | Puede ser un nombre de archivo completo o corto o el nombre de un recurso incrustado. Use una cadena vacía para cambiar al modo de evaluación. |

### Observaciones

Intenta encontrar la licencia en las siguientes ubicaciones:

1. Ruta explícita.

2. La carpeta que contiene el ensamblaje del componente Aspose.

3. La carpeta que contiene el ensamblado de llamada del cliente.

4. La carpeta que contiene el ensamblado de entrada (inicio).

5. Un recurso incrustado en el ensamblado de llamada del cliente.

**Nota:**En .NET Compact Framework, intenta encontrar la licencia solo en estas ubicaciones:

1. Ruta explícita.

2. Un recurso incrustado en el ensamblado de llamadas del cliente.

2. La carpeta que contiene el archivo JAR del componente Aspose.

3. La carpeta que contiene el archivo JAR de llamada del cliente.

### Ejemplos

En este ejemplo, se intentará encontrar un archivo de licencia llamado MyLicense.lic en la carpeta que contiene  el componente, en la carpeta que contiene el ensamblado que llama, en la carpeta del ensamblado de entrada y luego en los recursos incrustados del ensamblado que llama.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
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

---

## SetLicense(Stream) {#setlicense}

Licencia el componente.

```csharp
public void SetLicense(Stream stream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | Un flujo que contiene la licencia. |

### Observaciones

Utilice este método para cargar una licencia desde una secuencia.

### Ejemplos

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### Ver también

* class [License](../)
* espacio de nombres [Aspose.Zip](../../license/)
* asamblea [Aspose.Zip](../../../)


