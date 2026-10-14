---
title: "GzipArchive.SetSource"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "GzipArchive メソッド。アーカイブ内で圧縮されるコンテンツを設定します"
type: docs
weight: 90
url: /ja/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

アーカイブ内で圧縮される内容を設定します。

```csharp
public void SetSource(Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブ用の入力ストリームです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

アーカイブ内で圧縮される内容を設定します。

```csharp
public void SetSource(FileInfo fileInfo)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileInfo | FileInfo | 圧縮対象のファイルへの参照です。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

アーカイブ内で圧縮される内容を設定します。

```csharp
public void SetSource(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 圧縮対象ファイルへのパス。 |

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

## 例

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

アーカイブ内で圧縮される内容を設定します。

```csharp
public void SetSource(TarArchive tarArchive)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| tarArchive | TarArchive | 圧縮対象の Tar アーカイブ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

このメソッドを使用して結合された tar.gz アーカイブを作成します。

## 例

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### 関連項目

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


