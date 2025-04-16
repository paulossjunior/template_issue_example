# 📋 Templates de Issues

Este repositório contém modelos padronizados para criar issues no GitHub. Cada template tem uma finalidade específica: reportar bugs, propor novas funcionalidades ou registrar tarefas operacionais.

---

## 🐞 `BUG_TEMPLATE.md`

Modelo para relatar **erros, falhas ou comportamentos inesperados** no sistema.

### 🔧 Estrutura:
- **Título:** `[BUG] O título do erro`
- **Descrição do Bug**
- **Comportamento Observado**
- **Comportamento Esperado**
- **Informações Adicionais**

### 📌 Exemplo:

```md
title: "[BUG] Erro ao salvar formulário de cadastro"

# Descrição do Bug
O botão "Salvar" não responde ao clique no navegador Firefox.

## Comportamento Observado
Ao clicar em "Salvar", nada acontece. Nenhuma requisição é feita (verificado no DevTools).

### Comportamento Esperado
Ao clicar, o formulário deveria ser validado e uma requisição POST deveria ser enviada para `/api/usuario`.

# Informações Adicionais
- Navegador: Firefox 123
- SO: Ubuntu 22.04
- Logs: Nenhum erro no console.
```

---

## ✨ `FEATURE_TEMPLATE.md`

Modelo para propor e descrever **novas funcionalidades** que entreguem valor ao cliente.

### 🔧 Estrutura:
- **Título:** `[FEATURE] Nome da funcionalidade`
- **Descrição**
- **Requisitos Técnicos**
- **Atividades a serem realizadas**
- **Critérios de Aceitação**
- **Observações**

### 📌 Exemplo:

```md
title: "[FEATURE] Adicionar autenticação via Google"

# Descrição
Permitir que os usuários façam login utilizando sua conta do Google.

## Requisitos Técnicos
- Usar OAuth 2.0
- Integrar com a biblioteca `react-oauth/google`

# Atividades a serem realizadas
- [ ] Criar botão "Login com Google"
- [ ] Implementar integração OAuth
- [ ] Armazenar token no localStorage

# Critérios de Aceitação (Feature-Level)
- O usuário consegue fazer login com sua conta Google
- Os dados do perfil são salvos na base local
- O sistema reconhece o usuário autenticado

## Observações
A funcionalidade deve funcionar em desktop e mobile.
```

---

## 📌 `TASK_TEMPLATE.md`

Modelo voltado para **tarefas operacionais**, como reuniões, documentação ou organização do projeto.

### 🔧 Estrutura:
- **Título:** `[TASK] Nome da tarefa`
- **Objetivo da Tarefa**
- **Entregáveis**
- **Observações**

### 📌 Exemplo:

```md
title: "[TASK] Criar documentação da API"

# Objetivo da Tarefa
Documentar os endpoints da API no Swagger.

# Entregáveis
- [ ] Adicionar anotação OpenAPI em todos os endpoints
- [ ] Atualizar rota `/docs` com Swagger UI
- [ ] Validar se a documentação está acessível em produção

## Observações
Colaborar com o time de backend para entender o fluxo das rotas.
```

---

## ✅ Boas Práticas

- Use os prefixos `[BUG]`, `[FEATURE]`, e `[TASK]` para facilitar a triagem.
- Preencha todos os campos de forma clara.
- Sempre associe a issue ao pull request correspondente.
- Utilize checklists para facilitar o acompanhamento.
- Adicione prints ou evidências sempre que possível.
