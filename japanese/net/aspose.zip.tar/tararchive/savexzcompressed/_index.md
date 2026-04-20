---
title: TarArchive.SaveXzCompressed
second_title: Aspose.ZIP for .NET API リファレンス
description: TarArchive 方法. xz 圧縮でアーカイブをストリームに保存します
type: docs
weight: 150
url: /ja/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

xz 圧縮でアーカイブをストリームに保存します。

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| output | Stream | 宛先ストリーム。 |
| format | Nullable`1 | tar ヘッダー形式を定義します。可能な場合、NULL 値は UStar として扱われます。 |
| settings | XzArchiveSettings | 特定の xz アーカイブの設定のセット: 辞書サイズ、ブロック サイズ、チェック タイプ。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *output*無効である。 |
| ArgumentException | *output*書き込み不可です。 |

### 備考

*output*ストリームは書き込み可能である必要があります。

### 例

```csharp
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### 関連項目

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

xz 圧縮でパスごとにアーカイブをパスに保存します。

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 作成するアーカイブのパス。指定したファイル名が既存のファイルを指している場合、上書きされます。 |
| format | Nullable`1 | tar ヘッダー形式を定義します。可能な場合、NULL 値は UStar として扱われます。 |
| settings | XzArchiveSettings | 特定の xz アーカイブの設定のセット: 辞書サイズ、ブロック サイズ、チェック タイプ。 |

### 例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### 関連項目

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)


