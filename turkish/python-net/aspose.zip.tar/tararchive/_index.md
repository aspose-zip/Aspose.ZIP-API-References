---
title: "TarArchive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 10
url: /tr/python-net/aspose.zip.tar/tararchive/
---

## TarArchive class

Bu sınıf bir tar arşiv dosyasını temsil eder. tar arşivlerini oluşturmak, çıkarmak veya güncellemek için kullanın.

TarArchive türü aşağıdaki üyeleri sunar:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| TarArchive() | [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) sınıfının yeni bir örneğini başlatır. |
| TarArchive(source_stream) | Arşivden çıkarılabilecek bir giriş listesi oluşturan [Archive](/zip/python-net/aspose.zip/archive/) sınıfının yeni bir örneğini başlatır. |
| TarArchive(path) | [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| entries | Arşivi oluşturan [TarEntry](/zip/python-net/aspose.zip.tar/tarentry/) türündeki girişleri alır. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| create_entry(name, source, file_info) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, file_info, open_immediately) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, path, open_immediately) | Arşiv içinde tek bir giriş oluşturur. |
| create_entries(directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| create_entries(source_directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| delete_entry(entry) | Giriş listesinden belirli bir girişin ilk oluşumunu kaldırır. |
| delete_entry(entry_index) |  |
| save(output, format) |  |
| save(destination_file_name, format) |  |
| save_gzipped(output, format) |  |
| save_gzipped(path, format) |  |
| save_zstandard(output, format) |  |
| save_zstandard(path, format) |  |
| save_lzipped(output, format) |  |
| save_lzipped(path, format) |  |
| save_lzma_compressed(output, format) |  |
| save_lzma_compressed(path, format) |  |
| save_lz4_compressed(output, format) |  |
| save_lz4_compressed(path, format) |  |
| save_xz_compressed(output, format, settings) |  |
| save_xz_compressed(path, format, settings) |  |
| save_z_compressed(output, format) |  |
| save_z_compressed(path, format) |  |
| from_g_zip(source) | Sağlanan gzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_g_zip(path) | Sağlanan gzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_zstandard(source) | Sağlanan Zstandard arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_zstandard(path) | Sağlanan Zstandard arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_l_zip(source) | Sağlanan lzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_l_zip(path) | Sağlanan lzip arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_lzma(source) | Sağlanan LZMA arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_lzma(path) | Sağlanan LZMA arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_lz4(path) | Sağlanan LZ4 arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_lz4(source) | Sağlanan LZ4 arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_xz(source) | Sağlanan xz format arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_xz(path) | Sağlanan xz format arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_z(source) | Sağlanan Zstandard arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| from_z(path) | Sağlanan Zstandard arşivini çıkarır ve çıkarılan verilerden [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) oluşturur. |
| extract_to_directory(destination_directory) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |

### İlgili

* namespace [aspose.zip.tar](/zip/python-net/aspose.zip.tar/)
* assembly [Aspose.Zip](/zip/python-net/)

