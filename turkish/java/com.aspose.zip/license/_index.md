---
title: "License"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bileşeni lisanslamak için yöntemler sağlar."
type: docs
weight: 79
url: /tr/java/com.aspose.zip/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Bileşeni lisanslamak için yöntemler sağlar.


Bu örnekte, bileşen jar dosyasını içeren klasörde MyLicense.lic adlı bir lisans dosyası bulunmaya çalışılacaktır:

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


Bileşeni lisanslandırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| licenseFile | java.io.File | dosya yolu adının temsili |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


Bileşeni lisanslandırır.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| licenseName | java.lang.String | Tam veya kısa bir dosya adı ya da gömülü kaynağın adı olabilir. Değerlendirme moduna geçmek için boş bir dize kullanın. |

