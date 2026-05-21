# Casos de Teste - Cadastro de Usuário

## Documentação completa

Os casos de teste completos também estão disponíveis em formato Excel dentro do projeto.
<br>
[Clique e acesse a planilha]()
<br>

## CT-001 - Cadastro de usuário válido

### Prioridade
Alta

### Pré-condição
Usuário não cadastrado

### Dados de entrada

| Campo | Valor |
|---|---|
| Nome | Bruna |
| Email | bruna@testes.com |
| Senha | 147852 |

### Passos
1. Acessar https://www.automationpratice.com.br/
2. Clicar em "Cadastro"
3. Inserir nome, email e senha
4. Clicar no botão "Cadastrar"

### Resultado esperado
- Cadastro realizado com sucesso
- Redirecionamento para página inicial
- Exibição de popup de boas-vindas

### Resultado obtido
- Cadastro realizado com sucesso
- Redirecionamento para página inicial
- Popup exibido corretamente

### Status
✅ Passou

---

## CT-002 - Cadastro de usuário já cadastrado

### Prioridade
Alta

### Pré-condição
Usuário previamente cadastrado

### Dados de entrada

| Campo | Valor |
|---|---|
| Nome | Bruna |
| Email | bruna@testes.com |
| Senha | 147852 |

### Passos
1. Acessar https://www.automationpratice.com.br/
2. Clicar em "Cadastro"
3. Inserir nome, email e senha
4. Clicar no botão "Cadastrar"

### Resultado esperado
- Sistema não deve concluir cadastro
- Exibir mensagem:
  "Usuário já cadastrado"

### Resultado obtido
- Usuário cadastrado com sucesso

### Status
❌ Falhou

---

## CT-003 - Cadastro sem preenchimento dos campos

### Prioridade
Alta

### Pré-condição
Usuário não cadastrado

### Dados de entrada
Campos vazios

### Passos
1. Acessar https://www.automationpratice.com.br/
2. Clicar em "Cadastro"
3. Não preencher os campos
4. Clicar em "Cadastrar"

### Resultado esperado
- Sistema não deve concluir cadastro
- Exibir mensagem:
  "O campo nome deve ser preenchido"

### Resultado obtido
- Mensagem exibida corretamente

### Status
✅ Passou

---

## CT-004 - Cadastro com nome contendo letras e números

### Prioridade
Alta

### Pré-condição
Usuário não cadastrado

### Dados de entrada

| Campo | Valor |
|---|---|
| Nome | Giovana27 |
| Email | gio@testes.com |
| Senha | 123456 |

### Passos
1. Acessar página de cadastro
2. Inserir dados informados
3. Clicar em "Cadastrar"

### Resultado esperado
- Sistema deve bloquear cadastro
- Exibir mensagem:
  "Formato inválido no campo nome"

### Resultado obtido
- Cadastro realizado com sucesso

### Status
❌ Falhou

