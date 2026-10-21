> Machine-translated from [README.md](README.md) into Русский — corrections welcome.

# KlausVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KlausVibe_fr.png" alt="Скриншот KlausVibe" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/klausvibe">klausvibe.eu</a>
</p>

KlausVibe — это **сборка Claude** из семейства _Vibe_ — форк ZCode, ориентированный на одного провайдера: **Claude** (Anthropic). Одна модель, одно рабочее пространство, партнёр — а не агент.

Семейство _Vibe_ выпускает по одному специализированному приложению на каждого провайдера (DeepVibe для DeepSeek, KimiVibe для Kimi, LamaVibe для Ollama, KlausVibe для Claude, …), каждое со своим характером. Оно существует **наряду** с ZCode, а не вместо него: ZCode — для работы с несколькими провайдерами, приложения Vibe — для тех, кому нужна одна модель, одно рабочее пространство, один партнёр. Полный код проекта см. в основном репозитории.

## Загрузки

Установщики для macOS, Windows и Linux доступны на [странице релизов](../../releases); самый новый релиз всегда помечен тегом **latest**:

| Платформа | Файлы |
| --- | --- |
| macOS (Apple Silicon) | `KlausVibe-<version>-mac-arm64.dmg` · `KlausVibe-<version>-mac-arm64.zip` |
| Windows | `KlausVibe-<version>-win-x64.exe` |
| Linux | `KlausVibe-<version>-linux-x86_64.AppImage` · `KlausVibe-<version>-linux-amd64.deb` · `KlausVibe-<version>-linux-x86_64.rpm` · `KlausVibe-<version>-linux-x64.pkg.tar.zst` |

Все приложения семейства *Vibe* выпускаются с **одинаковым номером версии** (сейчас 1.0.5). Встроенный механизм обновления проверяет последний релиз этого репозитория.

> **macOS (Apple Silicon):** сборка **неподписанная** (нет платной программы Apple Developer), поэтому Gatekeeper
> предупреждает при первом запуске. Приложение подписано ad-hoc — откройте его один раз через **правый клик → Открыть** или выполните
> `xattr -dr com.apple.quarantine "/Applications/KlausVibe.app"`.

## Сборка из исходного кода

Требуются Git, Node.js **24.14.0** и pnpm **10.33.2** (см. `mise.toml`).

```bash
pnpm bootstrap
# run the KlausVibe flavor in dev
pnpm dev:desktop:klaus
# package (KlausVibe flavor)
ZCODE_KLAUS_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Лицензия и атрибуция

Создано на основе ZCode (Apache-2.0); лицензия и NOTICE сохранены. KlausVibe — независимый проект, не связанный с ZCode/Z.ai или Anthropic. Claude и Anthropic являются товарными знаками их владельца; логотип используется с разрешения оператора.
