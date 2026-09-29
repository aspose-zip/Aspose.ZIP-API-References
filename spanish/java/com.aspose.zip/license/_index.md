---
title: "License"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Proporciona métodos para licenciar el componente."
type: docs
weight: 79
url: /es/java/com.aspose.zip/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Proporciona métodos para licenciar el componente.


En este ejemplo, se intentará encontrar un archivo de licencia llamado MyLicense.lic en la carpeta que contiene el archivo jar del componente:

```

``````

License license = new License();
license.setLicense("MyLicense.lic");
 
```


## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | Initializes a new instance of the [License](../../com.aspose.zip/license) class. |
## Methods

| Method | Description |
| --- | --- |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Licenses the component. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licenses the component. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Licenses the component. |
### License() {#License--}
```
public License()
```


Initializes a new instance of the [License](../../com.aspose.zip/license) class.


In this example, an attempt will be made to find a license file named MyLicense.lic in the folder that contains the component jar file:

```

``````

     License license = new License();
     license.setLicense("MyLicense.lic");
 
```



### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Licencia el componente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| licenseFile | java.io.File | representación de la ruta del archivo |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


Licencia el componente.

```

``````

License license = new License();
license.setLicense(myStream);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A stream that contains the license. |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Licenses the component.

Library tries to find the license in the following locations:

1. Explicit path.

2. The folder that contains the Aspose component JAR file.

3. The folder that contains the client's calling JAR file.


In this example, an attempt will be made to find a license file named MyLicense.lic in locations listed above:

```

``````

     License license = new License();
     license.setLicense("MyLicense.lic");
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| licenseName | java.lang.String | Puede ser un nombre de archivo completo o corto o el nombre de un recurso incrustado. Use una cadena vacía para cambiar al modo de evaluación. |

