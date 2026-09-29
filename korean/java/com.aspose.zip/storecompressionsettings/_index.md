---
title: "StoreCompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZIP 아카이브 내 Store 압축에 대한 설정."
type: docs
weight: 124
url: /ko/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

ZIP 아카이브 내 Store 압축에 대한 설정.

이 메서드는 원본 데이터를 그대로 저장합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | 새 인스턴스를 초기화합니다. [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) 클래스. |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


새 인스턴스를 초기화합니다. [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) 클래스.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



