# Bug Reports - Cadastro de Usuário

Os casos de teste completos e bug reports também estão disponíveis em formato Excel dentro do projeto.
<br>
[Clique e acesse a planilha]()
<br>

## BUG-001 - Cadastro de usuário já cadastrado anteriormente

### Caso de teste relacionado

CT-002

### Descrição

O sistema permite realizar cadastro utilizando um usuário previamente cadastrado.

### Resultado esperado

O sistema deve bloquear o cadastro e exibir mensagem:
"Usuário já cadastrado".

### Resultado obtido

Cadastro realizado com sucesso utilizando usuário já existente.

### Causa raiz

Falha na comunicação com banco de dados.

### Tipo

Back End

### Severidade

Alta

### Ambiente

Homologação

### Data

17/05/2026

### Responsável

Bruna Lourenço

### Evidências

![Bug 001 - print 1](evidencias/BUG 001/Bug 001 - print 1.png)
![Bug 001 -print 2](evidencias/BUG 001/Bug 001 - print 2.png)
![Bug 001 -print 3](evidencias/BUG 001/Bug 001 - print 3.png)
![Bug 001 -print 4](evidencias/BUG 001/Bug 001 - print 4.png)

---

## BUG-002 - Tipo de caractere inválido no campo nome

### Caso de teste relacionado

CT-004

### Descrição

O campo nome aceita preenchimento com letras e números.

### Resultado esperado

O sistema deve aceitar apenas letras no campo nome.

### Resultado obtido

Cadastro realizado normalmente utilizando caracteres inválidos.

### Causa raiz

Falha na validação de dados.

### Tipo

Front End

### Severidade

Média

### Ambiente

Homologação

### Data

17/05/2026

### Responsável

Bruna Lourenço

### Evidências

![Bug 002 - print 1](evidencias/BUG 002/Bug 002 - print 1.png)
![Bug 002 - print 2](evidencias/BUG 002/Bug 002 - print 2.png)

---

## BUG-003 - Ausência de limite mínimo de caracteres no campo nome

### Caso de teste relacionado

CT-005

### Descrição

O sistema permite cadastro utilizando apenas uma letra no campo nome.

### Resultado esperado

O campo nome deve exigir quantidade mínima de caracteres.

### Resultado obtido

Cadastro realizado normalmente com apenas uma letra.

### Causa raiz

Falha na validação de dados.

### Tipo

Front End

### Severidade

Média

### Ambiente

Homologação

### Data

17/05/2026

### Responsável

Bruna Lourenço

### Evidências

![Bug 003 - print 1](evidencias/BUG 003/Bug 003 - print 1.png)
![Bug 003 - print 2](evidencias/BUG 003/Bug 003 - print 2.png)

---

## BUG-004 - Campo nome aceita apenas números

### Caso de teste relacionado

CT-006

### Descrição

O campo nome aceita preenchimento somente com números.

### Resultado esperado

O sistema deve aceitar apenas caracteres alfabéticos.

### Resultado obtido

Cadastro realizado normalmente utilizando números.

### Causa raiz

Falha na validação de dados.

### Tipo

Front End

### Severidade

Média

### Ambiente

Homologação

### Data

17/05/2026

### Responsável

Bruna Lourenço

### Evidências

![Bug 004 - print 1](evidencias/BUG 004/Bug 004 - print 1.png)
![Bug 004 - print 2](evidencias/BUG 004/Bug 004 - print 2.png)

## BUG-005 - Tipo de caracter inválido para o campo nome

### Caso de teste relacionado

CT-007

### Descrição

O campo nome aceita preenchimento com caracteres especiais.

### Resultado esperado

O sistema deve aceitar apenas caracteres alfabéticos no campo nome.

### Resultado obtido

Cadastro realizado normalmente utilizando caracteres especiais no campo nome.

### Causa raiz

Falha na validação de dados.

### Tipo

Front End

### Severidade

Média

### Ambiente

Homologação

### Data

17/05/2026

### Responsável

Bruna Lourenço

### Evidências

![Bug 005 - print 1](evidencias/BUG 005/Bug 005 - print 1.png)
![Bug 005 - print 2](evidencias/BUG 005/Bug 005 - print 2.png)
