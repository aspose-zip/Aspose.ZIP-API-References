---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarArchive メソッド。アーカイブ内に単一のエントリを作成します"
type: docs
weight: 40
url: /ja/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |
| compressionSettings | XarCompressionSettings | 追加された [`XarEntry`](../../xarentry/) アイテムに使用される圧縮設定です。 |

### 戻り値

Xar エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *name* が null です。 |
| ArgumentException | *name* が空です。 |
| ArgumentNullException | *fileInfo* が null です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが破棄されるまでブロックされます。

## 例

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### 関連項目

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| sourcePath | String | 圧縮対象ファイルへのパス。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |
| compressionSettings | XarCompressionSettings | 追加された [`XarEntry`](../../xarentry/) アイテムに使用される圧縮設定です。 |

### 戻り値

Xar エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourcePath* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *sourcePath* が空、または空白のみ、または無効な文字が含まれています。 - または - *name* の一部であるファイル名が 100 文字を超えています。 |
| UnauthorizedAccessException | *sourcePath* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *sourcePath*、ファイル名、またはその両方がシステム定義の最大長を超えています。例えば、Windows プラットフォームではパスは 248 文字未満、ファイル名は 260 文字未満である必要があります。- または - *name* が xar に対して長すぎます。 |
| NotSupportedException | *sourcePath* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| InvalidOperationException | xar アーカイブを変更できません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*sourcePath* パラメータで提供されたファイル名はエントリ名に影響しません。

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが破棄されるまでブロックされます。

## 例

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### 関連項目

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| compressionSettings | XarCompressionSettings | 追加された [`XarEntry`](../../xarentry/) アイテムに使用される圧縮設定です。 |

### 戻り値

Xar エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *name* が null です。 |
| ArgumentNullException | *source* が null です。 |
| ArgumentException | *name* が空です。 |
| InvalidOperationException | xar アーカイブを変更できません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### 関連項目

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


