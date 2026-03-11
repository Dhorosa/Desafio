# Desafio - Cadastro de Colaboradores

Aplicacao web para gestao de colaboradores e departamentos, com autenticacao no Firebase, filtros, edicao em etapas e persistencia no Firestore.

## Acesso online

- App: https://desafio-weld-rho.vercel.app
- GitHub: https://github.com/Dhorosa/Desafio

## Tecnologias usadas

- React 19
- TypeScript
- Vite
- Material UI
- React Hook Form
- Zod
- Firebase Authentication
- Firestore

## Como executar localmente

### 1. Instale as dependencias

```bash
npm install
```

### 2. Crie o arquivo .env.local

No Windows (PowerShell):

```powershell
Copy-Item .env.example .env.local
```

No Mac/Linux:

```bash
cp .env.example .env.local
```

### 3. Preencha o .env.local

Use as variaveis do seu projeto Firebase:

```env
VITE_FIREBASE_API_KEY=...
VITE_FIREBASE_AUTH_DOMAIN=...
VITE_FIREBASE_PROJECT_ID=...
VITE_FIREBASE_STORAGE_BUCKET=...
VITE_FIREBASE_MESSAGING_SENDER_ID=...
VITE_FIREBASE_APP_ID=...
```

### 4. Rode o projeto

```bash
npm run dev
```

### 5. Abra no navegador

- http://127.0.0.1:5173

## Acesso de teste

Se o Firebase estiver configurado com autenticacao por e-mail e senha, use um usuario valido criado no Authentication.

## Funcionalidades

- Login com Firebase Authentication
- Rotas protegidas
- Pagina 404
- Cadastro, edicao e exclusao de colaboradores
- Exclusao em massa de colaboradores
- Cadastro, edicao e exclusao de departamentos
- Exclusao em massa de departamentos
- Filtros por nome, e-mail e departamento
- Formulario em etapas
- Regra de gestor por departamento

## Se der erro ao iniciar

- Verifique se o arquivo se chama exatamente .env.local
- Verifique se todas as variaveis do Firebase foram preenchidas
- Reinicie o npm run dev depois de alterar o .env.local
