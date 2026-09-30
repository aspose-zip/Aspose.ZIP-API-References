---
title: "클래스 FastLZStream"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.FastLZ.FastLZStream 클래스. FastLZ로 데이터를 압축하는 스트림 래퍼입니다. 데코레이터 패턴을 구현합니다."
type: docs
weight: 500
url: /ko/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

FastLZ로 데이터를 압축하는 스트림 래퍼입니다. 데코레이터 패턴을 구현합니다.

```csharp
public class FastLZStream : Stream
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | `FastLZStream` 클래스의 새 인스턴스를 초기화하여 압축을 준비합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | 현재 스트림이 읽기를 지원하는지 여부를 나타내는 값을 가져옵니다. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | 현재 스트림이 탐색을 지원하는지 여부를 나타내는 값을 가져옵니다. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | 현재 스트림이 쓰기를 지원하는지 여부를 나타내는 값을 가져옵니다. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | 스트림의 길이(바이트)를 가져옵니다. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | 현재 스트림 내의 위치를 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | 현재 스트림을 닫고 현재 스트림과 연결된 모든 리소스(소켓 및 파일 핸들 등)를 해제합니다. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | 이 스트림의 모든 버퍼를 비우고 버퍼링된 데이터를 기본 장치에 기록하도록 합니다. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | 스트림에서 바이트 시퀀스를 읽고 읽은 바이트 수만큼 스트림 내 위치를 이동합니다. 지원되지 않음. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | 현재 스트림 내의 위치를 설정합니다. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | 현재 스트림의 길이를 설정합니다. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | 압축 스트림에 바이트 시퀀스를 쓰고 쓰여진 바이트 수만큼 현재 스트림 내 위치를 이동합니다. |

### 또 보기

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


