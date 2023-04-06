---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP for .NET API リファレンス
description: CpioArchive 方法. xz 圧縮でアーカイブをストリームに保存します
type: docs
weight: 100
url: /ja/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

xz 圧縮でアーカイブをストリームに保存します。

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| output | Stream | 宛先ストリーム。 |
| cpioFormat | CpioFormat | cpio ヘッダー形式を定義します。 |
| settings | XzArchiveSettings | 特定の xz アーカイブの設定のセット: 辞書サイズ、ブロック サイズ、チェック タイプ。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *output*無効である。 |
| ArgumentException | *output*書き込み不可です。 |

### 備考

*output*ストリームは書き込み可能である必要があります。

### 例

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### 関連項目

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* 名前空間 [Aspose.Zip.Cpio](../../cpioarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

xz 圧縮でパスごとにアーカイブをパスに保存します。

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 作成するアーカイブのパス。指定したファイル名が既存のファイルを指している場合、上書きされます。 |
| cpioFormat | CpioFormat | cpio ヘッダー形式を定義します。 |
| settings | XzArchiveSettings | 特定の xz アーカイブの設定のセット: 辞書サイズ、ブロック サイズ、チェック タイプ。 |

### 例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### 関連項目

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* 名前空間 [Aspose.Zip.Cpio](../../cpioarchive/)
* 組み立て [Aspose.Zip](../../../)


