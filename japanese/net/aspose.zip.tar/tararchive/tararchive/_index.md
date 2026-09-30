---
title: "TarArchive.TarArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive コンストラクタ。TarArchive クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

[`TarArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public TarArchive()
```

## 例

以下の例はファイルを圧縮する方法を示しています。

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(Stream, TarLoadOptions) {#constructor_1}

[`TarArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public TarArchive(Stream sourceStream, TarLoadOptions loadOptions = null)
```

| パラメーター | 説明 |
| --- | --- |
| sourceStream | アーカイブのソースです。シーク可能である必要があります。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| ArgumentNullException | *sourceStream* が null です。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Open`](../../tarentry/open/) メソッドをご覧ください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 関連項目

* class [TarLoadOptions](../../tarloadoptions/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(string, TarLoadOptions) {#constructor_2}

[`TarArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public TarArchive(string path, TarLoadOptions loadOptions = null)
```

| パラメーター | 説明 |
| --- | --- |
| path | アーカイブ ファイルへのパス。 |

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
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Open`](../../tarentry/open/) メソッドをご覧ください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new TarArchive("archive.tar", new TarLoadOptions() { CancellationToken = cancellationToken }))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 関連項目

* class [TarLoadOptions](../../tarloadoptions/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


