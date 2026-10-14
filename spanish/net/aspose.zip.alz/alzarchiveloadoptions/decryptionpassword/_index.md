---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad AlzArchiveLoadOptions. Obtiene o establece la contraseña para descifrar las entradas."
type: docs
weight: 30
url: /es/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Obtiene o establece la contraseña para descifrar las entradas.

```csharp
public string DecryptionPassword { get; set; }
```

## Ejemplos

Puede proporcionar la contraseña de descifrado una vez al extraer el archivo.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.alz"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
        {
            using (var decompressed = archive.Entries[0].Open())
            {
                byte[] b = new byte[8192];
                int bytesRead;
                while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
                    extracted.Write(b, 0, bytesRead);
                
            }
        }
    }
}
```

### Ver también

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


