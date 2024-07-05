
---

# 🚀 Criando um Projeto com React.js e Tailwind CSS

## 📦 Início Rápido

### Comando para criar um novo projeto React.js:
```sh
npm install -g create-react-app
# ou
npx create-react-app design-patterns
```

### Após a instalação, abra o projeto no VS Code:
```sh
ls
cd nome-da-pasta
code .
```

## 🗂️ Organização das Pastas

```plaintext
assets/

pages/ 
  └── dashboard
  └── home
  └── login
  └── products
  └── register
  └── suppliers

shared/ 
  └── components/
      └── alert
      └── drawer
      └── label
      └── modals
      └── products
      └── subtitle
      └── suppliers
  └── contexts
  └── environment
  └── layouts
  └── routes

services/
  └── api
      └── auth
      └── axiosConfig
      └── categories
      └── products
      └── reports
      └── suppliers
```

## 🎨 Instalar Tailwind CSS

### Passo 1: Instale o Tailwind CSS via npm e inicialize o arquivo de configuração:
```sh
npm install -D tailwindcss
npx tailwindcss init
```

### Passo 2: Configure os caminhos do seu modelo
Adicione os caminhos para todos os seus arquivos de modelo no seu `tailwind.config.js`.

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### Passo 3: Adicione as diretivas Tailwind ao seu CSS
Adicione as diretivas `@tailwind` para cada uma das camadas do Tailwind ao seu arquivo `./src/index.css`.

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### Passo 4: Inicie o processo de construção
Execute o processo de compilação com o comando:

```sh
npm run start
```

---