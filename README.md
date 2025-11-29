# AVA - SAGE

**Sistema de Aprendizagem e Gestão Educacional**

O **AVA - SAGE** é uma plataforma integrada para instituições de ensino superior que unifica as vertentes acadêmica (LMS/AVA) e administrativa (SGE). O sistema visa centralizar a gestão de aulas, notas, financeiro e comunicação, eliminando a fragmentação de dados e otimizando a eficiência operacional da instituição.

Este é o repositório central que agrupa os módulos de Frontend e Backend.

## 📂 Estrutura do Projeto

O projeto é dividido em dois microsserviços/repositórios principais:

| Módulo | Repositório | Tecnologias Principais |
| :--- | :--- | :--- |
| **Backend** | [ava-backend](https://github.com/otaviocostao/ava-backend) | NestJS, TypeORM, Postgres, Socket.io |
| **Frontend** | [AVA-UNIFAN](https://github.com/RiosWesley/AVA-UNIFAN) | Next.js, React, TailwindCSS |

## 🚀 Funcionalidades Principais

  - ✔️ **Gestão Acadêmica e Administrativa:** Unificação de LMS e SGE.
  - ✔️ **Interface Reativa:** Construída com React e Next.js para uma experiência fluida.
  - ✔️ **Backend Escalável:** API RESTful desenvolvida em NestJS com TypeScript.
  - ✔️ **Comunicação Real-Time:** Uso de Socket.io para recursos interativos.
  - ✔️ **Infraestrutura Híbrida:** Backend em EC2 (AWS) e Banco de Dados/Storage no Supabase.

## 🛠️ Tecnologias Utilizadas

### Backend

  *  **Nest.js** (Framework principal)
  *  **TypeScript**
  *  **PostgreSQL** (Via Supabase)
  *  **TypeORM**
  * **Socket.io** (WebSockets)

### Frontend

  *  **Next.js** (Client-side rendering)
  *  **React**
  *  **TailwindCSS**
  * **Axios**

### Infraestrutura & Cloud

  *  **AWS EC2** (Hospedagem da API)
  *  **Supabase** (Banco de Dados e Storage de Arquivos)

-----

## ⚙️ Como Rodar o Projeto

Siga os passos abaixo para executar a aplicação localmente.

### Pré-requisitos

Antes de começar, certifique-se de ter instalado:

  * [Node.js v18+](https://nodejs.org/)
  * [Git](https://git-scm.com/)
  * Gerenciador de pacotes `npm` ou `yarn`.

### 1\. Clonando o Repositório (Importante)

Como este repositório utiliza submódulos, você deve cloná-lo de forma recursiva para baixar também o código do front e do back:

```bash
git clone --recurse-submodules https://github.com/otaviocostao/ava-project.git
cd ava-project
```

*Caso já tenha clonado sem os submódulos, execute:*

```bash
git submodule update --init --recursive
```

### 2\. Configurando o Backend

1.  Acesse a pasta do backend:
    ```bash
    cd ava-backend
    ```
2.  Instale as dependências:
    ```bash
    npm install
    ```
3.  Crie um arquivo `.env` na raiz do backend seguindo o exemplo do `.env.example` (configure suas credenciais do Supabase/Postgres).
4.  Execute o projeto:
    ```bash
    npm run start:dev
    ```

### 3\. Configurando o Frontend

1.  Em um novo terminal, acesse a pasta do frontend:
    ```bash
    cd AVA-UNIFAN
    ```
2.  Instale as dependências:
    ```bash
    npm install
    ```
3.  Crie um arquivo `.env.local` na raiz do frontend com as variáveis necessárias (ex: URL da API).
4.  Execute o projeto:
    ```bash
    npm run dev
    ```
