# Testes BDD

## Funcionalidade: Login

### Cenário: Login com sucesso
Dado que o usuário está na página de login  
Quando ele insere um email válido  
E uma senha válida  
E clica no botão entrar  
Então ele deve ser redirecionado para a página inicial  

---

### Cenário: Login inválido
Dado que o usuário está na página de login  
Quando ele insere dados inválidos  
E clica no botão entrar  
Então o sistema deve exibir uma mensagem de erro  
