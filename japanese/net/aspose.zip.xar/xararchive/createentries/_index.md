---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarArchive メソッド。指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します"
type: docs
weight: 30
url: /ja/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceDirectory | String | 圧縮するディレクトリ。 |
| compressionSettings | Boolean | The compression settings used for added [`XarEntry`](../../xarentry/) items. |
| includeRootDirectory | XarCompressionSettings | ルートディレクトリ自体を含めるかどうかを示します。 |

### 戻り値

Xar エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceDirectory* が null です。 |
| SecurityException | 呼び出し元は *sourceDirectory* へアクセスするための必要な権限を持っていません。 |
| ArgumentException | *sourceDirectory* に "、&lt;、&gt;、または &#x7C; のような無効な文字が含まれています。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。例えば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。指定されたパス、ファイル名、またはその両方が長すぎます。 |
| IOException | *sourceDirectory* はディレクトリではなくファイルを指します。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### 関連項目

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| directory | DirectoryInfo | 圧縮するディレクトリ。 |
| compressionSettings | Boolean | The compression settings used for added [`XarEntry`](../../xarentry/) items. |
| includeRootDirectory | XarCompressionSettings | ルートディレクトリ自体を含めるかどうかを示します。 |

### 戻り値

Xar エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *directory* は null です。 |
| SecurityException | 呼び出し元は *directory* へアクセスするための必要な権限を持っていません。 |
| IOException | *directory* はディレクトリではなくファイルを指します。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### 関連項目

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


