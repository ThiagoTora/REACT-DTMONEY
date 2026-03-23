<img width="1860" height="972" alt="image" src="https://github.com/user-attachments/assets/28b9ae38-ba71-49c6-bd19-1beb54ea67c7" />


### ---------- DT Money - Gestão de Finanças Pessoais
O DT Money é uma aplicação de controlo financeiro desenvolvida para ajudar os utilizadores a gerir as suas entradas e saídas de capital de forma simples e intuitiva. A aplicação permite o registo de transações, a visualização de um resumo financeiro (entradas, saídas e total) e a filtragem de dados.

### ---------- Tecnologias Utilizadas

- React (com Vite)
- TypeScript
- Styled Components (para estilização)
- Axios (para consumo de API)
- Context API (para gestão de estado global das transações)
- React Hook Form + Zod (para validação e gestão de formulários)
- Radix UI (para componentes de acessibilidade como Modais)
- JSON Server (como API simulada para desenvolvimento)

### ---------- Funcionalidades

- Resumo de Saldo: Cálculo automático de entradas, saídas e o valor total em conta através de um hook personalizado (useSummary).
- Listagem de Transações: Visualização de todas as atividades financeiras registadas.
- Pesquisa Dinâmica: Filtro de transações por descrição.
- Novo Registo: Modal para adicionar novas transações categorizadas como entrada ou saída.
- Formatação: Valores e datas formatados de acordo com a moeda local e padrões regionais.

### ---------- Instalação e Execução
1. Clone o repositório:
   
    ```bash 
        git clone https://github.com/ThiagoTora/REACT-DTMONEY.git
        cd REACT-DTMONEY
    ```
    
2. Instale as dependências:
   
    ```bash
        npm install
    ```
3. Iniciar a API (JSON Server):

    ```bash
        npm run dev:server
    ```
    
4. Iniciar a aplicação
   
    ```bash
         npm run dev
    ```

### ---------- ESTRUTURA DO PROJETO
```bash
   REACT-DTMONEY/
   ├── public/
   │   └── vite.svg
   ├── src/
   │   ├── @types/
   │   │   └── styled.d.ts
   │   ├── assets/
   │   │   └── logo.svg
   │   ├── components/
   │   │   ├── Header/
   │   │   │   ├── index.tsx
   │   │   │   └── styles.ts
   │   │   ├── NewTransactionsModal/
   │   │   │   ├── index.tsx
   │   │   │   └── styles.ts
   │   │   └── Summary/
   │   │       ├── index.tsx
   │   │       └── styles.ts
   │   ├── Contexts/
   │   │   └── TransactionsContext.tsx
   │   ├── hooks/
   │   │   └── useSummary.tsx
   │   ├── lib/
   │   │   └── axios.ts
   │   ├── pages/
   │   │   └── Transactions/
   │   │       ├── components/
   │   │       │   └── SearchForm/
   │   │       │       ├── index.tsx
   │   │       │       └── styles.ts
   │   │       ├── index.tsx
   │   │       └── styles.ts
   │   ├── styles/
   │   │   ├── themes/
   │   │   │   └── default.ts
   │   │   └── global.ts
   │   ├── utils/
   │   │   └── formatter.ts
   │   ├── App.tsx
   │   ├── main.tsx
   │   └── vite-env.d.ts
   ├── .eslintrc.json
   ├── .gitignore
   ├── index.html
   ├── package.json
   ├── package-lock.json
   ├── server.json
   ├── tsconfig.json
   ├── tsconfig.app.json
   ├── tsconfig.node.json
   └── vite.config.ts
```
