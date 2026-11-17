# Портфолио — Мартин Миллер

**Сайт:** <https://maka-o.github.io/my/>  
**Репозиторий:** <https://github.com/MAKA-O/my>

Одностраничный сайт-портфолио. Собран по данным GitHub-профиля
[MAKA-O](https://github.com/MAKA-O): проекты, стек и ссылки взяты из публичных
репозиториев, ничего не придумано.

## Стек

- HTML5, CSS3 (custom properties, Grid, `clamp()` и fluid layout)
- Vanilla JavaScript: мобильное меню, scrollspy, reveal-анимации, год в футере
- Без сборки, фреймворков и npm-зависимостей
- Google Fonts (Playfair Display, Golos Text, JetBrains Mono) с системными
  фолбэками — при отсутствии сети сайт остаётся читаемым

## Файлы

```text
index.html        разметка и весь контент
styles.css        дизайн-система, адаптив, обложки проектов
script.js         меню, навигация, анимации появления
assets/avatar.jpg локальный аватар
```

## Запуск

Самый простой способ — открыть `index.html` двойным щелчком: сайт работает по
`file://` без сервера.

Если нужен локальный сервер (например, для проверки в другом браузере):

```powershell
python -m http.server 8000
```

Затем откройте <http://localhost:8000>.

## Хостинг на GitHub Pages

Сайт уже опубликован: <https://maka-o.github.io/my/>.

**Как обновлять:**

```powershell
git add .
git commit -m "Update site"
git push
```

GitHub Pages пересоберёт сайт автоматически за 1–2 минуты. Сборка не нужна:
все пути относительные, а `.nojekyll` отключает обработку Jekyll.

**Если разворачивать с нуля:**

1. Создайте публичный репозиторий и загрузите в него файлы сайта.
2. Откройте **Settings → Pages**.
3. В разделе **Build and deployment** выберите **Deploy from a branch**.
4. Укажите ветку `main` и папку `/ (root)`, нажмите **Save**.
5. Через 1–2 минуты сайт будет доступен по адресу из раздела Pages
   (для репозитория `my` — `https://maka-o.github.io/my/`).

## Что можно настроить

- **Фото** — замените `assets/avatar.jpg`, сохранив имя файла.
- **Тексты** — блоки «О себе», описания проектов и подписи находятся в
  `index.html`.
- **Ссылки и почта** — поиском по `MAKA-O` и `mrmmvo@gmail.com`.
- **Цвета и шрифты** — токены в `:root` в начале `styles.css`.
- **Проекты** — карточки устроены однотипно; обложки собраны из CSS/SVG, без
  растровых скриншотов.

## Источники данных

- Профиль: <https://github.com/MAKA-O>
- Проекты: [HH7d](https://github.com/MAKA-O/HH7d),
  [sit](https://github.com/MAKA-O/sit) (+ [демо](https://maka-o.github.io/sit/index.html)),
  [bl2](https://github.com/MAKA-O/bl2),
  [VUE1](https://github.com/MAKA-O/VUE1)
- Аватар: GitHub-профиль пользователя
