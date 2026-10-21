---
title: "GzipArchive"
second_title: "Aspose.Zip Python için .NET API Referansı"
description: 
type: docs
weight: 10
url: /tr/python-net/aspose.zip.gzip/gziparchive/
---

## GzipArchive class

Bu sınıf bir gzip arşiv dosyasını temsil eder. gzip arşivlerini oluşturmak veya çıkarmak için kullanın.

GzipArchive türü aşağıdaki üyeleri gösterir:
## Yapıcılar
| Ad | Açıklama |
| :- | :- |
| GzipArchive() | Sıkıştırma için hazırlanmış [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) sınıfının yeni bir örneğini başlatır. |
| GzipArchive(source_stream, parse_header) | Kod çözme için hazırlanmış [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) sınıfının yeni bir örneğini başlatır. |
| GzipArchive(source_stream, options) | Kod çözme için hazırlanmış [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) sınıfının yeni bir örneğini başlatır. |
| GzipArchive(path, options) | Kod çözme için hazırlanmış [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) sınıfının yeni bir örneğini başlatır. |
| GzipArchive(path, parse_header) | Kod çözme için hazırlanmış [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) sınıfının yeni bir örneğini başlatır. |
## Özellikler
| Ad | Açıklama |
| :- | :- |
| uncompressed_size | Orijinal dosyanın boyutunu alır. |
| name | Orijinal dosyanın adı. |
| file_entries | [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) türündeki arşivi oluşturan girişleri alır. |
| biçim | Arşiv biçimini alır. |
| length | Girdinin uzunluğunu bayt cinsinden alır. |
## Yöntemler
| Ad | Açıklama |
| :- | :- |
| set_source(source) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| set_source(file_info) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| set_source(path) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| set_source(tar_archive) | Arşiv içinde sıkıştırılacak içeriği ayarlar. |
| extract(destination) | Arşivi sağlanan akışa çıkarır. |
| extract(path) | Arşivin içeriğini sağlanan dizine çıkarır. |
| save(output_stream) | Arşivi sağlanan akışa kaydeder. |
| save(destination_file_name) | Arşivi sağlanan hedef dosyaya kaydeder. |
| open() | Arşivi çıkarma için açar ve arşiv içeriğiyle bir akış sağlar. |
| extract_to_directory(destination_directory) | Arşivin içeriğini sağlanan dizine çıkarır. |

### İlgili

* namespace [aspose.zip.gzip](/zip/python-net/aspose.zip.gzip/)
* assembly [Aspose.Zip](/zip/python-net/)

