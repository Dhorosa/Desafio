# Desafio - Cadastro de Colaboradores

Aplicação web para gestão de colaboradores e departamentos, com autenticação no Firebase, filtros, edição em etapas e persistência no Firestore.

## Acesso online

- App: `link a definir após o deploy`

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

### 1. Instale as dependências

```bash
npm install
```

### 2. Crie o arquivo `.env.local`

No Windows (PowerShell):

```powershell
Copy-Item .env.example .env.local
```

No Mac/Linux:

```bash
cp .env.example .env.local
```

### 3. Preencha o `.env.local`

Use as variáveis do seu projeto Firebase:

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

- [http://127.0.0.1:5173](http://127.0.0.1:5173)

## Acesso de teste

Se o Firebase estiver configurado com autenticação por e-mail e senha, use um usuário válido criado no Authentication.

## Funcionalidades

- Login com Firebase Authentication
- Rotas protegidas
- Página 404
- Cadastro, edição e exclusão de colaboradores
- Exclusão em massa de colaboradores
- Cadastro, edição e exclusão de departamentos
- Exclusão em massa de departamentos
- Filtros por nome, e-mail e departamento
- Formulário em etapas
- Regra de gestor por departamento

## Se der erro ao iniciar

- Verifique se o arquivo se chama exatamente `.env.local`
- Verifique se todas as variáveis do Firebase foram preenchidas
- Reinicie o `npm run dev` depois de alterar o `.env.local`
