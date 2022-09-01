---
title: ZArchive
second_title: Aspose.ZIP for .NET API 参考
description: 初始化准备压缩的ZArchiveaspose.zip.z/zarchive类的新实例
type: docs
weight: 10
url: /zh/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

初始化准备压缩的[`ZArchive`](../../zarchive)类的新实例。

```csharp
public ZArchive()
```

### 也可以看看

* class [ZArchive](../../zarchive)
* 命名空间 [Aspose.Zip.Z](../../zarchive)
* 部件 [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

初始化准备解压缩的[`ZArchive`](../../zarchive)类的新实例。

```csharp
public ZArchive(Stream source)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| source | Stream | 存档的来源。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentException | *source*不可搜索。 |
| ArgumentNullException | *source*为空。 |

### 评论

此构造函数不解压缩。请参阅[`Extract`](../extract)解压方法。

### 也可以看看

* class [ZArchive](../../zarchive)
* 命名空间 [Aspose.Zip.Z](../../zarchive)
* 部件 [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

初始化准备解压缩的[`ZArchive`](../../zarchive)类的新实例。

```csharp
public ZArchive(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 存档源的路径。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *path*为空。 |
| SecurityException | 调用者没有访问所需的权限 |
| ArgumentException | *path*为空，仅包含空格，或包含无效字符。 |
| UnauthorizedAccessException | 对文件*path*的访问被拒绝。 |
| PathTooLongException | 指定的*path*、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | *path*的文件在字符串中间包含一个冒号 (:)。 |

### 评论

此构造函数不解压缩。请参阅[`Extract`](../extract)解压方法。

### 也可以看看

* class [ZArchive](../../zarchive)
* 命名空间 [Aspose.Zip.Z](../../zarchive)
* 部件 [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->