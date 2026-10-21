> Machine-translated from [README.md](README.md) into Deutsch — corrections welcome.

# KlausVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KlausVibe_fr.png" alt="KlausVibe screenshot" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/klausvibe">klausvibe.eu</a>
</p>

KlausVibe ist der **Claude-Build** der _Vibe_-Familie — ein Fork von ZCode, der sich auf einen einzigen Anbieter konzentriert: **Claude** (Anthropic). Ein Modell, ein Arbeitsbereich, ein Partner — kein Agent.

Die _Vibe_-Familie liefert eine fokussierte App pro Anbieter (DeepVibe für DeepSeek, KimiVibe für Kimi, LamaVibe für Ollama, KlausVibe für Claude, …), jede mit ihrem eigenen Charakter. Sie existiert **neben** ZCode, nicht an dessen Stelle: ZCode für den Multi-Provider-Workflow, die Vibe-Apps für Menschen, die ein Modell, einen Arbeitsbereich, einen Partner wollen. Den vollständigen Codebestand findest du im Hauptquellcode-Repository.

## Downloads

Installer für macOS, Windows und Linux findest du auf der [Releases-Seite](../../releases); die neueste Version ist immer mit **latest** getaggt:

| Plattform | Dateien |
| --- | --- |
| macOS (Apple Silicon) | `KlausVibe-<version>-mac-arm64.dmg` · `KlausVibe-<version>-mac-arm64.zip` |
| Windows | `KlausVibe-<version>-win-x64.exe` |
| Linux | `KlausVibe-<version>-linux-x86_64.AppImage` · `KlausVibe-<version>-linux-amd64.deb` · `KlausVibe-<version>-linux-x86_64.rpm` · `KlausVibe-<version>-linux-x64.pkg.tar.zst` |

Jede App der *Vibe*-Familie wird mit der **gleichen Versionsnummer** veröffentlicht (derzeit 1.0.5). Der integrierte Updater prüft die neueste Version dieses Repositorys.

> **macOS (Apple Silicon):** Der Build ist **unsigniert** (kein kostenpflichtiges Apple Developer Program), daher
> warnt Gatekeeper beim ersten Start. Die App ist ad-hoc signiert — öffne sie einmal über **Rechtsklick → Öffnen** oder führe
> `xattr -dr com.apple.quarantine "/Applications/KlausVibe.app"` aus.

## Aus dem Quellcode bauen

Erfordert Git, Node.js **24.14.0** und pnpm **10.33.2** (siehe `mise.toml`).

```bash
pnpm bootstrap
# run the KlausVibe flavor in dev
pnpm dev:desktop:klaus
# package (KlausVibe flavor)
ZCODE_KLAUS_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Lizenz & Namensnennung

Basiert auf ZCode (Apache-2.0); die Lizenz und der NOTICE-Hinweis bleiben erhalten. KlausVibe ist ein unabhängiges Projekt und steht in keiner Verbindung zu ZCode/Z.ai oder Anthropic. Claude und Anthropic sind Marken ihrer jeweiligen Inhaber; das Logo wird mit Genehmigung des Betreibers verwendet.
