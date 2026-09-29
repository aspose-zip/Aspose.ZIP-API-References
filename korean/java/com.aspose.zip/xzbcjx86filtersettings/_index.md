---
title: "XzBcjX86FilterSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "xz Bcj X86 필터에 대한 설정."
type: docs
weight: 148
url: /ko/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

xz Bcj X86 필터에 대한 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | 새 인스턴스를 초기화합니다 [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


새 인스턴스를 초기화합니다 [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). 실행 파일 및 라이브러리를 [XzArchive](../../com.aspose.zip/xzarchive) 내에서 압축하는 데 사용합니다.

```

``````

XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save("archive.xz");
}
 
```



