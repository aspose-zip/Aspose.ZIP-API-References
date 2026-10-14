---
title: "AppleArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file Apple Archive .aar."
type: docs
weight: 16
url: /id/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Kelas ini mewakili file Apple Archive (.aar). Gunakan untuk menyusun file Apple Archive.

Apple dan Apple Archive adalah merek dagang Apple Inc.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dengan pengaturan yang digunakan untuk entri yang disusun. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dengan pengaturan yang digunakan untuk entri yang disusun. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Membuat satu entri dalam arsip. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Membuat satu entri dalam arsip. |
| [dispose()](#dispose--) | Melakukan tugas yang ditentukan aplikasi yang terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [getEntries()](#getEntries--) | Mendapatkan entri yang membentuk arsip. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Mendapatkan pengaturan yang digunakan untuk entri yang baru disusun. |
| [isSolid()](#isSolid--) | Mendapatkan nilai yang menunjukkan apakah arsip menggunakan kompresi solid. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Menyimpan arsip ke aliran yang disediakan. |
| [save(String destinationFileName)](#save-java.lang.String-) | Menyimpan arsip ke file tujuan yang disediakan. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dengan pengaturan yang digunakan untuk entri yang disusun.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dengan pengaturan yang digunakan untuk entri yang disusun.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Pengaturan yang digunakan saat menyusun Apple Archive baru. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | Sumber arsip. |

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) dan [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) untuk mendekompresi. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Sumber arsip. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Opsi untuk memuat arsip yang ada. |

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) dan [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) untuk mendekompresi. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | path | java.lang.String | Jalur lengkap atau jalur relatif ke file arsip. |

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) dan [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) untuk mendekompresi. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [AppleArchive](../../com.aspose.zip/applearchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Jalur lengkap atau jalur relatif ke file arsip. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Opsi untuk memuat arsip yang ada. |

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) dan [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) untuk mendekompresi. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| direktori | java.io.File | Direktori untuk dikompres. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| direktori | java.io.File | Direktori untuk dikompres. |
| includeRootDirectory | boolean | Menunjukkan apakah akan menyertakan direktori root itu sendiri atau tidak. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Membuat satu entri dalam arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | Nama entri. |
| fileInfo | java.io.File | Metadata file yang akan dikompres. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Membuat satu entri dalam arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | Nama entri. |
| fileInfo | java.io.File | Metadata file yang akan dikompres. |
| openImmediately | boolean | True, jika membuka file segera, jika tidak membuka file saat penyimpanan arsip. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Membuat satu entri dalam arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | Nama entri. |
| source | java.io.InputStream | Aliran input untuk entri. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Membuat satu entri dalam arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | Nama entri. |
| path | java.lang.String | Jalur ke file yang akan dikompres. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Membuat satu entri dalam arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String | Nama entri. |
| path | java.lang.String | Jalur ke file yang akan dikompres. |
| openImmediately | boolean | True, jika membuka file segera, jika tidak membuka file saat penyimpanan arsip. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Melakukan tugas yang ditentukan aplikasi yang terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mengekstrak semua file dalam arsip ke direktori yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Jalur ke direktori tempat menempatkan file yang diekstrak. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Mendapatkan entri yang membentuk arsip.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - entri yang membentuk arsip.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Mendapatkan format arsip.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Mendapatkan pengaturan yang digunakan untuk entri yang baru disusun.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Mendapatkan nilai yang menunjukkan apakah arsip menggunakan kompresi solid. Dalam mode solid, semua data entri dikompresi sebagai satu aliran dan ekstraksi entri individual tidak tersedia. Gunakan [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--) sebagai gantinya.

**Returns:**
boolean - nilai yang menunjukkan apakah arsip menggunakan kompresi solid.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Menyimpan arsip ke aliran yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | output | java.io.OutputStream | Aliran tujuan. |

`output` harus dapat ditulis. Beberapa pengaturan kompresi, seperti LZ4, juga memerlukan aliran yang dapat dicari. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Menyimpan arsip ke file tujuan yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | java.lang.String | Jalur arsip yang akan dibuat. |

