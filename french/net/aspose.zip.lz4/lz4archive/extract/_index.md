---
title: "Lz4Archive.Extract"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode Lz4Archive. Extrait l'archive vers le fichier selon le chemin"
type: docs
weight: 30
url: /fr/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Extrait l'archive vers le fichier par chemin.

```csharp
public FileInfo Extract(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

### Valeur de retour

Info d'un fichier extrait.

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Le flux source est trop court. |
| InvalidDataException | Octets incorrects trouvés lors du décodage. |
| NotSupportedException | Cette version LZ4 n'est pas prise en charge. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| InvalidOperationException | L'archive est préparée pour la composition. |

### Voir aussi

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrait l'archive vers le flux fourni.

```csharp
public void Extract(Stream destination)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destination | Stream | Flux de destination. Doit être accessible en écriture. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* ne prend pas en charge l'écriture. |
| EndOfStreamException | Le flux source est trop court. |
| InvalidDataException | Octets incorrects trouvés lors du décodage. |
| NotSupportedException | Cette version LZ4 n'est pas prise en charge. |
| InvalidOperationException | L'archive est préparée pour la composition. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Voir aussi

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


