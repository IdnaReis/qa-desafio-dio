# Casos de Teste — SauceDemo

**Projeto:** Desafio QA DIO  
**Analista:** Idna Reis  
**Site testado:** https://www.saucedemo.com  
**Data:** Abril/2026  

---

## CT01 — Login com sucesso

| Campo | Descrição |
|---|---|
| **ID** | CT01 |
| **User Story** | US01 |
| **Título** | Login com credenciais válidas |
| **Pré-condição** | Usuário cadastrado no sistema |
| **Prioridade** | Alta |

**Passos:**
1. Acessar https://www.saucedemo.com
2. Inserir usuário: `standard_user`
3. Inserir senha: `secret_sauce`
4. Clicar no botão "Login"

**Resultado esperado:** Usuário é redirecionado para a página de produtos (`/inventory.html`) com sucesso.

**Resultado obtido:** ✅ Conforme esperado

---

## CT02 — Login com usuário inválido

| Campo | Descrição |
|---|---|
| **ID** | CT02 |
| **User Story** | US01 |
| **Título** | Login com usuário inexistente |
| **Pré-condição** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**
1. Acessar https://www.saucedemo.com
2. Inserir usuário: `usuario_invalido`
3. Inserir senha: `secret_sauce`
4. Clicar no botão "Login"

**Resultado esperado:** Sistema exibe mensagem de erro: *"Username and password do not match any user in this service"*

**Resultado obtido:** ✅ Conforme esperado

---

## CT03 — Login com senha inválida

| Campo | Descrição |
|---|---|
| **ID** | CT03 |
| **User Story** | US01 |
| **Título** | Login com senha incorreta |
| **Pré-condição** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**
1. Acessar https://www.saucedemo.com
2. Inserir usuário: `standard_user`
3. Inserir senha: `senha_errada`
4. Clicar no botão "Login"

**Resultado esperado:** Sistema exibe mensagem de erro informando credenciais inválidas.

**Resultado obtido:** ✅ Conforme esperado

---

## CT04 — Login com campos vazios

| Campo | Descrição |
|---|---|
| **ID** | CT04 |
| **User Story** | US01 |
| **Título** | Login sem preencher campos |
| **Pré-condição** | Nenhuma |
| **Prioridade** | Média |

**Passos:**
1. Acessar https://www.saucedemo.com
2. Deixar os campos de usuário e senha em branco
3. Clicar no botão "Login"

**Resultado esperado:** Sistema exibe mensagem de erro solicitando preenchimento dos campos obrigatórios.

**Resultado obtido:** ✅ Conforme esperado

---

## CT05 — Login com usuário bloqueado

| Campo | Descrição |
|---|---|
| **ID** | CT05 |
| **User Story** | US01 |
| **Título** | Tentativa de login com usuário bloqueado |
| **Pré-condição** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**
1. Acessar https://www.saucedemo.com
2. Inserir usuário: `locked_out_user`
3. Inserir senha: `secret_sauce`
4. Clicar no botão "Login"

**Resultado esperado:** Sistema exibe mensagem informando que o usuário está bloqueado.

**Resultado obtido:** ✅ Conforme esperado

---

## CT06 — Logout do sistema

| Campo | Descrição |
|---|---|
| **ID** | CT06 |
| **User Story** | US01 |
| **Título** | Logout com sucesso |
| **Pré-condição** | Usuário logado no sistema |
| **Prioridade** | Média |

**Passos:**
1. Fazer login com `standard_user` / `secret_sauce`
2. Clicar no menu hambúrguer (ícone superior esquerdo)
3. Clicar em "Logout"

**Resultado esperado:** Usuário é redirecionado para a tela de login e sessão é encerrada.

**Resultado obtido:** ✅ Conforme esperado

