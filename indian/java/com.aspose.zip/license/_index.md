---
title: "License"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "घटक को लाइसेंस करने के लिए मेथड प्रदान करता है।"
type: docs
weight: 79
url: /hi/java/com.aspose.zip/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

घटक को लाइसेंस करने के लिए मेथड प्रदान करता है।


इस उदाहरण में, कंपोनेंट jar फ़ाइल वाले फ़ोल्डर में MyLicense.lic नाम की लाइसेंस फ़ाइल खोजने का प्रयास किया जाएगा:

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


कंपोनेंट को लाइसेंस देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| licenseFile | java.io.File | फ़ाइल पाथनाम का प्रतिनिधित्व |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


कंपोनेंट को लाइसेंस देता है।

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| licenseName | java.lang.String | यह पूर्ण या संक्षिप्त फ़ाइल नाम या एम्बेडेड रिसोर्स का नाम हो सकता है। मूल्यांकन मोड में स्विच करने के लिए खाली स्ट्रिंग का उपयोग करें। |

