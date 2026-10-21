> Machine-translated from [README.md](README.md) into Español — corrections welcome.

# KlausVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KlausVibe_fr.png" alt="KlausVibe screenshot" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/klausvibe">klausvibe.eu</a>
</p>

KlausVibe es la **build de Claude** de la familia _Vibe_ — un fork de ZCode enfocado en un único proveedor: **Claude** (Anthropic). Un modelo, un espacio de trabajo, un compañero — no un agente.

La familia _Vibe_ distribuye una aplicación enfocada por proveedor (DeepVibe para DeepSeek, KimiVibe para Kimi, LamaVibe para Ollama, KlausVibe para Claude, …), cada una con su propio carácter. Existe **junto a** ZCode, no en su lugar: ZCode para el flujo de trabajo multiproveedor, las aplicaciones Vibe para quienes quieren un modelo, un espacio de trabajo, un compañero. Consulta el repositorio principal del código fuente para ver la base de código completa.

## Descargas

Los instaladores para macOS, Windows y Linux están en la [página de releases](../../releases); la versión más reciente siempre está etiquetada como **latest**:

| Plataforma | Archivos |
| --- | --- |
| macOS (Apple Silicon) | `KlausVibe-<version>-mac-arm64.dmg` · `KlausVibe-<version>-mac-arm64.zip` |
| Windows | `KlausVibe-<version>-win-x64.exe` |
| Linux | `KlausVibe-<version>-linux-x86_64.AppImage` · `KlausVibe-<version>-linux-amd64.deb` · `KlausVibe-<version>-linux-x86_64.rpm` · `KlausVibe-<version>-linux-x64.pkg.tar.zst` |

Cada aplicación de la familia *Vibe* se publica con el **mismo número de versión** (actualmente 1.0.5). El actualizador integrado comprueba la última release de este repositorio.

> **macOS (Apple Silicon):** la build **no está firmada** (sin Apple Developer Program de pago), por lo que Gatekeeper
> avisa en el primer inicio. La aplicación está firmada ad-hoc — ábrela una vez con **clic derecho → Abrir**, o ejecuta
> `xattr -dr com.apple.quarantine "/Applications/KlausVibe.app"`.

## Compilar desde el código fuente

Requiere Git, Node.js **24.14.0** y pnpm **10.33.2** (ver `mise.toml`).

```bash
pnpm bootstrap
# run the KlausVibe flavor in dev
pnpm dev:desktop:klaus
# package (KlausVibe flavor)
ZCODE_KLAUS_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Licencia y atribución

Construido sobre ZCode (Apache-2.0); la licencia y el NOTICE se conservan. KlausVibe es un proyecto independiente y no está afiliado a ZCode/Z.ai ni a Anthropic. Claude y Anthropic son marcas registradas de sus propietarios; el logotipo se utiliza con el permiso del operador.
