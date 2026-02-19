
# Casos de Uso do Sistema

## UC01 — Realizar Login
**Ator Principal:** Usuário

**Objetivo:** Permitir que o usuário acesse o sistema.

**Pré-condições:**
- Usuário deve possuir cadastro ativo.

**Pós-condições:**
- Sessão iniciada com sucesso.

**Fluxo Principal:**
1. O usuário informa e-mail e senha.
2. O sistema valida as credenciais.
3. O sistema autentica o usuário e redireciona para a tela inicial.

**Fluxos Alternativos:**
- **A1 — Senha incorreta:**
  - O sistema exibe mensagem de erro.
- **A2 — Conta bloqueada:**
  - O sistema impede o login e instrui o usuário a recuperar o acesso.

---

## UC02 — Recuperar Senha
**Ator Principal:** Usuário

**Objetivo:** Permitir que o usuário redefina sua senha caso a esqueça.

**Pré-condições:**
- Usuário deve ter uma conta registrada.

**Pós-condições:**
- Link de redefinição enviado ao e-mail do usuário.

**Fluxo Principal:**
1. O usuário solicita recuperação de senha.
2. O sistema solicita o e-mail cadastrado.
3. O usuário informa o e-mail.
4. O sistema envia link de redefinição para o e-mail informado.

**Fluxos Alternativos:**
- **A1 — E-mail não encontrado:**
  - O sistema informa que o e-mail não está associado a nenhuma conta.

---

## UC03 — Atualizar Perfil
**Ator Principal:** Usuário Autenticado

**Objetivo:** Permitir que o usuário atualize suas informações pessoais.

**Pré-condições:**
- Usuário deve estar autenticado.

**Pós-condições:**
- Informações atualizadas armazenadas no sistema.

**Fluxo Principal:**
1. O usuário acessa a área de perfil.
2. O usuário altera dados como nome, foto ou telefone.
3. O usuário confirma as alterações.
4. O sistema salva os novos dados e exibe confirmação.

**Fluxos Alternativos:**
- **A1 — Dados inválidos:**
  - O sistema rejeita e solicita correção.

