---
title: Vite
permalink: /notes/vite/
---

[Назад](..) # [Главная](/) / [Конспекты](/notes) / {{ page.title }}

---

<p style="margin: 0"><br></p>

# {{ page.title }}

# Плагины для Vite

## [unplugin-fonts](https://github.com/cssninjaStudio/unplugin-fonts)

Универсальный загрузчик веб-шрифтов.

### Установка

    npm i unplugin-fonts -D

### Подключение

_vite.config.js_

```js
import Fonts from 'unplugin-fonts/vite';

export default defineConfig({
    plugins: [
        Fonts({
            google: {
                families: [
                    {
                        name: 'Ubuntu',
                        styles: 'ital,wght@0,300;0,400;0,500;0,700',
                    },
                ],
            },
        }),
    ],
});
```
