---
title: "AppleArchive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 10
url: /tr/python-net/aspose.zip.apple/applearchive/
---

## AppleArchive class

Bu sınıf bir Apple Archive (.aar) dosyasını temsil eder. Apple Archive dosyaları oluşturmak için kullanın.

AppleArchive türü aşağıdaki üyeleri gösterir:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| AppleArchive(new_entry_settings) | [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) sınıfının yeni bir örneğini, birleştirilmiş girişler için kullanılan ayarlarla başlatır. |
| AppleArchive(source_stream, load_options) | [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
| AppleArchive(path, load_options) | [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) sınıfının yeni bir örneğini başlatır ve arşivden çıkarılabilecek bir giriş listesi oluşturur. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| girişler | Arşivi oluşturan girişleri alır. |
| is_solid | Arşivin katı sıkıştırma kullanıp kullanmadığını gösteren bir değer alır.<br/>            Katı modda, tüm giriş verileri tek bir akış olarak sıkıştırılır ve<br/>            tek tek giriş çıkarımı mevcut değildir. Kullan |
| new_entry_settings | Yeni oluşturulan girişler için kullanılan ayarları alır. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| create_entry(name, path, open_immediately) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, source) | Arşiv içinde tek bir giriş oluşturur. |
| create_entry(name, file_info, open_immediately) | Arşiv içinde tek bir giriş oluşturur. |
| save(output) | Arşivi sağlanan akışa kaydeder. |
| save(destination_file_name) | Arşivi sağlanan hedef dosyaya kaydeder. |
| create_entries(directory, include_root_directory) | Verilen dizindeki tüm dosya ve dizinleri özyinelemeli olarak arşive ekler. |
| extract_to_directory(destination_directory) | Arşivdeki tüm dosyaları sağlanan dizine çıkarır. |

### İlgili

* namespace [aspose.zip.apple](/zip/python-net/aspose.zip.apple/)
* assembly [Aspose.Zip](/zip/python-net/)

