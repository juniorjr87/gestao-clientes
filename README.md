# RestoExpenses

Aplicação de gestão de despesas para restaurantes.

## Configuração Firebase

1. Crie um projeto no [Firebase Console](https://console.firebase.google.com/).
2. Ative o **Authentication** e habilite o provedor **Email/Password**.
3. Crie um utilizador manualmente na aba "Users" do Authentication (este será o seu login Master).
4. Ative o **Firestore Database** em modo de produção.
5. Copie as regras de segurança do ficheiro `firestore.rules` para a aba "Rules" do Firestore.
6. Vá a "Project Settings" -> "General" -> "Your apps" -> SDK setup and configuration (npm).
7. Copie as chaves para o ficheiro `.env` (baseado no `.env.example`).

## Funcionalidades

- **Master Login**: Apenas utilizadores autenticados podem aceder.
- **Fornecedores**: Gestão com categorias e cores.
- **Despesas**: Registo rápido com distinção de Fatura/Sem Fatura.
- **Relatórios**: Tabela mensal com exportação para PDF e Excel.

## Tecnologias

- React + Vite + TypeScript
- Tailwind CSS
- Firebase (Auth + Firestore)
- jsPDF + AutoTable (PDF)
- SheetJS (Excel)
