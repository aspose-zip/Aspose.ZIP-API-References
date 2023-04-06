---
title: Bzip2Archive.SetSource
second_title: Aspose.ZIP for .NET API リファレンス
description: Bzip2Archive 方法. アーカイブ内で圧縮するコンテンツを設定します
type: docs
weight: 60
url: /ja/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(Stream source)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブの入力ストリーム。 |

### 例

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### 関連項目

* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(FileInfo fileInfo)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| fileInfo | FileInfo | 圧縮するファイルへの参照。 |

### 例

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### 関連項目

* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 圧縮するファイルへのパス。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *path*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*path*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*path*否定された。 |
| PathTooLongException | 指定された*path*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*path*文字列の途中にコロン (:) が含まれています。 |

### 例

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### 関連項目

* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| tarArchive | TarArchive | 圧縮する tar アーカイブ。 |
| format | TarFormat | tar ヘッダー形式を定義します。 |

### 備考

この方法を使用して、共同 tar.bz2 アーカイブを構成します。

### 例

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(tarArchive);
        bzippedArchive.Save("archive.tar.bz2");
    }
}
```

### 関連項目

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| cpioArchive | CpioArchive | 圧縮する cpio アーカイブ。 |
| format | CpioFormat | cpio ヘッダー形式を定義します。 |

### 備考

このメソッドを使用して、ジョイント cpio.bz2 アーカイブを構成します。

### 例

```csharp
using (var cpioArchive = new CpioArchive())
{
    cpioArchive.CreateEntry("first.bin", "data1.bin");
    cpioArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(cpioArchive);
        bzippedArchive.Save("archive.cpio.bz2");
    }
}
```

### 関連項目

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive/)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat/)
* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)


