---
title: XzArchive.XzArchive
second_title: Aspose.ZIP for .NET API 参考
description: XzArchive 构造函数. 初始化一个新的实例XzArchive类并以 xz 格式组成存档
type: docs
weight: 10
url: /zh/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

初始化一个新的实例[`XzArchive`](../)类并以 xz 格式组成存档。

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| settings | XzArchiveSettings | 一组设置特定的 xz 存档：字典大小、块大小、检查类型。 |

### 也可以看看

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* 命名空间 [Aspose.Zip.Xz](../../xzarchive/)
* 部件 [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

初始化一个新的实例[`XzArchive`](../)准备解压的类.

```csharp
public XzArchive(Stream source)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| source | Stream | 存档的来源。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | *source*不可搜索。 |
| ArgumentNullException | *source*一片空白。 |

### 评论

此构造函数不解压缩。看[`Extract`](../extract/)解压方法.

### 也可以看看

* class [XzArchive](../)
* 命名空间 [Aspose.Zip.Xz](../../xzarchive/)
* 部件 [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

初始化一个新的实例[`XzArchive`](../)准备解压的类.

```csharp
public XzArchive(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 存档源的路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*path*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*path*被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*path*在字符串中间包含一个冒号 (:)。 |

### 评论

此构造函数不解压缩。看[`Extract`](../extract/)解压方法.

### 也可以看看

* class [XzArchive](../)
* 命名空间 [Aspose.Zip.Xz](../../xzarchive/)
* 部件 [Aspose.Zip](../../../)


