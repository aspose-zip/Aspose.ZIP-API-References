---
title: "TarArchive.SaveZstandard"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。Zstandard 圧縮でアーカイブをストリームに保存します"
type: docs
weight: 220
url: /ja/net/aspose.zip.tar/tararchive/savezstandard/
---
## SaveZstandard(Stream, TarFormat?) {#savezstandard}

Zstandard 圧縮を使用してストリームにアーカイブを保存します。

```csharp
public void SaveZstandard(Stream output, TarFormat? format = default)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |
| フォーマット | Nullable`1 | tar ヘッダー形式を定義します。null 値は可能な場合、USTar として扱われます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *output* は null です。 |
| ArgumentException | *output* は書き込み可能ではありません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |
| IOException | I/O エラーが発生しました。 |

## 備考

*output* must be writable.

## 例

```csharp
using (FileStream result = File.OpenWrite("result.tar.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
        }
    }
}
```

### 関連項目

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveZstandard(string, TarFormat?) {#savezstandard_1}

Zstandard 圧縮を使用してパスで指定されたファイルにアーカイブを保存します。

```csharp
public void SaveZstandard(string path, TarFormat? format = default)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| フォーマット | Nullable`1 | tar ヘッダー形式を定義します。null 値は可能な場合、USTar として扱われます。 |

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

## 例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.tar.zst");
    }
}
```

### 関連項目

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


