---
title: "DeflateCompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZIP 아카이브 내 Deflate 압축에 대한 설정."
type: docs
weight: 59
url: /ko/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

ZIP 아카이브 내 Deflate 압축에 대한 설정.

Deflate는 LZ77 알고리즘과 허프만 코딩을 결합한 무손실 데이터 압축 알고리즘입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | 새 인스턴스를 초기화합니다 [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) 클래스의. |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


새 인스턴스를 초기화합니다 [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) 클래스의.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



