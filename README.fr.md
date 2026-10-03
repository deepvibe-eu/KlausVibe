> Machine-translated from [README.md](README.md) into Français — corrections welcome.

# KlausVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KlausVibe_fr.png" alt="Capture d'écran de KlausVibe" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/klausvibe">klausvibe.eu</a>
</p>

KlausVibe est la **version Claude** de la famille _Vibe_ — un fork de ZCode centré sur un seul fournisseur : **Claude** (Anthropic). Un modèle, un espace de travail, un partenaire — pas un agent.

La famille _Vibe_ propose une application dédiée par fournisseur (DeepVibe pour DeepSeek, KimiVibe pour Kimi, LamaVibe pour Ollama, KlausVibe pour Claude, …), chacune avec son propre caractère. Elle existe **aux côtés** de ZCode, et non à sa place : ZCode pour le flux de travail multi-fournisseurs, les applications Vibe pour ceux qui veulent un modèle, un espace de travail, un partenaire. Consultez le dépôt source principal pour l'ensemble du code.

## Téléchargements

Les installateurs pour macOS, Windows et Linux sont publiés dans [Releases](../../releases). Le programme de mise à jour intégré vérifie ce dépôt.

## Compilation depuis les sources

Nécessite Git, Node.js **24.14.0** et pnpm **10.33.2** (voir `mise.toml`).

```bash
pnpm bootstrap
# run the KlausVibe flavor in dev
pnpm dev:desktop:klaus
# package (KlausVibe flavor)
ZCODE_KLAUS_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Licence et attribution

Basé sur ZCode (Apache-2.0) ; la licence et le NOTICE sont conservés. KlausVibe est un projet indépendant et n'est affilié ni à ZCode/Z.ai ni à Anthropic. Claude et Anthropic sont des marques de leur propriétaire ; le logo est utilisé avec l'autorisation de l'exploitant.
