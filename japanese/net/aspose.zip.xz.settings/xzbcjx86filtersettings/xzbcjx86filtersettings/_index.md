---
title: "XzBcjX86FilterSettings.XzBcjX86FilterSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XzBcjX86FilterSettings コンストラクタ。XzBcjX86FilterSettings の新しいインスタンスを初期化します。XzArchive 内の実行ファイルやライブラリを圧縮するために使用します"
type: docs
weight: 10
url: /ja/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

[`XzBcjX86FilterSettings`](../) の新しいインスタンスを初期化します。[`XzArchive`](../../../aspose.zip.xz/xzarchive/) 内の実行ファイルとライブラリを圧縮するために使用します。

```csharp
public XzBcjX86FilterSettings()
```

## 例

```csharp
XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
using (XzArchive archive = new XzArchive(settings))
{
    archive.SetSource("data.bin");
    archive.Save("archive.xz");
}
```

### 関連項目

* class [XzBcjX86FilterSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* assembly [Aspose.Zip](../../../)


