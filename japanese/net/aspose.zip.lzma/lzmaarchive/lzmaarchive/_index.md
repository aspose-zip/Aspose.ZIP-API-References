---
title: "LzmaArchive.LzmaArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzmaArchive コンストラクタ。LzmaArchive クラスの新しいインスタンスを初期化し、lzma 形式でアーカイブを作成します"
type: docs
weight: 10
url: /ja/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

[`LzmaArchive`](../) クラスの新しいインスタンスを初期化し、lzma 形式でアーカイブを作成します。

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 設定 | LzmaArchiveSettings | 特定の lzma アーカイブの設定セットです。 |

### 関連項目

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

[`LzmaArchive`](../) クラスの新しいインスタンスを初期化し、解凍のために準備します。

```csharp
public LzmaArchive(Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソースです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *source* が null です。 |

## 備考

このコンストラクタは解凍しません。解凍については [`Extract`](../extract/) メソッドをご参照ください。

### 関連項目

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

[`LzmaArchive`](../) クラスの新しいインスタンスを初期化し、解凍のために準備します。

```csharp
public LzmaArchive(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブのソースへのパスです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| IOException | ファイルは既に開かれています。 |

## 備考

このコンストラクタは解凍しません。解凍については [`Extract`](../extract/) メソッドをご参照ください。

## 例

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
}
```

### 関連項目

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


