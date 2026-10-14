---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "IVolumeStreamProvider メソッド。分割マルチボリュームアーカイブのボリュームが書き込まれた後に呼び出されます"
type: docs
weight: 20
url: /ja/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

分割（マルチボリューム）アーカイブのボリュームが書き込まれた後に呼び出されます。

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| index | Int32 | 書き込まれたボリュームの数で、0 から始まります。 |
| s | Stream | ボリュームが書き込まれる先のストリームです。 |
| isLast | Boolean | そのボリュームがアーカイブを終了するかどうかです。 |

### 関連項目

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


