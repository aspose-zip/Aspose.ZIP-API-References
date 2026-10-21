---
title: "CpioArchive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 10
url: /tr/python-net/aspose.zip.cpio/cpioarchive/
---

## CpioArchive class

Bu sınıf cpio arşiv dosyasını temsil eder.

CpioArchive türü aşağıdaki üyeleri sunar:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| CpioArchive() | Yeni bir [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) sınıfı örneği başlatır. |
| CpioArchive(source_stream) | Yeni bir [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| CpioArchive(path) | Yeni bir [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) sınıfı örneği başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| entries | [CpioEntry](/zip/python-net/aspose.zip.cpio/cpioentry/) türündeki arşivi oluşturan girdileri alır. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| create_entries(source_directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| create_entries(directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| create_entry(name, file_info, open_immediately) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source_path, open_immediately) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source) | Arşiv içinde tek bir giriş oluşturur. |
| delete_entry(entry) | Giriş listesinden belirli bir girişin ilk oluşumunu kaldırır. |
| delete_entry(entry_index) |  |
| save(destination_file_name, cpio_format) | Arşivi sağlanan hedef dosyaya kaydeder. |
| save(output, cpio_format) | Arşivi sağlanan akışa kaydeder. |
| save_gzipped(output, cpio_format) | Arşivi gzip sıkıştırmasıyla akışa kaydeder. |
| save_gzipped(path, cpio_format) | Arşivi gzip sıkıştırmasıyla belirtilen yola dosya olarak kaydeder. |
| save_lzipped(output, cpio_format) | Arşivi lzip sıkıştırmasıyla akışa kaydeder. |
| save_lzipped(path, cpio_format) | Arşivi lzip sıkıştırmasıyla belirtilen yola dosya olarak kaydeder. |
| save_lzma_compressed(output, cpio_format) | Arşivi LZMA sıkıştırmasıyla akışa kaydeder. |
| save_lzma_compressed(path, cpio_format) | Arşivi lzma sıkıştırmasıyla belirtilen yola dosya olarak kaydeder. |
| save_xz_compressed(output, cpio_format, settings) | Arşivi xz sıkıştırmasıyla akışa kaydeder. |
| save_xz_compressed(path, cpio_format, settings) | Arşivi xz sıkıştırmasıyla belirtilen yola kaydeder. |
| save_z_compressed(output, cpio_format) | Arşivi Z sıkıştırmasıyla akışa kaydeder. |
| save_z_compressed(path, cpio_format) | Arşivi Z sıkıştırmasıyla belirtilen yola kaydeder. |
| save_zstandard(output, cpio_format) | Arşivi Zstandard sıkıştırmasıyla akışa kaydeder. |
| save_zstandard(path, cpio_format) | Arşivi Zstandard sıkıştırmasıyla belirtilen dosyaya kaydeder. |
| extract_to_directory(destination_directory) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |

### İlgili

* namespace [aspose.zip.cpio](/zip/python-net/aspose.zip.cpio/)
* assembly [Aspose.Zip](/zip/python-net/)

