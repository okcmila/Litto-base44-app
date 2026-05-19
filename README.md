# Litto – Clube do Livro 📚

> App web de clube do livro com mapa de bibliotecas públicas de São Paulo.

---

Essa versãoa da plataforma foi criada pelo Base44 e migrado para o Github Codespace para adaptar autenticação e banco de dados para o Firebase.

[Relatório com Prompts e a Construção do Site](https://docs.google.com/document/d/1L_ScAtN6gdhlVj38P4pokKj_GtWZCMc-potcQe5qJlQ/edit?usp=sharing)

---

## Tecnologias Usadas 

- React
- Vite
- React Router DOM
- Firebase Authentication
- Framer Motion
- Tailwind CSS (design system customizado)
- Material Icons

---

##Estrutura do projeto
```.
├── .gitignore
├── README.md
├── components.json
├── eslint.config.js
├── index.html
├── jsconfig.json
├── package-lock.json
├── package.json
├── postcss.config.js
├── public
│   ├── favicon.svg
│   └── icons.svg
├── src
│   ├── App.css
│   ├── App.jsx
│   ├── api
│   ├── assets
│   │   ├── hero.png
│   │   ├── react.svg
│   │   └── vite.svg
│   ├── components
│   │   ├── ProtectedRoute.jsx
│   │   ├── auth
│   │   │   └── AuthInput.jsx
│   │   ├── home
│   │   │   ├── BooksSection.jsx
│   │   │   ├── CategoriesSection.jsx
│   │   │   ├── CommunitySection.jsx
│   │   │   ├── FeaturedBookSection.jsx
│   │   │   ├── FeedbackSection.jsx
│   │   │   ├── HeroSection.jsx
│   │   │   ├── MoviesSection.jsx
│   │   │   └── WhyLittoSection.jsx
│   │   ├── layout
│   │   │   ├── AppLayout.jsx
│   │   │   ├── Footer.jsx
│   │   │   ├── MobileNav.jsx
│   │   │   └── Navbar.jsx
│   │   └── ui
│   │       ├── BrutalButton.jsx
│   │       ├── BrutalCard.jsx
│   │       ├── MaterialIcon.jsx
│   │       ├── accordion.jsx
│   │       ├── alert-dialog.jsx
│   │       ├── alert.jsx
│   │       ├── aspect-ratio.jsx
│   │       ├── avatar.jsx
│   │       ├── badge.jsx
│   │       ├── breadcrumb.jsx
│   │       ├── button.jsx
│   │       ├── calendar.jsx
│   │       ├── card.jsx
│   │       ├── carousel.jsx
│   │       ├── chart.jsx
│   │       ├── checkbox.jsx
│   │       ├── collapsible.jsx
│   │       ├── command.jsx
│   │       ├── context-menu.jsx
│   │       ├── dialog.jsx
│   │       ├── drawer.jsx
│   │       ├── dropdown-menu.jsx
│   │       ├── form.jsx
│   │       ├── hover-card.jsx
│   │       ├── input-otp.jsx
│   │       ├── input.jsx
│   │       ├── label.jsx
│   │       ├── menubar.jsx
│   │       ├── navigation-menu.jsx
│   │       ├── pagination.jsx
│   │       ├── popover.jsx
│   │       ├── progress.jsx
│   │       ├── radio-group.jsx
│   │       ├── resizable.jsx
│   │       ├── scroll-area.jsx
│   │       ├── select.jsx
│   │       ├── separator.jsx
│   │       ├── sheet.jsx
│   │       ├── sidebar.jsx
│   │       ├── skeleton.jsx
│   │       ├── slider.jsx
│   │       ├── sonner.jsx
│   │       ├── switch.jsx
│   │       ├── table.jsx
│   │       ├── tabs.jsx
│   │       ├── textarea.jsx
│   │       ├── toast.jsx
│   │       ├── toaster.jsx
│   │       ├── toggle-group.jsx
│   │       ├── toggle.jsx
│   │       ├── tooltip.jsx
│   │       └── use-toast.jsx
│   ├── hooks
│   │   └── use-mobile.jsx
│   ├── index.css
│   ├── lib
│   │   ├── AuthContext.jsx
│   │   ├── PageNotFound.jsx
│   │   ├── firebase.js
│   │   ├── query-client.js
│   │   └── utils.js
│   ├── main.jsx
│   ├── pages
│   │   ├── Bibliotecas.jsx
│   │   ├── Cadastro.jsx
│   │   ├── Comunidade.jsx
│   │   ├── Entrar.jsx
│   │   ├── Explorar.jsx
│   │   ├── Home.jsx
│   │   ├── Perfil.jsx
│   │   └── RecuperarSenha.jsx
│   └── utils
│       └── index.ts
├── tailwind.config.js
├── vercel.json
└── vite.config.js

---

## Arquitetura do Deploy

O projeto utiliza arquitetura frontend distribuída:
-Frontend hospedado no Vercel
-Aplicação desenvolvida em React + Vite
-Autenticação gerenciada pelo Firebase Authentication
-Navegaçãao SPA utilizando React Router DOM
-Estado global de autenticação via Context API

Fluxo: Usuário - Vercel (React App) - Firebase Authentiction
