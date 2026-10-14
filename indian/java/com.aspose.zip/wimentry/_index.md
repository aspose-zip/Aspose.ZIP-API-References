---
title: "WimEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "wim इमेज के भीतर एकल फ़ाइल या निर्देशिका का प्रतिनिधित्व करता है।"
type: docs
weight: 132
url: /hi/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

wim इमेज के भीतर एकल फ़ाइल या निर्देशिका का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | फ़ाइल या निर्देशिका के वैकल्पिक डेटा स्ट्रीम के नाम प्राप्त करता है। |
| [getArchive()](#getArchive--) | प्रविष्टि जिस आर्काइव से संबंधित है उसे प्राप्त करता है। |
| [getChangeTime()](#getChangeTime--) | फ़ाइल या निर्देशिका के अंतिम परिवर्तन का समय प्राप्त करता है। |
| [getCreationTime()](#getCreationTime--) | फ़ाइल या निर्देशिका का निर्माण समय प्राप्त करता है। |
| [getFileAttributes()](#getFileAttributes--) | फ़ाइल या निर्देशिका के गुण प्राप्त करता है। |
| [getFullPath()](#getFullPath--) | छवि के भीतर प्रविष्टि का पूर्ण पथ प्राप्त करता है। |
| [getHardLink()](#getHardLink--) | फ़ाइल या निर्देशिका का हार्डलिंक आईडी प्राप्त करता है। |
| [getImage()](#getImage--) | प्रविष्टि जिस छवि से संबंधित है, उसे प्राप्त करता है। |
| [getLastAccessTime()](#getLastAccessTime--) | फ़ाइल या निर्देशिका का अंतिम अभिगमन समय प्राप्त करता है। |
| [getLastWriteTime()](#getLastWriteTime--) | फ़ाइल या निर्देशिका का संशोधन समय प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | फ़ाइल या निर्देशिका का संशोधन समय प्राप्त करता है। |
| [getName()](#getName--) | छवि के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [getParent()](#getParent--) | प्रविष्टि जिस मूल निर्देशिका से संबंधित है, उसे प्राप्त करता है। |
| [getShortName()](#getShortName--) | छवि के भीतर प्रविष्टि का संक्षिप्त नाम प्राप्त करता है। |
| [hasHardLinks()](#hasHardLinks--) | फ़ाइल या निर्देशिका के अन्य नामों से ज्ञात होने की स्थिति प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | यह दर्शाने वाला मान प्राप्त करता है कि प्रविष्टि एक निर्देशिका है या नहीं। |
| [toString()](#toString--) | वर्ग [WimEntry](../../com.aspose.zip/wimentry) की इंस्टेंस का स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


फ़ाइल या निर्देशिका के वैकल्पिक डेटा स्ट्रीम के नाम प्राप्त करता है।

**Returns:**
java.lang.String[] - फ़ाइल या निर्देशिका के वैकल्पिक डेटा स्ट्रीम के नाम
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


प्रविष्टि जिस आर्काइव से संबंधित है उसे प्राप्त करता है।

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


फ़ाइल या निर्देशिका के अंतिम परिवर्तन का समय प्राप्त करता है।

**Returns:**
java.util.Date - फ़ाइल या निर्देशिका के अंतिम परिवर्तन का समय
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


फ़ाइल या निर्देशिका का निर्माण समय प्राप्त करता है।

**Returns:**
java.util.Date - फ़ाइल या निर्देशिका का निर्माण समय
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


फ़ाइल या निर्देशिका के गुण प्राप्त करता है।

**Returns:**
int - फ़ाइल या निर्देशिका के गुण
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


छवि के भीतर प्रविष्टि का पूर्ण पथ प्राप्त करता है।

**Returns:**
java.lang.String - छवि के भीतर प्रविष्टि का पूर्ण पथ
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


फ़ाइल या निर्देशिका का हार्डलिंक आईडी प्राप्त करता है।

**Returns:**
long - फ़ाइल या निर्देशिका का हार्डलिंक आईडी
### getImage() {#getImage--}
```
public final WimImage getImage()
```


प्रविष्टि जिस छवि से संबंधित है, उसे प्राप्त करता है।

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


फ़ाइल या निर्देशिका का अंतिम अभिगमन समय प्राप्त करता है।

**Returns:**
java.util.Date - फ़ाइल या निर्देशिका का अंतिम पहुँच समय
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


फ़ाइल या निर्देशिका का संशोधन समय प्राप्त करता है।

**Returns:**
java.util.Date - फ़ाइल या निर्देशिका का संशोधन समय
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


फ़ाइल या निर्देशिका का संशोधन समय प्राप्त करता है।

**Returns:**
java.util.Date - फ़ाइल या निर्देशिका का संशोधन समय
### getName() {#getName--}
```
public final String getName()
```


छवि के भीतर प्रविष्टि का नाम प्राप्त करता है।

**Returns:**
java.lang.String - छवि के भीतर प्रविष्टि का नाम
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


प्रविष्टि जिस मूल निर्देशिका से संबंधित है, उसे प्राप्त करता है।

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


छवि के भीतर प्रविष्टि का संक्षिप्त नाम प्राप्त करता है।

**Returns:**
java.lang.String - छवि के भीतर प्रविष्टि का संक्षिप्त नाम
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


फ़ाइल या निर्देशिका के अन्य नामों से ज्ञात होने की स्थिति प्राप्त करता है।

**Returns:**
boolean - क्या फ़ाइल या निर्देशिका को अन्य नामों से जाना जाता है
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


यह दर्शाने वाला मान प्राप्त करता है कि प्रविष्टि एक निर्देशिका है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि प्रविष्टि एक निर्देशिका का प्रतिनिधित्व करती है या नहीं
### toString() {#toString--}
```
public String toString()
```


वर्ग [WimEntry](../../com.aspose.zip/wimentry) की इंस्टेंस का स्ट्रिंग प्रतिनिधित्व लौटाता है।

**Returns:**
java.lang.String - इस ऑब्जेक्ट का स्ट्रिंग प्रतिनिधित्व
