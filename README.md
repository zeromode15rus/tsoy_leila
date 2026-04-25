# Кабинет УЗИ — Цой Л.Б.

Одностраничный сайт (React + Vite), **тёплая** светлая тема, отдельно от шаблона `olhovoy`.

## Локальный запуск

```bash
cd tsoi-uzi
npm install
npm run dev
```

## Что отредактировать перед публикацией

- `src/data/siteData.js` — адрес, телефоны, при необходимости ФИО и формулировки.
- `index.html` — `<title>`, meta description, **canonical** (замените `https://example.com/`).
- `public/photo/` — фото врача; в `siteData` укажите `photoPath: 'photo/имя-файла.jpg'`.
- `public/docs/license.pdf` — скан лицензии; до загрузки кнопка «Скачать» отдаст 404.
- `public/sitemap.xml` и `public/robots.txt` — подставьте реальный домен.

## Сборка

```bash
npm run build
```

Артефакты в папке `dist/`. Для GitHub Project Pages при необходимости:  
`VITE_BASE=/имя-репозитория/ npm run build`

## Публикация на GitHub Pages

1. Создайте **новый** репозиторий, запушьте **содержимое папки `tsoi-uzi`** в корень (или саму папку как корень).
2. **Settings → Pages → Build and deployment → GitHub Actions.**
3. Первый push в `main` запустит workflow `.github/workflows/deploy-pages.yml` (нужен включённый Pages для репо).

## Структура

```
tsoi-uzi/
  src/
    App.jsx, App.css, index.css, main.jsx
    data/siteData.js
  public/
    docs/, photo/
  index.html, vite.config.js, package.json
```
# tsoy_leila
