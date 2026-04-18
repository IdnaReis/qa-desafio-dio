
# Ciclo de Vida do Bug

**Projeto:** Desafio QA DIO  
**Analista:** Idna Reis  
**Data:** Abril/2026  

---

## Fluxo do ciclo de vida

```
Novo → Em análise → Em desenvolvimento → Em teste → Resolvido → Fechado
                         ↓
                     Rejeitado
```

---

## Descrição de cada status

| Status | Descrição |
|---|---|
| **Novo** | Bug identificado e registrado pelo QA |
| **Em análise** | Time de desenvolvimento avalia o bug |
| **Em desenvolvimento** | Desenvolvedor corrigindo o problema |
| **Em teste** | QA valida se a correção funcionou |
| **Resolvido** | Correção validada pelo QA com sucesso |
| **Fechado** | Bug encerrado após validação final |
| **Rejeitado** | Comportamento considerado esperado pelo time |

---

## Exemplo de registro de bug

| Campo | Descrição |
|---|---|
| **ID** | BUG-001 |
| **Título** | Mensagem de erro não exibida ao deixar campos vazios |
| **Ambiente** | Web — Chrome 120 / Windows 11 |
| **Severidade** | Média |
| **Prioridade** | Alta |
| **Status** | Fechado |
| **Reportado por** | Idna Reis |
| **Data** | Abril/2026 |

**Passos para reproduzir:**
1. Acessar https://www.saucedemo.com
2. Deixar os campos de usuário e senha em branco
3. Clicar no botão "Login"

**Resultado obtido:** Nenhuma mensagem de erro foi exibida.

**Resultado esperado:** Sistema deveria exibir a mensagem *"Username is required"*.

**Evidência:** Ver pasta `/evidências`

---

## Boas práticas no registro de bugs

- Sempre incluir passos detalhados para reprodução
- Informar ambiente (navegador, sistema operacional, versão)
- Anexar evidências (prints, vídeos)
- Classificar severidade e prioridade corretamente
- Manter o status atualizado durante todo o ciclo
