# SOTEX Banner

Адаптивный HTML/CSS-баннер для главной страницы бренда SOTEX.  
Баннер сделан без JavaScript, полностью на градиентах и тенях, с аккуратной мобильной версией.

## Демо:
> https://eva-kotofe-eva.github.io/sotex-banner/  

## Превью

> https://eva-kotofe-eva.github.io/sotex-banner/preview-desktop.png

## Структура проекта

- `index.html` — страница-демо с подключённым баннером.
- `sotex-main-banner.css` — основной файл стилей баннера.
- `img/` — исходник - один единственный аппаратик (ну и картинка превьюшки):
  - `sotex-495.png` (или другое имя) — PNG аппарата с прозрачным фоном.
  - `preview-desktop.png` — скриншоты для README.

## Особенности

- 🎯 **Чистый HTML + CSS**  
  Без JS и сторонних библиотек — можно спокойно встраивать в любые CMS и шаблоны.

- 🌈 **Сложный фон без картинок - ой как он мне прям нравится ну вообще**  
  Стена, пол, синяя подсветка, вертикальные полоски и виньетка собраны на:
  - `linear-gradient`
  - `radial-gradient`
  - `repeating-linear-gradient`

- 📱 **Адаптивность - моя головная боль но зато красивое))**  
  Три основных состояния:
  - десктоп (до 1420 px),
  - «ноутбуки» (`max-width: 1200px`),
  - планшеты/мобильные (`max-width: 768px`):
    - текст центрируется,
    - аппарат уходит под текст,
    - подсветка смещена под аппарат.

- ✨ **Аккуратная типографика**  
  - шрифты на основе `Roboto`;
  - знак `®` оформлен как верхний индекс через отдельный класс `.sotex-reg`, но вот здесь даже спроисть не у кого как это все влияет на пс;
  - лёгкий псевдо-обвод текста через `text-shadow` для читаемости.

- 🎬 **Небольшие анимации**  
  Плавное появление текста и аппарата (`fadeInLeft`, `fadeInRight`, `fadeInUp`).  
  И плюсик , при включённой опции «уменьшить анимацию» в системе (`prefers-reduced-motion`) анимации отключаются.

## Как использовать баннер в другом проекте

1. Подключите CSS
2. Вставьте HTML-блок баннера в нужное место страницы
3. Проверьте путь к картинке аппарата (src="img/sotex-495.png") и к CSS-файлу — подправьте под свою структуру проекта.

Кастомизация

Текст — меняется прямо в index.html внутри .sotex-banner__title и .sotex-banner__text.
Цвета фона и подсветки — блок background: в .sotex-banner (десктоп) и в медиазапросе @media (max-width: 768px).
Размер аппарата — свойство height у .sotex-banner__image.
Анимации — можно отключить или изменить в блоке @keyframes и классах animation.

Лицензия

Проект можно свободно использовать и адаптировать под коммерческие и некоммерческие проекты компании SOTEX.
Если будете использовать вне компании — буду рада, если в README останется ссылка на этот репозиторий.


---

## English version

# SOTEX Banner

Responsive HTML/CSS hero banner for the SOTEX brand homepage.  
Built without JavaScript, only gradients, shadows and media queries, with a neat mobile layout.

Demo: https://eva-kotofe-eva.github.io/sotex-banner/  

## Preview

> https://eva-kotofe-eva.github.io/sotex-banner/preview-desktop.png

## Project structure

- `index.html` — demo page with the connected banner.
- `sotex-main-banner.css` — main stylesheet for the banner.
- `img/` — source graphics:
  - `sotex-495.png` — sprayer PNG with transparent background.
  - `preview-desktop.png` — screenshot used in this README.

## Highlights

- **Pure HTML + CSS**  
  No JS or external libraries.

- **Gradient-based background**  
  Wall, floor, blue glow and vertical stripes are created with:
  `linear-gradient`, `radial-gradient`, `repeating-linear-gradient`.

- **Responsive layout**  
  Desktop, laptop and tablet/mobile breakpoints:
  text rearranges, the sprayer moves under the text, lighting shifts.

- **Careful typography & motion**  
  Roboto-based fonts, small `text-shadow` for readability,  
  subtle entrance animations with `@keyframes` and
  `prefers-reduced-motion` support.

## Re-use

Designed to be easy to drop into existing projects:
one CSS file, one HTML block and one PNG image; colors and sizes are adjusted directly in CSS.

## License

Free to use and adapt in SOTEX commercial and non-commercial projects.  
For external projects, a link back to this repository is welcome but not required.

