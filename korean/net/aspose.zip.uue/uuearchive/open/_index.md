---
title: "UueArchive.Open"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "UueArchive 메서드. 디코딩을 위해 아카이브를 열고 아카이브 내용을 포함하는 스트림을 제공합니다."
type: docs
weight: 60
url: /ko/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

디코딩을 위해 아카이브를 열고 아카이브 내용을 포함한 스트림을 제공합니다.

```csharp
public Stream Open()
```

### 반환 값

아카이브의 내용을 나타내는 스트림입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 비고

스트림에서 읽어 파일의 원본 내용을 가져옵니다. 예제 섹션을 참조하십시오.

## 예제

사용법:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 이상 - Stream.CopyTo 메서드를 사용합니다:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 및 이전 버전 - 바이트를 수동으로 복사합니다:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### 또 보기

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


