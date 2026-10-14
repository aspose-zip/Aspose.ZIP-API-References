---
title: "SevenZipCipher"
second_title: "Aspose.ZIP for Java API 참조"
description: "7-zip 암호화에 사용되는 AES 암호에 대한 기본 클래스."
type: docs
weight: 110
url: /ko/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

7-zip 암호화에 사용되는 AES 암호에 대한 기본 클래스.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | 현재 변환을 재사용할 수 있는지 여부를 나타내는 값을 가져옵니다. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | 여러 블록을 변환할 수 있는지 여부를 나타내는 값을 가져옵니다. |
| [dispose()](#dispose--) | 관리되지 않는 리소스를 해제하거나, 릴리스하거나, 재설정하는 애플리케이션 정의 작업을 수행합니다. |
| [getInputBlockSize()](#getInputBlockSize--) | 입력 블록 크기를 가져옵니다. |
| [getOutputBlockSize()](#getOutputBlockSize--) | 출력 블록 크기를 가져옵니다. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | 입력 바이트 배열의 지정된 영역을 변환하고, 결과 변환을 출력 바이트 배열의 지정된 영역에 복사합니다. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | 지정된 바이트 배열의 지정된 영역을 변환합니다. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


현재 변환을 재사용할 수 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 현재 변환을 재사용할 수 있는지 여부를 나타내는 값
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


여러 블록을 변환할 수 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 여러 블록을 변환할 수 있는지 여부를 나타내는 값
### dispose() {#dispose--}
```
public abstract void dispose()
```


관리되지 않는 리소스를 해제하거나, 릴리스하거나, 재설정하는 애플리케이션 정의 작업을 수행합니다.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


입력 블록 크기를 가져옵니다.

**Returns:**
int - 입력 블록 크기
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


출력 블록 크기를 가져옵니다.

**Returns:**
int - 출력 블록 크기
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


입력 바이트 배열의 지정된 영역을 변환하고, 결과 변환을 출력 바이트 배열의 지정된 영역에 복사합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inputBuffer | byte[] | 변환을 계산할 입력 |
| inputOffset | int | 데이터 사용을 시작할 입력 바이트 배열의 오프셋 |
| inputCount | int | 데이터로 사용할 입력 바이트 배열의 바이트 수 |
| outputBuffer | byte[] | 변환을 기록할 출력 |
| outputOffset | int | 데이터 쓰기를 시작할 출력 바이트 배열의 오프셋 |

**Returns:**
int - 기록된 바이트 수
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


지정된 바이트 배열의 지정된 영역을 변환합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inputBuffer | byte[] | 변환을 계산할 입력 |
| inputOffset | int | 데이터 사용을 시작할 입력 바이트 배열의 오프셋 |
| inputCount | int | 데이터로 사용할 입력 바이트 배열의 바이트 수 |

**Returns:**
byte[] - 계산된 변환
