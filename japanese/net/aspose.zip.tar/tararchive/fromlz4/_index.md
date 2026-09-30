---
title: "TarArchive.FromLZ4"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。指定された LZ4 アーカイブを展開し、抽出されたデータから TarArchive を作成します"
type: docs
weight: 30
url: /ja/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

指定された LZ4 アーカイブを展開し、抽出されたデータから [`TarArchive`](../) を作成します。

重要: このメソッド内で LZ4 アーカイブは完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | 呼び出し元にアクセスに必要な権限がありません |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイルは無効な形式です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| EndOfStreamException | ファイルが短すぎます。 |
| InvalidDataException | ファイルのシグネチャが正しくありません。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |
| InvalidOperationException | アーカイブは構成のために準備されています。 |

## 備考

LZ4 抽出ストリームは圧縮アルゴリズムの特性上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部的にシーク可能なストリームで動作する必要があります。

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

指定された LZ4 アーカイブを展開し、抽出されたデータから [`TarArchive`](../) を作成します。

重要: このメソッド内で LZ4 アーカイブは完全に展開され、内容は内部に保持されます。メモリ使用量に注意してください。

```csharp
public static TarArchive FromLZ4(Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソースです。 |

### 戻り値

[`TarArchive`](../) のインスタンス

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *source* から読み取れません |
| ArgumentNullException | *source* が null です。 |
| EndOfStreamException | *source* が短すぎます。 |
| InvalidDataException | *source* のシグネチャが正しくありません。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 備考

LZ4 抽出ストリームは圧縮アルゴリズムの特性上シーク可能ではありません。Tar アーカイブは任意のレコードを抽出する機能を提供するため、内部的にシーク可能なストリームで動作する必要があります。

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


