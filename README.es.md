> Machine-translated from [README.md](README.md) into Español — corrections welcome.

# KlausVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KlausVibe_fr.png" alt="Captura de pantalla de KlausVibe" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/klausvibe">klausvibe.eu</a>
</p>

KlausVibe es la **build de Claude** de la familia _Vibe_ — un fork de ZCode enfocado en un único proveedor: **Claude** (Anthropic). Un modelo, un espacio de trabajo, un socio — no un agente.

La familia _Vibe_ distribuye una aplicación enfocada por proveedor (DeepVibe para DeepSeek, KimiVibe para Kimi, LamaVibe para Ollama, KlausVibe para Claude, …), cada una con su propio carácter. Existe **junto a** ZCode, no en su lugar: ZCode para el flujo de trabajo multiproveedor, las aplicaciones Vibe para quienes quieren un modelo, un espacio de trabajo, un socio. Consulta el repositorio de código fuente principal para ver la base de código completa.

## Descargas

Los instaladores para macOS, Windows y Linux se publican en [Releases](../../releases). El actualizador integrado comprueba este repositorio.

## Compilar desde el código fuente

Requiere Git, Node.js **24.14.0** y pnpm **10.33.2** (consulta `mise.toml`).

```bash
pnpm bootstrap
# run the KlausVibe flavor in dev
pnpm dev:desktop:klaus
# package (KlausVibe flavor)
ZCODE_KLAUS_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Licencia y atribución

Construido sobre ZCode (Apache-2.0); la licencia y el NOTICE se conservan. KlausVibe es un proyecto independiente y no está afiliado a ZCode/Z.ai ni a Anthropic. Claude y Anthropic son marcas registradas de sus propietarios; el logotipo se utiliza con el permiso del operador.
