---
title: Class SevenZipCipher
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Crypto.SevenZipCipher 수업. 7zip 암호화에 사용되는 AES 암호의 기본 클래스.
type: docs
weight: 190
url: /ko/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

7-zip 암호화에 사용되는 AES 암호의 기본 클래스.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## 속성

| 이름 | 설명 |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | 현재 변환을 재사용할 수 있는지 여부를 나타내는 값을 가져옵니다. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | 여러 블록을 변환할 수 있는지 여부를 나타내는 값을 가져옵니다. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | 입력 블록 크기를 가져옵니다. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | 출력 블록 크기를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | 관리되지 않는 리소스 해제, 해제 또는 재설정과 관련된 응용 프로그램 정의 작업을 수행합니다. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | 입력 바이트 배열의 지정된 영역을 변환하고 결과 변환을 출력 바이트 배열의 지정된 영역에 복사합니다. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | 지정된 바이트 배열의 지정된 영역을 변환합니다. |

### 또한보십시오

* 네임스페이스 [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* 집회 [Aspose.Zip](../../)


