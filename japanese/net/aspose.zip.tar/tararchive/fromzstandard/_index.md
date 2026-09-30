---
title: "TarArchive.FromZstandard"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。提供された Zstandard アーカイブを抽出し、抽出されたデータから TarArchive を構成します"
type: docs
weight: 80
url: /ja/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

提供された Zstandard アーカイブを抽出し、抽出されたデータから [`TarArchive`](../) を構成します。

重要: このメソッド内で Zstandard アーカイブは完全に抽出され、その内容は内部に保持されます。メモリ使用量に注意してください。

```csharp
public static TarArchive FromZstandard(Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソースです。 |

### 戻り値

[`TarArchive`](../) のインスタンス

### 例外

| 例外 | 条件 |
| --- | --- |
| IOException | Zstandard ストリームが破損しているか、読み取れません。 |
| InvalidDataException | データが破損しています。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

提供された Zstandard アーカイブを抽出し、抽出されたデータから [`TarArchive`](../) を構成します。

重要: このメソッド内で Zstandard アーカイブは完全に抽出され、その内容は内部に保持されます。メモリ使用量に注意してください。

```csharp
public static TarArchive FromZstandard(string path)
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
| IOException | Zstandard ストリームが破損しているか、読み取れません。 |
| InvalidDataException | データが破損しています。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


