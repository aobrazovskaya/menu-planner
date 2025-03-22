# Menu Planner

## ✨ Описание проекта

Menu Planner — это веб-приложение для планирования меню на неделю с возможностью выбора блюд и генерации списка покупок.

## ✅ Функциональность

* 📅 Календарь: планирование приёмов пищи на неделю.

* 🍽️ База рецептов: просмотр и добавление блюд.

* 🛍️ Список покупок: автоматическое формирование списка необходимых продуктов.

* 🔐 Авторизация: регистрация и вход пользователей (по желанию).

## Используемый стек технологий

### Frontend (React SPA)

* React + Vite

* React Query — управление API-запросами.

* react-calendar — календарь.

* dnd-kit — drag & drop для управления меню.

### Backend (NestJS + PostgreSQL)

* NestJS — создание API.

* PostgreSQL + Prisma — база данных.

* JWT — аутентификация пользователей.

* Express.js — обработка запросов (встроено в NestJS).

## 🔄 Развёртывание и запуск

1. Клонирование репозитория

```
# Фронтенд
git clone https://github.com/aobrazovskaya/menu-planner.git
cd menu-planner

# Бэкенд
git clone https://github.com/aobrazovskaya/menu-planner-backend.git
cd menu-planner-backend
```

2. Установка зависимостей

```
# Фронтенд
cd menu-planner
npm install

# Бэкенд
cd menu-planner-backend
npm install
```

3. Настройка переменных окружения

4. Запуск проекта

```
# Запуск фронтенда
cd menu-planner
npm run dev

# Запуск бэкенда
cd menu-planner-backend
npm run start:dev
```

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default tseslint.config({
  extends: [
    // Remove ...tseslint.configs.recommended and replace with this
    ...tseslint.configs.recommendedTypeChecked,
    // Alternatively, use this for stricter rules
    ...tseslint.configs.strictTypeChecked,
    // Optionally, add this for stylistic rules
    ...tseslint.configs.stylisticTypeChecked,
  ],
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default tseslint.config({
  plugins: {
    // Add the react-x and react-dom plugins
    'react-x': reactX,
    'react-dom': reactDom,
  },
  rules: {
    // other rules...
    // Enable its recommended typescript rules
    ...reactX.configs['recommended-typescript'].rules,
    ...reactDom.configs.recommended.rules,
  },
})
```
