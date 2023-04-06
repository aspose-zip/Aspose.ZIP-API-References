---
title: License.SetLicense
second_title: Référence de l'API Aspose.ZIP pour .NET
description: License méthode. Licence du composant.
type: docs
weight: 20
url: /fr/net/aspose.zip/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licence du composant.

```csharp
public void SetLicense(string licenseName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| licenseName | String | Peut être un nom de fichier complet ou court ou le nom d'une ressource intégrée. Utilisez une chaîne vide pour passer en mode d'évaluation. |

### Remarques

Essaie de trouver la licence aux emplacements suivants :

1. Chemin explicite.

2. Le dossier qui contient l'assemblage du composant Aspose.

3. Le dossier qui contient l'assembly appelant du client.

4. Le dossier qui contient l'assembly d'entrée (démarrage).

5. Une ressource intégrée dans l'assembly appelant du client.

**Note:**Sur le .NET Compact Framework, essaie de trouver la licence uniquement dans ces emplacements :

1. Chemin explicite.

2. Une ressource intégrée dans l'assembly appelant du client.

2. Le dossier qui contient le fichier JAR du composant Aspose.

3. Le dossier qui contient le fichier JAR appelant du client.

### Exemples

Dans cet exemple, une tentative sera faite pour trouver un fichier de licence nommé MyLicense.lic dans le dossier qui contient  le composant, dans le dossier qui contient l'assembly appelant, dans le dossier de l'assembly d'entrée puis dans les ressources embarquées de l'assembly appelant.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

le fichier jar du composant :

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Voir également

* class [License](../)
* espace de noms [Aspose.Zip](../../license/)
* Assemblée [Aspose.Zip](../../../)

---

## SetLicense(Stream) {#setlicense}

Licence du composant.

```csharp
public void SetLicense(Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Un flux qui contient la licence. |

### Remarques

Utilisez cette méthode pour charger une licence à partir d'un flux.

### Exemples

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### Voir également

* class [License](../)
* espace de noms [Aspose.Zip](../../license/)
* Assemblée [Aspose.Zip](../../../)


