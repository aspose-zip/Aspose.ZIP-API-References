---
title: "LzipArchive.LzipArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzipArchive コンストラクタ。LzipArchive の新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

[`LzipArchive`](../) の新しいインスタンスを初期化します。

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 設定 | LzipArchiveSettings | 特定の lzip アーカイブの設定で、辞書サイズを定義します。 |

### 関連項目

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(Stream, LzipLoadOptions) {#constructor_1}

[`LzipArchive`](../) クラスの新しいインスタンスを初期化し、解凍のために準備します。

```csharp
public LzipArchive(Stream sourceStream, LzipLoadOptions options = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| オプション | LzipLoadOptions | アーカイブを読み込む際のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| ArgumentNullException | *sourceStream* が null です。 |
| InvalidDataException | ヘッダーが lzip タイプのアーカイブと一致しません。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| IOException | I/O エラーが発生しました。 |

## 備考

このコンストラクタは解凍しません。解凍については [`Extract`](../extract/) メソッドをご参照ください。

### 関連項目

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(string, LzipLoadOptions) {#constructor_2}

[`LzipArchive`](../) クラスの新しいインスタンスを初期化し、解凍のために準備します。

```csharp
public LzipArchive(string path, LzipLoadOptions options = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブのソースへのパスです。 |
| オプション | LzipLoadOptions | アーカイブを読み込む際のオプション。 |

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
| InvalidDataException | ヘッダーが lzip タイプのアーカイブと一致しません。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |

## 備考

このコンストラクタは解凍しません。解凍については [`Extract`](../extract/) メソッドをご参照ください。

## 例

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### 関連項目

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


