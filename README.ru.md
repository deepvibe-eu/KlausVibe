> Machine-translated from [README.md](README.md) into Русский — corrections welcome.

# KlausVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KlausVibe_fr.png" alt="Скриншот KlausVibe" width="auto" />
</div>

<p align="center">
  <a href="https://deepvibe.eu/klausvibe">klausvibe.eu</a>
</p>

KlausVibe — это **сборка Claude** из семейства _Vibe_ — форк ZCode, ориентированный на одного провайдера: **Claude** (Anthropic). Одна модель, одно рабочее пространство, партнёр — не агент.

Семейство _Vibe_ выпускает по одному специализированному приложению на каждого провайдера (DeepVibe для DeepSeek, KimiVibe для Kimi, LamaVibe для Ollama, KlausVibe для Claude, …), каждое со своим характером. Оно существует **рядом** с ZCode, а не вместо него: ZCode — для работы с несколькими провайдерами, приложения Vibe — для тех, кому нужна одна модель, одно рабочее пространство, один партнёр. Полную кодовую базу см. в основном репозитории.

## Загрузки

Установщики для macOS, Windows и Linux публикуются в разделе [Releases](../../releases). Встроенное средство обновления проверяет этот репозиторий.

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
