---
title: "CpioArchive.SaveXzCompressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CpioArchive メソッド。xz 圧縮でストリームにアーカイブを保存します。"
type: docs
weight: 120
url: /ja/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

xz 圧縮でアーカイブをストリームに保存します。

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |
| cpioFormat | CpioFormat | cpio ヘッダー形式を定義します。 |
| 設定 | XzArchiveSettings | 特定の xz アーカイブの設定セット：辞書サイズ、ブロックサイズ、チェックタイプ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *output* は null です。 |
| ArgumentException | *output* は書き込み可能ではありません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

*output*The stream must be writable.

## 例

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
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

xz 圧縮でパスで指定されたパスにアーカイブを保存します。

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| cpioFormat | CpioFormat | cpio ヘッダー形式を定義します。 |
| 設定 | XzArchiveSettings | 特定の xz アーカイブの設定セット：辞書サイズ、ブロックサイズ、チェックタイプ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentNullException | *path* は `null` です。 |
| IOException | I/O エラーが発生しました。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |

## 例

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
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


