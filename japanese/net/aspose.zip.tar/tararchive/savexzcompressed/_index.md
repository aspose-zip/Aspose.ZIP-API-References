---
title: "TarArchive.SaveXzCompressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。xz 圧縮でアーカイブをストリームに保存します"
type: docs
weight: 200
url: /ja/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

xz 圧縮でアーカイブをストリームに保存します。

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |
| フォーマット | Nullable`1 | tar ヘッダー形式を定義します。null 値は可能な場合、USTar として扱われます。 |
| 設定 | XzArchiveSettings | 特定の xz アーカイブの設定セット：辞書サイズ、ブロックサイズ、チェックタイプ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *output* は null です。 |
| ArgumentException | *output* は書き込み可能ではありません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |
| IOException | I/O エラーが発生しました。 |

## 備考

*output*The stream must be writable.

## 例

```csharp
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### 関連項目

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

xz 圧縮でパスで指定されたパスにアーカイブを保存します。

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| フォーマット | Nullable`1 | tar ヘッダー形式を定義します。null 値は可能な場合、USTar として扱われます。 |
| 設定 | XzArchiveSettings | 特定の xz アーカイブの設定セット：辞書サイズ、ブロックサイズ、チェックタイプ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| UnauthorizedAccessException | 呼び出し元に必要な権限がありません。-または- *path* が読み取り専用のファイルまたはディレクトリを指定しました。 |
| ArgumentException | *path* は長さゼロの文字列であるか、空白文字のみを含むか、InvalidPathChars で定義された 1 つ以上の無効な文字を含んでいます。 |
| ArgumentNullException | *path* が null です。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| DirectoryNotFoundException | 指定された *path* は無効です（例: マッピングされていないドライブ上にある場合）。 |
| NotSupportedException | *path* の形式が無効です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |
| IOException | I/O エラーが発生しました。 |

## 例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### 関連項目

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


