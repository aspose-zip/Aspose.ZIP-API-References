---
title: "FastLZOutputStream"
second_title: "Aspose.ZIP for Java API 참조"
description: "FastLZ로 데이터를 압축하는 스트림 래퍼."
type: docs
weight: 68
url: /ko/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

FastLZ로 데이터를 압축하는 스트림 래퍼입니다. 데코레이터 패턴을 구현합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | 압축을 위해 준비된 FastLZStream 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | 현재 스트림을 닫고 현재 스트림과 연결된 모든 리소스(소켓 및 파일 핸들 등)를 해제합니다. |
| [flush()](#flush--) | 이 스트림의 모든 버퍼를 비우고 버퍼링된 데이터를 기본 장치에 기록하도록 합니다. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | 압축 스트림에 바이트 시퀀스를 쓰고, 쓰여진 바이트 수만큼 현재 스트림 내 위치를 이동합니다. |
| [write(int b)](#write-int-) | 지정된 바이트를 이 출력 스트림에 씁니다. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


압축을 위해 준비된 FastLZStream 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.OutputStream | 압축된 데이터를 저장하기 위한 스트림 |
| compressionLevel | int | 빠른 압축을 위해 1을 사용하고, 더 나은 압축 비율을 위해 2를 사용합니다. |

### close() {#close--}
```
public void close()
```


현재 스트림을 닫고 현재 스트림과 연결된 모든 리소스(소켓 및 파일 핸들 등)를 해제합니다.

### flush() {#flush--}
```
public void flush()
```


이 스트림의 모든 버퍼를 비우고 버퍼링된 데이터를 기본 장치에 기록하도록 합니다.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


압축 스트림에 바이트 시퀀스를 쓰고, 쓰여진 바이트 수만큼 현재 스트림 내 위치를 이동합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| buffer | byte[] | 바이트 배열입니다. 이 메서드는 buffer에서 현재 스트림으로 count 바이트를 복사합니다. |
| offset | int | buffer에서 현재 스트림으로 바이트 복사를 시작할 0 기반 바이트 오프셋 |
| count | int | 현재 스트림에 기록될 바이트 수 |

### write(int b) {#write-int-}
```
public void write(int b)
```


지정된 바이트를 이 출력 스트림에 씁니다. `write`에 대한 일반 계약은 하나의 바이트가 출력 스트림에 기록된다는 것입니다. 기록될 바이트는 인수 `b`의 하위 8비트이며, `b`의 상위 24비트는 무시됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| b | int | 해당 `byte` |

