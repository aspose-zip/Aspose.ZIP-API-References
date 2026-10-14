---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "FastLZStream 메서드. 스트림에서 바이트 시퀀스를 읽고, 읽은 바이트 수만큼 스트림 내 위치를 이동합니다. 지원되지 않음"
type: docs
weight: 90
url: /ko/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

스트림에서 바이트 시퀀스를 읽고 읽은 바이트 수만큼 스트림 내 위치를 이동합니다. 지원되지 않음.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 버퍼 | Byte[] | 바이트 배열입니다. 이 메서드가 반환될 때, 버퍼는 지정된 바이트 배열을 포함하며, offset부터 (offset + count - 1)까지의 값은 현재 소스에서 읽은 바이트로 교체됩니다. |
| 오프셋 | Int32 | 버퍼에서 현재 스트림으로부터 읽은 데이터를 저장하기 시작할 0부터 시작하는 바이트 오프셋입니다. |
| 카운트 | Int32 | 현재 스트림에서 읽을 최대 바이트 수입니다. |

### 반환 값

버퍼에 읽힌 총 바이트 수입니다. 요청된 바이트 수보다 적을 수 있으며, 이는 해당 바이트가 현재 사용 가능하지 않거나 스트림 끝에 도달한 경우 0(0)이 될 수 있습니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| NotSupportedException | 해당 작업은 지원되지 않습니다. |

### 또 보기

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


