# Календарь Android
1. Распакуйте ZIP и загрузите содержимое в корень репозитория, включая скрытую папку `.github` (файл `.github/workflows/build.yml`). Если она не загружается, создайте файл с этим путём через Add file → Create new file и вставьте содержимое build.yml.
2. В Settings → Secrets and variables → Actions → New repository secret создайте секрет `CALENDAR_KEYSTORE`. Вставьте содержимое отдельно полученного файла calendar_signing_secret.txt. Не публикуйте этот файл в репозитории. Сохраните личную резервную копию.
3. Actions → Build and publish Calendar APK → Run workflow. После успеха APK находится в Releases. Постоянная ссылка: https://github.com/LOGIN/REPO/releases/latest/download/calendar.apk (для приватного репозитория требуется вход).
4. Установите APK на Android, разрешив установку из этого источника. Для обновлений не меняйте секрет и идентификатор приложения.

Приложение автономное, Android 8+. Данные в локальном хранилище. При удалении приложения данные теряются. Данные из HTML-версии не переносятся автоматически. Напоминания работают только при открытом приложении. Сборка на GitHub и запуск на Android пока не проверены.
