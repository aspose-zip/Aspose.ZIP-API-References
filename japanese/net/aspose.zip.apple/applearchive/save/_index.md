---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AppleArchive メソッド。提供されたストリームにアーカイブを保存します"
type: docs
weight: 90
url: /ja/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

アーカイブを指定されたストリームに保存します。

```csharp
public void Save(Stream output)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されました。 |
| ArgumentNullException | *output* は `null` です。 |
| ArgumentException | *output* は書き込み可能ではありません。 |
| ArgumentOutOfRangeException | 設定された LZ4 または Zlib のブロックサイズが正の値ではありません。 |
| NotSupportedException | 圧縮設定が欠如しているかサポートされていません、直接構成がシーク不可のストリームを使用している、またはエントリ/アーカイブのサイズが現在の Apple Archive の制限を超えています。 |

## 備考

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### 関連項目

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

提供された宛先ファイルにアーカイブを保存します。

```csharp
public void Save(string destinationFileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパスです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されました。 |
| ArgumentException | *destinationFileName* が無効です。 |
| ArgumentNullException | *destinationFileName* は `null` です。 |
| ArgumentOutOfRangeException | 設定された LZ4 または Zlib のブロックサイズが正の値ではありません。 |
| NotSupportedException | 圧縮設定が欠如しているかサポートされていません、直接構成がシーク不可のストリームを使用している、またはエントリ/アーカイブのサイズが現在の Apple Archive の制限を超えています。 |

### 関連項目

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


