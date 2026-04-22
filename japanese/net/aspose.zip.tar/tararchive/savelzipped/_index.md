---
title: TarArchive.SaveLzipped
second_title: Aspose.ZIP for .NET API リファレンス
description: TarArchive 方法. アーカイブを lzip 圧縮でストリームに保存します
type: docs
weight: 140
url: /ja/net/aspose.zip.tar/tararchive/savelzipped/
---
## SaveLzipped(Stream, TarFormat?) {#savelzipped}

アーカイブを lzip 圧縮でストリームに保存します。

```csharp
public void SaveLzipped(Stream output, TarFormat? format = default)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| output | Stream | 宛先ストリーム。 |
| format | Nullable`1 | tar ヘッダー形式を定義します。可能な場合、NULL 値は UStar として扱われます。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *output*無効である。 |
| ArgumentException | *output*書き込み不可です。 |

### 備考

*output*書き込み可能でなければなりません。

### 例

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### 関連項目

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SaveLzipped(string, TarFormat?) {#savelzipped_1}

アーカイブを lzip 圧縮のパスでファイルに保存します。

```csharp
public void SaveLzipped(string path, TarFormat? format = default)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 作成するアーカイブのパス。指定したファイル名が既存のファイルを指している場合、上書きされます。 |
| format | Nullable`1 | tar ヘッダー形式を定義します。可能な場合、NULL 値は UStar として扱われます。 |

### 例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.lz");
    }
}
```

### 関連項目

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)


