---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "XarBzip2CompressionSettings 생성자. XarBzip2CompressionSettings 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

[`XarBzip2CompressionSettings`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| blockSize | Int32 | 블록 크기(백 킬로바이트 단위). |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentOutOfRangeException | 블록 크기가 1과 9 사이가 아닙니다. |

## 예제

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### 또 보기

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

[`XarBzip2CompressionSettings`](../) 클래스의 새 인스턴스를 기본 블록 크기로 초기화합니다. 기본 블록 크기는 9백 킬로바이트와 같습니다.

```csharp
public XarBzip2CompressionSettings()
```

### 또 보기

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


