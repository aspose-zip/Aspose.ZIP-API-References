---
title: "クラス XzArchiveSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Xz.Settings.XzArchiveSettings クラス。このクラスは特定の xz アーカイブの設定セットを含みます"
type: docs
weight: 1520
url: /ja/net/aspose.zip.xz.settings/xzarchivesettings/
---
## XzArchiveSettings class

このクラスは特定の xz アーカイブの設定セットを含みます。

```csharp
public class XzArchiveSettings
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [XzArchiveSettings](xzarchivesettings/#constructor)() | `XzArchiveSettings` クラスの新しいインスタンスを、単一の LZMA2 圧縮を使用して初期化します。 |
| [XzArchiveSettings](xzarchivesettings/#constructor_1)(XzFilterSettings[], long, XzCheckType) | `XzArchiveSettings` クラスの新しいインスタンスをカスタム パラメータで初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| static [FastestSpeed](../../aspose.zip.xz.settings/xzarchivesettings/fastestspeed/) { get; } | `XzArchiveSettings` クラスのインスタンスを取得します（辞書サイズが 65536 バイト、LZMA2 フィルタ、ブロックサイズが 1 メガバイト、CRC32 チェックサム）。 |
| static [FastSpeed](../../aspose.zip.xz.settings/xzarchivesettings/fastspeed/) { get; } | `XzArchiveSettings` クラスのインスタンスを取得します（辞書サイズが 1 メガバイト、LZMA2 フィルタ、ブロックサイズが 4 メガバイト、CRC32 チェックサム）。 |
| static [HighCompression](../../aspose.zip.xz.settings/xzarchivesettings/highcompression/) { get; } | `XzArchiveSettings` クラスのインスタンスを取得します（辞書サイズが 32 メガバイト、LZMA2 フィルタ、ブロックサイズが 128 メガバイト、CRC32 チェックサム）。 |
| static [MaximumCompression](../../aspose.zip.xz.settings/xzarchivesettings/maximumcompression/) { get; } | `XzArchiveSettings` クラスのインスタンスを取得します（辞書サイズが 64 メガバイト、LZMA2 フィルタ、ブロックサイズが 256 メガバイト、CRC32 チェックサム）。 |
| static [Normal](../../aspose.zip.xz.settings/xzarchivesettings/normal/) { get; } | `XzArchiveSettings` クラスのインスタンスを取得します（辞書サイズが 16 メガバイト、LZMA2 フィルタ、ブロックサイズが 64 メガバイト、CRC32 チェックサム）。 |
| [CompressionThreads](../../aspose.zip.xz.settings/xzarchivesettings/compressionthreads/) { get; set; } | 圧縮スレッド数を取得または設定します。値が 1 より大きい場合、マルチスレッド圧縮が使用されます。 |

### 関連項目

* namespace [Aspose.Zip.Xz.Settings](../../aspose.zip.xz.settings/)
* assembly [Aspose.Zip](../../)


