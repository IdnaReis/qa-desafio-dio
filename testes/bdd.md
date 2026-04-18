# Testes BDD — SauceDemo

**Projeto:** Desafio QA DIO  
**Analista:** Idna Reis  
**Site testado:** https://www.saucedemo.com  
**Data:** Abril/2026  

---

## Funcionalidade: Login no sistema

### Cenário 1 — Login com sucesso

```gherkin
Dado que o usuário acessa https://www.saucedemo.com
Quando insere o usuário "standard_user"
E insere a senha "secret_sauce"
E clica no botão "Login"
Então o sistema redireciona para a página de produtos
E exibe a lista de produtos disponíveis
```

---

### Cenário 2 — Login com credenciais inválidas

```gherkin
Dado que o usuário acessa https://www.saucedemo.com
Quando insere o usuário "usuario_invalido"
E insere a senha "secret_sauce"
E clica no botão "Login"
Então o sistema exibe a mensagem de erro
"Username and password do not match any user in this service"
E o usuário permanece na tela de login
```

---

### Cenário 3 — Login com campos vazios

```gherkin
Dado que o usuário acessa https://www.saucedemo.com
Quando deixa o campo de usuário em branco
E deixa o campo de senha em branco
E clica no botão "Login"
Então o sistema exibe a mensagem "Username is required"
E o usuário permanece na tela de login
```

---

### Cenário 4 — Login com usuário bloqueado

```gherkin
Dado que o usuário acessa https://www.saucedemo.com
Quando insere o usuário "locked_out_user"
E insere a senha "secret_sauce"
E clica no botão "Login"
Então o sistema exibe a mensagem
"Sorry, this user has been locked out"
E o acesso é negado
```

---

### Cenário 5 — Logout do sistema

```gherkin
Dado que o usuário está logado no sistema como "standard_user"
Quando clica no menu hambúrguer
E clica na opção "Logout"
Então o sistema encerra a sessão
E redireciona o usuário para a tela de login
```
