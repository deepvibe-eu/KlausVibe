> Machine-translated from [README.md](README.md) into Deutsch — corrections welcome.

# KlausVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KlausVibe_fr.png" alt="KlausVibe screenshot" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/klausvibe">klausvibe.eu</a>
</p>

KlausVibe ist der **Claude-Build** der _Vibe_-Familie — ein Fork von ZCode, der sich auf einen einzigen Anbieter konzentriert: **Claude** (Anthropic). Ein Modell, ein Arbeitsbereich, ein Partner — kein Agent.

Die _Vibe_-Familie liefert eine fokussierte App pro Anbieter (DeepVibe für DeepSeek, KimiVibe für Kimi, LamaVibe für Ollama, KlausVibe für Claude, …), jede mit ihrem eigenen Charakter. Sie existiert **neben** ZCode, nicht an dessen Stelle: ZCode für den Multi-Provider-Workflow, die Vibe-Apps für Menschen, die ein Modell, einen Arbeitsbereich, einen Partner wollen. Siehe das Hauptquell-Repository für die vollständige Codebasis.

## Downloads

Installer für macOS, Windows und Linux werden unter [Releases](../../releases) veröffentlicht. Der integrierte Updater prüft dieses Repository.

## Aus dem Quellcode erstellen

Erfordert Git, Node.js **24.14.0** und pnpm **10.33.2** (siehe `mise.toml`).

```bash
pnpm bootstrap
# run the KlausVibe flavor in dev
pnpm dev:desktop:klaus
# package (KlausVibe flavor)
ZCODE_KLAUS_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Lizenz & Namensnennung

Basiert auf ZCode (Apache-2.0); die Lizenz und NOTICE bleiben erhalten. KlausVibe ist ein unabhängiges Projekt und ist weder mit ZCode/Z.ai noch mit Anthropic verbunden. Claude und Anthropic sind Marken ihrer jeweiligen Inhaber; das Logo wird mit Genehmigung des Betreibers verwendet.
