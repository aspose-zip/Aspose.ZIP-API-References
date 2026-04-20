---
title: XzArchiveSettings.XzArchiveSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: XzArchiveSettings コンストラクタ. の新しいインスタンスを初期化しますXzArchiveSettings単一の LZMA2 圧縮を使用するクラス.
type: docs
weight: 10
url: /ja/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

の新しいインスタンスを初期化します[`XzArchiveSettings`](../)単一の LZMA2 圧縮を使用するクラス.

```csharp
public XzArchiveSettings()
```

### 備考

LZMA2 フィルタ サイズのデフォルト辞書は 16 メガバイト、デフォルト ブロック サイズは 64 メガバイト、デフォルト チェックサム タイプは CRC32 です。

### 関連項目

* class [XzArchiveSettings](../)
* 名前空間 [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* 組み立て [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

の新しいインスタンスを初期化します[`XzArchiveSettings`](../)カスタム パラメータを持つクラス.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filters | XzFilterSettings[] | 作成するために順次適用されるフィルター (コンプレッサー)[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .単体でも可[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) またはペア[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/)と[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | xz アーカイブ ブロックのサイズ。 |
| checkType | XzCheckType | 非圧縮データのチェックサム計算のタイプ。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize*負です。 |
| ArgumentNullException | *filters*無効である |
| ArgumentException | *filters*フィルタが 1 つ未満または 2 つを超えるか、最後のフィルタがありません[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### 例

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### 関連項目

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* 名前空間 [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* 組み立て [Aspose.Zip](../../../)


