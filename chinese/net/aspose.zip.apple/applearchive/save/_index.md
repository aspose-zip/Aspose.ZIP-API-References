---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AppleArchive 方法。将存档保存到提供的流中"
type: docs
weight: 90
url: /zh/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

将存档保存到提供的流中。

```csharp
public void Save(Stream output)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | 流 | 目标流。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放。 |
| ArgumentNullException | *output* 为 `null`。 |
| ArgumentException | *output* 不可写。 |
| ArgumentOutOfRangeException | 配置的 LZ4 或 Zlib 块大小不是正数。 |
| NotSupportedException | 压缩设置缺失或不受支持，直接组成使用不可定位的流，或条目/存档大小超出当前 Apple Archive 限制。 |

## 备注

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### 另请参阅

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

将存档保存到提供的目标文件中。

```csharp
public void Save(string destinationFileName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | String | 要创建的存档的路径。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放。 |
| ArgumentException | *destinationFileName* 无效。 |
| ArgumentNullException | *destinationFileName* 为 `null`。 |
| ArgumentOutOfRangeException | 配置的 LZ4 或 Zlib 块大小不是正数。 |
| NotSupportedException | 压缩设置缺失或不受支持，直接组成使用不可定位的流，或条目/存档大小超出当前 Apple Archive 限制。 |

### 另请参阅

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


