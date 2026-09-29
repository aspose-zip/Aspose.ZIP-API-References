---
title: "Bzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZIP 아카이브 내 Bzip2 압축에 대한 설정."
type: docs
weight: 41
url: /ko/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

ZIP 아카이브 내 Bzip2 압축에 대한 설정.

bzip2는 Burrows-Wheeler 블록 정렬 텍스트 압축 알고리즘과 Huffman 코딩을 사용하여 파일을 압축합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | 새로운 [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) 클래스 인스턴스를 초기화합니다. |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | 기본 블록 크기(9백 킬로바이트)로 새로운 [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 블록 크기(백 킬로바이트 단위). |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


새로운 [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) 클래스 인스턴스를 초기화합니다.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


블록 크기(백 킬로바이트 단위).

**Returns:**
int - 블록 크기(백 킬로바이트 단위)
