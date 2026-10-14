---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "FastLZStream 생성자. 압축을 위해 준비된 FastLZStream 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

압축을 위해 준비된 [`FastLZStream`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 압축 데이터를 저장하기 위한 스트림입니다. |
| compressionLevel | Int32 | 더 빠른 압축을 위해 1을 사용하고, 더 나은 압축 비율을 위해 2를 사용합니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *stream*이 null입니다. |
| ArgumentException | *stream*은(는) 쓰기를 지원하지 않습니다. |
| ArgumentOutOfRangeException | *compressionLevel*은(는) 2보다 크거나 1보다 작습니다. |

### 또 보기

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


