---
title: "XzArchiveSettings.XzArchiveSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XzArchiveSettings コンストラクタ。単一の LZMA2 圧縮を使用して XzArchiveSettings クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

[`XzArchiveSettings`](../) クラスの新しいインスタンスを単一の LZMA2 圧縮で初期化します。

```csharp
public XzArchiveSettings()
```

## 備考

LZMA2 フィルタのデフォルト辞書サイズは 16 メガバイト、デフォルトブロックサイズは 64 メガバイト、デフォルトのチェックサムタイプは CRC32 です。

### 関連項目

* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

[`XzArchiveSettings`](../) クラスの新しいインスタンスをカスタムパラメータで初期化します。

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filters | XzFilterSettings[] | [`XzArchive`](../../../aspose.zip.xz/xzarchive/) を作成するために順次適用されるフィルタ（圧縮器）です。単一の [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) または [`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) と [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) のペアのいずれかにできます。 |
| blockSize | Int64 | xz アーカイブブロックのサイズ。 |
| checkType | XzCheckType | 非圧縮データのチェックサム計算タイプ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* が負の値です。 |
| ArgumentNullException | *filters* が null です。 |
| ArgumentException | *filters* に 1 個未満または 2 個を超えるフィルターが含まれているか、最後のフィルターが [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) ではありません。 |

## 例

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
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)


