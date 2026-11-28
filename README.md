# Mi Tacógrafo — збірка APK на GitHub

1. На GitHub створи новий репозиторій (Create new repository), назва будь-яка.
2. Завантаж у нього ВСІ файли з цього архіву разом з папками `www`, `assets` і `.github` та файлом `debug.keystore` (Add file → Upload files). Папку `.github` з телефона зручніше завантажувати через вебверсію GitHub «Desktop site».
3. Вкладка Actions → «Build APK» → Run workflow (зелена збірка йде ~5–8 хв).
4. Відкрий завершений запуск → внизу Artifacts → `mi-tacografo-apk` (zip з `app-debug.apk`). Розпакуй і встанови APK.

Важливо: не губи `debug.keystore`. З ним кожна нова збірка підписана однаково й встановлюється поверх старої без втрати даних.
Дані зберігаються в самій програмі (localStorage). Перед першою заміною версії зроби експорт JSON.
Оновлення програми: заміни `www/index.html` на нову версію й запусти Run workflow.
