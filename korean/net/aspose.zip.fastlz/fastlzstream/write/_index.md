---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "FastLZStream 메서드. 바이트 시퀀스를 압축 스트림에 쓰고, 쓰여진 바이트 수만큼 현재 스트림 내 위치를 이동합니다"
type: docs
weight: 120
url: /ko/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

압축 스트림에 바이트 시퀀스를 쓰고 쓰여진 바이트 수만큼 현재 스트림 내 위치를 이동합니다.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 버퍼 | Byte[] | 바이트 배열입니다. 이 메서드는 버퍼에서 현재 스트림으로 count 바이트를 복사합니다. |
| 오프셋 | Int32 | 버퍼에서 현재 스트림으로 바이트 복사를 시작할 0부터 시작하는 바이트 오프셋입니다. |
| 카운트 | Int32 | 현재 스트림에 기록될 바이트 수입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 스트림이 해제된 경우 발생합니다. |
| ArgumentNullException | *buffer*는 `null`입니다. |

### 또 보기

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


