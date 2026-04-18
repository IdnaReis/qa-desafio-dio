
# Histórias de Usuário — SauceDemo

**Projeto:** Desafio QA DIO  
**Analista:** Idna Reis  
**Data:** Abril/2026  

---

## US01 — Login

**Como** usuário,  
**Quero** fazer login no sistema com meu usuário e senha,  
**Para** acessar minha conta e visualizar os produtos disponíveis.

### Critérios de aceitação:
- O sistema deve aceitar credenciais válidas e redirecionar para a página de produtos
- O sistema deve exibir mensagem de erro para credenciais inválidas
- O sistema deve exibir mensagem de erro para campos vazios
- O sistema deve bloquear o acesso de usuários bloqueados

---

## US02 — Logout

**Como** usuário logado,  
**Quero** sair da minha conta,  
**Para** encerrar minha sessão com segurança.

### Critérios de aceitação:
- O sistema deve encerrar a sessão ao clicar em "Sair"
- O sistema deve redirecionar para a tela de login após o logout
- O sistema não deve permitir acesso às páginas internas após o logout
