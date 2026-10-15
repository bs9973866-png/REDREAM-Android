# RedReam — Minecraft Java Launcher (Android)

Android-приложение с интерфейсом лаунчера RedReam: версии, поиск модов Modrinth, 3D-скин, ИИ-помощник, настройки.
Интерфейс лежит в `app/src/main/assets/index.html` и открывается внутри WebView.

## Как получить APK
1. Загрузите все файлы проекта в репозиторий GitHub (ветка `main`).
2. Вкладка **Actions** → **Build APK** → дождитесь зелёной галочки (3–6 минут).
3. Внутри запуска скачайте артефакт **RedReam-apk**, распакуйте и установите `RedReam.apk`.
4. Для релиза создайте тег `v0.1.0`: APK появится в Releases.

## Статус
Работает: интерфейс, Modrinth, список версий, 3D-скин, ИИ (нужен ключ Anthropic в «Ещё»).
Пока имитируется: вход Microsoft и Ely.by, запуск самой игры, CurseForge.

## Как добавить запуск игры
Запуск Java Edition на Android делают PojavLauncher и Zalith Launcher (LGPL-3.0).
Путь: форкнуть Zalith, заменить его экраны экранами RedReam, подключить вход Microsoft и Ely.by (authlib-injector).
