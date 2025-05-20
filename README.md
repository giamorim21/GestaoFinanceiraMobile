# 💰 MiniApp Financeiro

Um aplicativo móvel simples e eficiente para gerenciamento de despesas diárias, com geração automática de relatórios semanais e login via Conta Google. Desenvolvido para a plataforma Android com foco em usabilidade, organização e boas práticas de desenvolvimento.

---

## 📚 Informações Gerais

- **Nome do Projeto:** MiniApp Financeiro  
- **Grupo:** [Nome dos integrantes do grupo]  
- **Disciplina:** [Nome da disciplina]  
- **Professor(a):** [Nome do professor(a)]  
- **Semestre:** 2025.1  

---

## 🧠 Descrição Geral

O **MiniApp Financeiro** é um aplicativo voltado para o controle financeiro pessoal. Com ele, o usuário pode registrar suas despesas diárias e visualizar relatórios semanais com informações detalhadas sobre seus gastos. O app utiliza **persistência de dados local** por meio do `RoomDatabase` e conta com **autenticação via Conta Google**, agregando segurança e inovação.

---

## 📋 Regras de Negócio

### 2.1. 📌 Cadastro de Despesas
- Registro de despesas diárias.
- Cada despesa contém:
  - Descrição (texto)
  - Valor (decimal positivo)
  - Data (selecionável)
  - Categoria (alimentação, transporte, lazer, etc.)
- Regras:
  - Descrição e valor são obrigatórios.
  - Valor deve ser maior que zero.

### 2.2. 💾 Armazenamento e Recuperação
- Persistência local com `RoomDatabase`.
- Dados mantidos mesmo após fechar o app.
- Permite consulta por **data** e **categoria**.

### 2.3. 📊 Relatório Semanal de Gastos
- Geração automática ao final de cada semana.
- Informações apresentadas:
  - Total semanal
  - Total por categoria
  - Média por dia
- Relatório é somente leitura.

### 2.4. 🔐 Autenticação com Conta Google
- Login obrigatório via API do Google.
- Dados vinculados à conta do usuário.
- Segurança contra acessos não autorizados.

---

## ✅ Casos de Uso

| ID    | Nome                     | Descrição                                                                 |
|-------|--------------------------|---------------------------------------------------------------------------|
| CU01  | Cadastrar Despesa        | Permite ao usuário inserir uma nova despesa com os campos obrigatórios.  |
| CU02  | Listar Despesas do Dia   | Exibe todas as despesas cadastradas no dia atual.                        |
| CU03  | Gerar Relatório Semanal  | Gera automaticamente o relatório com os totais e médias da semana.       |
| CU04  | Fazer Login com Google   | Permite o login usando a conta Google do usuário.                        |

---

## ⚠️ Restrições

- Aplicativo funciona **somente após o login** via Google.
- **Não** é permitido:
  - Despesas com valores negativos.
  - Campos obrigatórios em branco.
  - Geração manual de relatórios.
  - Edição ou exclusão de despesas após o cadastro (versão inicial).

---

## 📝 Considerações Finais

O **MiniApp Financeiro** foi desenvolvido com o objetivo de ser simples, funcional e eficaz para o controle de gastos diários. A autenticação via API do Google traz praticidade e segurança. O app atende a todos os critérios definidos no Plano de Ensino da disciplina.

---

## 🎥 Apresentação

- A apresentação será feita em aula, utilizando **emulador Android**.
- O foco será demonstrar o funcionamento do app e a experiência do usuário.
- O código-fonte **não será apresentado**, apenas o aplicativo em execução.

---

