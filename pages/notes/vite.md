---
title: Vite
permalink: /notes/vite
---

# {{ page.title }}

# Плагины для Vite

## [unplugin-fonts](https://github.com/cssninjaStudio/unplugin-fonts)

Универсальный загрузчик веб-шрифтов.

### Установка

    npm i unplugin-fonts -D

### vite.config.js

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
