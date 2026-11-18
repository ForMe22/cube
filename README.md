# cube

Fichier FreeCAD 1.1 : cube creux de 50 mm de côté, épaisseur de paroi 3 mm
(cavité interne de 44 x 44 x 44 mm).

## Contenu

- `cube.FCStd.b64` : le fichier projet FreeCAD `cube.FCStd` encodé en base64.

## Récupérer le fichier .FCStd

Le connecteur GitHub ne téléverse que du texte ; le fichier binaire est donc fourni encodé.

Linux / macOS :

```bash
base64 -d cube.FCStd.b64 > cube.FCStd
```

Windows PowerShell :

```powershell
[IO.File]::WriteAllBytes("cube.FCStd", [Convert]::FromBase64String((Get-Content cube.FCStd.b64 -Raw)))
```

Ouvrez ensuite `cube.FCStd` avec FreeCAD 1.1 (ou version récente) : si une
recomputation est demandée, cliquez sur l'icône d'actualisation.
