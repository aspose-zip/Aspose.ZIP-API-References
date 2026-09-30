---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CabArchive メソッド。アーカイブ内に単一のエントリを作成します。"
type: docs
weight: 40
url: /ja/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

アーカイブ内に単一のエントリを作成します。

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| path | String | 新しいファイルの完全修飾名、または圧縮対象の相対ファイル名。 |
| newEntrySettings | CabEntrySettings | 追加された [`CabEntry`](../../cabentry/) アイテムに使用される圧縮および暗号化設定。 |

### 戻り値

Cab エントリのインスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | アーカイブは抽出用に準備されており、エントリを追加できません。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*path* パラメータで指定されたファイル名はエントリ名に影響しません。

## 例

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### 関連項目

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | CabEntrySettings | 追加された [`CabEntry`](../../cabentry/) アイテムに使用される圧縮および暗号化設定。 |

### 戻り値

Cab エントリのインスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | アーカイブは抽出用に準備されており、エントリを追加できません。 |
| ArgumentNullException | *name* が null です。 |

## 例

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### 関連項目

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルのメタデータ。 |
| newEntrySettings | CabEntrySettings | 追加された [`CabEntry`](../../cabentry/) アイテムに使用される圧縮および暗号化設定。 |

### 戻り値

CAB エントリのインスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* は読み取り専用か、ディレクトリです。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| FileNotFoundException | *fileInfo* は見つからないファイルを表します。 |
| SecurityException | 呼び出し元は *fileInfo* にアクセスするための必要な権限を持っていません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | アーカイブは抽出用に準備されており、エントリを追加できません。 |
| ArgumentNullException | *name* が null です。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*fileInfo* パラメータで指定されたファイル名はエントリ名に影響しません。

## 例

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### 関連項目

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| streamProvider | Func`1 | エントリ用の入力ストリームを提供するメソッドです。 |
| newEntrySettings | CabEntrySettings | 追加された [`CabEntry`](../../cabentry/) アイテムに使用される圧縮および暗号化設定。 |

### 戻り値

CAB エントリのインスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブは解凍用にインスタンス化されています。 - または - ファイル数が上限に達しました。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentException | *name* が null または空です。 |

## 例

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### 関連項目

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


