# Java 25 in Jupyter (Binder) – Minimal-Repo

Dieses Repo startet auf mybinder.org ein JupyterLab mit:
- Java 25 (Temurin)
- Java 25 (conduziert via conda-forge)
- IJava-Kernel (Java in Jupyter-Notebooks)

## Loslegen (Binder)

Badge (ersetzen Sie `IHR_GITHUB_NAME/IHR_REPO`):
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/IHR_GITHUB_NAME/IHR_REPO/HEAD)

Direkt dieses Beispiel-Notebook öffnen (JupyterLab):
https://mybinder.org/v2/gh/IHR_GITHUB_NAME/IHR_REPO/HEAD?labpath=notebooks/01_einfuehrung_java.ipynb

## Ordnerstruktur
siehe Dateien in diesem Repo (.binder/, notebooks/).

## Nutzungshinweise
- Erster Start baut das Image (einige Minuten). Folgestarts sind schneller.
- In JupyterLab im Browser (auch iPad) ausführen.
- Sessions sind flüchtig. Änderungen ggf. herunterladen oder in eigenes Repo speichern.

## Troubleshooting
- Wenn der Java-Kernel fehlt oder `java -version` nicht 25 zeigt:
  - Binder-Build-Logs öffnen und den Abschnitt aus `postBuild` prüfen.
  - Die Adoptium-API-URL kann vorübergehend langsam sein; nach kurzer Zeit erneut starten.
- Maven-Dependencies werden per `%%maven` installiert (pro Kernel-Session).
