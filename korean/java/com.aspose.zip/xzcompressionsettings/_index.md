---
title: "XzCompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZIP 아카이브 내 Xz 압축에 대한 설정."
type: docs
weight: 149
url: /ko/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

ZIP 아카이브 내 Xz 압축에 대한 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | 새로운 [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) 클래스의 인스턴스를 초기화합니다. |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


새로운 [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) 클래스의 인스턴스를 초기화합니다.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(\"archive.zip\");
}
 
```



