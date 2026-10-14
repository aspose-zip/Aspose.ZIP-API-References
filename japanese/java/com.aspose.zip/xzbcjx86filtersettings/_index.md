---
title: "XzBcjX86FilterSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "xz Bcj X86 フィルタの設定。"
type: docs
weight: 148
url: /ja/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

xz Bcj X86 フィルタの設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | 新しいインスタンスを初期化します [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


新しいインスタンスを初期化します [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). それを使用して、[XzArchive](../../com.aspose.zip/xzarchive) 内の実行可能ファイルやライブラリを圧縮します。

```

``````

XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save("archive.xz");
}
 
```



