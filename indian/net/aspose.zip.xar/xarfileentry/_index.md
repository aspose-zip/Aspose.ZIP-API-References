---
title: Class XarFileEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.Xar.XarFileEntry कक्ष. xar संग्रह के भतर फ़इल प्रवष्ट क प्रतनधत्व करत है
type: docs
weight: 840
url: /hi/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

xar संग्रह के भीतर फ़ाइल प्रविष्टि का प्रतिनिधित्व करता है।

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## गुण

| नाम | विवरण |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | फ़ाइल या निर्देशिका का निर्माण समय प्राप्त करता है। |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | संग्रह के भीतर प्रविष्टि का पूरा पथ प्राप्त करता है। |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि प्रविष्टि निर्देशिका का प्रतिनिधित्व करती है या नहीं। |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | फ़ाइल या निर्देशिका का अंतिम एक्सेस समय प्राप्त करता है। |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | फ़ाइल या निर्देशिका का संशोधन समय प्राप्त करता है। |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | बाइट्स में प्रविष्टि की लंबाई प्राप्त करता है। |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | संग्रह के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | वह मूल निर्देशिका प्राप्त करता है जिसकी प्रविष्टि संबंधित है. |

## तरीकों

| नाम | विवरण |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | प्रदान की गई स्ट्रीम की प्रविष्टि निकालता है. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | दिए गए पथ द्वारा फाइल सिस्टम में प्रवेश को निकालता है। |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | निष्कर्षण के लिए प्रविष्टि खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### यह सभी देखें

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* नाम स्थान [Aspose.Zip.Xar](../../aspose.zip.xar/)
* सभा [Aspose.Zip](../../)


