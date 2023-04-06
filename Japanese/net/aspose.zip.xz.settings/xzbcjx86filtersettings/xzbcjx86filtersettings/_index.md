---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: XzBcjX86FilterSettings コンストラクタ. の新しいインスタンスを初期化しますXzBcjX86FilterSettings .実行可能ファイルとライブラリを圧縮するために使用しますXzArchive .
type: docs
weight: 10
url: /ja/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

の新しいインスタンスを初期化します[`XzBcjX86FilterSettings`](../) .実行可能ファイルとライブラリを圧縮するために使用します[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### 例

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
* 名前空間 [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* 組み立て [Aspose.Zip](../../../)


