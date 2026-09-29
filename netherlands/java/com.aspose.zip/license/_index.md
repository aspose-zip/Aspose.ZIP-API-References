---
title: "License"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Biedt methoden om de component te licentiëren."
type: docs
weight: 79
url: /nl/java/com.aspose.zip/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Biedt methoden om de component te licentiëren.


In dit voorbeeld wordt geprobeerd een licentiebestand met de naam MyLicense.lic te vinden in de map die het component‑jar‑bestand bevat:

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


Licentieert het component.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| licenseFile | java.io.File | representatie van bestandsnaampad |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


Licentieert het component.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| licenseName | java.lang.String | Kan een volledige of korte bestandsnaam of de naam van een ingebedde bron zijn. Gebruik een lege tekenreeks om over te schakelen naar evaluatiemodus. |

