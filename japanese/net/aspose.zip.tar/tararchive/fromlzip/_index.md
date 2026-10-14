---
title: "TarArchive.FromLZip"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。提供された lzip アーカイブを抽出し、抽出されたデータから TarArchive を構成します"
type: docs
weight: 40
url: /ja/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

提供された lzip アーカイブを抽出し、抽出されたデータから [`TarArchive`](../) を構成します。

重要: このメソッド内で lzip アーカイブは完全に展開され、その内容は内部に保持されます。メモリ使用量に注意してください。

```csharp
public static TarArchive FromLZip(Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソースです。 |

### 戻り値

[`TarArchive`](../) のインスタンス

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidDataException | アーカイブが破損しています。 |
| ArgumentException | *source* はシーク可能ではありません。 |
| ArgumentNullException | *source* が null です。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| IOException | I/O エラーが発生しました。 |
| InvalidOperationException | アーカイブヘッダーとサービス情報は読み取られませんでした。 |

## 備考

圧縮アルゴリズムの特性上、Lzip 抽出ストリームはシーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを使用して動作する必要があります。

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

提供された lzip アーカイブを抽出し、抽出されたデータから [`TarArchive`](../) を構成します。

重要: このメソッド内で lzip アーカイブは完全に展開され、その内容は内部に保持されます。メモリ使用量に注意してください。

```csharp
public static TarArchive FromLZip(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |

### 戻り値

[`TarArchive`](../) のインスタンス

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイルは無効な形式です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| InvalidDataException | アーカイブが破損しています。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| IOException | I/O エラーが発生しました。 |
| InvalidOperationException | アーカイブヘッダーとサービス情報は読み取られませんでした。 |

## 備考

圧縮アルゴリズムの特性上、Lzip 抽出ストリームはシーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部ではシーク可能なストリームを使用して動作する必要があります。

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


