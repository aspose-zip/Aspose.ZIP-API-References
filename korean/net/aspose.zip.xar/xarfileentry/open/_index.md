---
title: XarFileEntry.Open
second_title: .NET API 참조용 Aspose.ZIP
description: XarFileEntry 방법. 추출할 항목을 열고 항목 내용이 있는 스트림을 제공합니다.
type: docs
weight: 30
url: /ko/net/aspose.zip.xar/xarfileentry/open/
---
## XarFileEntry.Open method

추출할 항목을 열고 항목 내용이 있는 스트림을 제공합니다.

```csharp
public abstract Stream Open()
```

### 반환 값

항목의 내용을 나타내는 스트림입니다.

### 비고

파일의 원래 내용을 가져오기 위해 스트림에서 읽습니다. 예제 섹션을 참조하십시오.

### 예

사용법:

.NET 4.0 이상 - Stream.CopyTo 메서드 사용:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 이전 - 수동으로 바이트 복사:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### 또한보십시오

* class [XarFileEntry](../)
* 네임스페이스 [Aspose.Zip.Xar](../../xarfileentry/)
* 집회 [Aspose.Zip](../../../)


