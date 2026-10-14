---
title: "AlzEntry.Extract"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode AlzEntry. Extrait l'entrée dans le système de fichiers en utilisant le chemin fourni"
type: docs
weight: 60
url: /fr/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

Extrait l'entrée dans le système de fichiers au chemin fourni.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |
| mot de passe | String | Mot de passe optionnel pour le déchiffrement. |

### Valeur de retour

Les informations du fichier d'un fichier composé.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| InvalidDataException | L'archive est corrompue. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| FileNotFoundException | Le fichier est introuvable. |

## Exemples

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Voir aussi

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extrait l'entrée vers le flux fourni.

```csharp
public void Extract(Stream destination, string password = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destination | Stream | Flux de destination. Doit être accessible en écriture. |
| mot de passe | String | Mot de passe optionnel pour le déchiffrement. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* ne prend pas en charge l'écriture. |
| InvalidOperationException | L'archive n'est pas ouverte pour l'extraction. - ou - Cette entrée est un répertoire. |
| InvalidDataException | Données incorrectes dans l'entrée. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |

## Exemples

Extraire une entrée de l'archive ALZ avec un mot de passe.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Voir aussi

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


