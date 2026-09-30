---
title: "SharArchive.SharArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SharArchive コンストラクタ。SharArchive クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

[`SharArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public SharArchive()
```

## 例

以下の例はファイルを圧縮する方法を示しています。

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### 関連項目

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

[`SharArchive`](../) クラスの新しいインスタンスを、解凍用に初期化します。

```csharp
public SharArchive(string path)
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
| FileNotFoundException | ファイルが見つかりません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |

### 関連項目

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


