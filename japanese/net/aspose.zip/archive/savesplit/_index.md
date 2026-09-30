---
title: "Archive.SaveSplit"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Archive メソッド。提供された宛先ディレクトリにマルチボリュームアーカイブを保存します。"
type: docs
weight: 110
url: /ja/net/aspose.zip/archive/savesplit/
---
## SaveSplit(string, SplitArchiveSaveOptions) {#savesplit_1}

指定された宛先ディレクトリにマルチボリューム アーカイブを保存します。

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | String | アーカイブセグメントが作成されるディレクトリへのパス。 |
| オプション | SplitArchiveSaveOptions | ファイル名を含む、アーカイブ保存のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | このアーカイブは既存のソースから開かれました。 |
| NotSupportedException | このアーカイブは XZ 方式で圧縮され、かつ暗号化されています。 |
| ArgumentNullException | *destinationDirectory* が null です。 |
| SecurityException | 呼び出し元にディレクトリへアクセスするための必要な権限がありません。 |
| ArgumentException | *destinationDirectory* に \"、&gt;、&lt;、または &#x7C; などの無効な文字が含まれています。 |
| PathTooLongException | 指定されたパスがシステム定義の最大長を超えています。 |
| ObjectDisposedException | アーカイブは破棄されました。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |

## 備考

このメソッドは複数の (`n`) ファイル filename.z01, filename.z02, ..., filename.z(n-1), filename.zip を構成します。

既存のアーカイブをマルチボリュームにすることはできません。

## 例

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### 関連項目

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## SaveSplit(IVolumeStreamProvider, SplitArchiveSaveOptions) {#savesplit}

ボリュームプロバイダーが提供するストリームにマルチボリューム アーカイブを保存します。

```csharp
public void SaveSplit(IVolumeStreamProvider volumeStreamProvider, SplitArchiveSaveOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| volumeStreamProvider | IVolumeStreamProvider | アーカイブボリューム用の宛先ストリームのプロバイダーです。 |
| options | SplitArchiveSaveOptions | アーカイブ保存のオプションです。[`FileName`](../../../aspose.zip.saving/splitarchivesaveoptions/filename/) は無視されます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *volumeStreamProvider* または *options* が null です。 |
| InvalidOperationException | このアーカイブは既存のソースから開かれたか、プロバイダーが null または書き込み不可のストリームを返しました。 |
| NotSupportedException | アーカイブは XZ 圧縮を使用しています。 |
| ObjectDisposedException | アーカイブは破棄されました。 |

## 備考

提供されたストリームはシークをサポートする必要はありません。

完了した各ボリュームはフラッシュされ、[`VolumeCompleted`](../../../aspose.zip.saving/ivolumestreamprovider/volumecompleted/) に渡され、その後破棄されます。

既存のアーカイブをマルチボリュームにすることはできません。このオーバーロードでは XZ 圧縮はシークが必要なためサポートされていません。

## 例

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(provider,  new SplitArchiveSaveOptions("volume", 65536));
}
```

### 関連項目

* interface [IVolumeStreamProvider](../../../aspose.zip.saving/ivolumestreamprovider/)
* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


