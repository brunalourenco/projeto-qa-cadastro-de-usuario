# Cenários Gherkin

## Objetivo

Documentar regras de negócios e auxiliar posteriormente na automação de testes.

## Funcionalidade: Realizar Cadastro de usuário

### Cenário: Cadastro de usuário já cadastrado anteriormente

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informar dados de um usuário já cadastrado anteriormente  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir a mensagem "Usuário já cadastrado"

---

### Cenário: Cadastro sem dados de usuário

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** deixar os dados de cadastro vazios  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir a mensagem "O campo nome deve ser preenchido"

---

### Cenário: Cadastro com campo nome contendo letras e números

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informar o campo nome com letras e números  
**E** informar os demais campos com dados válidos  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir mensagem de formato inválido para o campo nome

---

### Cenário: Cadastro com campo nome contendo apenas 1 letra

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informar um nome com apenas uma letra  
**E** informar os demais campos com dados válidos  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir a mensagem "Formato inválido. O campo nome deverá conter no mínimo 6 letras"

---

### Cenário: Cadastro com campo nome contendo apenas números

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informar apenas números no campo nome  
**E** informar os demais campos com dados válidos  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir a mensagem "Formato inválido. O campo nome deverá conter no mínimo 6 letras"

---

### Cenário: Cadastro com campo nome contendo caracteres especiais

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informar caracteres especiais no campo nome  
**E** informar os demais campos com dados válidos  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir a mensagem "Formato inválido. O campo nome deverá conter no mínimo 6 letras"

---

### Cenário: Cadastro sem preencher o e-mail

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** deixar o campo e-mail vazio  
**E** informar os demais campos com dados válidos  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir a mensagem "O campo e-mail deve ser preenchido corretamente"

---

### Cenário: Cadastro campo email formato incorreto

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informe email em formato inválido  
**E** informar os demais campos com dados válidos  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir mensagem "O campo e-mail deve ser preenchido corretamente"

---

### Cenário: Cadastro campo senha vazio

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informe campo de senha vazio
**E** informar os demais campos com dados válidos  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir mensagem de erro "O campo senha deve ter pelo menos 6 dígitos"

---

### Cenário: Cadastro campo senha com 5 números

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informe campo de senha com 5 números
**E** informar os demais campos com dados válidos  
**Então** o cadastro não deverá ser concluído  
**E** o sistema deverá exibir mensagem de erro "O campo senha deve ter pelo menos 6 dígitos"

---

### Cenário: Cadastro campo senha com 6 números

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informe campo de senha com 6 números
**E** informar os demais campos com dados válidos  
**Então** o cadastro será concluído  
**E** o sistema deverá redirecionar para página inicial
**E** exibir mensagem de cadastro concluído e de boas vindas

---

### Cenário: Cadastro campo senha com 7 números

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informe campo de senha com 7 números
**E** informar os demais campos com dados válidos  
**Então** o cadastro será concluído  
**E** o sistema deverá redirecionar para página inicial
**E** exibir mensagem de cadastro concluído e de boas vindas

---

### Cenário: Cadastro campo senha apenas com letras

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informe campo de senha apenas com letras
**E** informar os demais campos com dados válidos  
**Então** o cadastro não será concluído  
**E** o sistema deverá exibir mensagem de erro "O campo senha deve ter pelo menos 6 dígitos"

---

### Cenário: Cadastro senha apenas com caracteres especiais

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informe campo de senha apenas com caracteres especiais
**E** informar os demais campos com dados válidos
**Então** o cadastro não será concluído
**E** o sistema deverá exibir mensagem de erro "O campo senha deve ter pelo menos 6 dígitos"

---

### Cenário: Cadastro campo senha com números letras e caracteres especiais

**Dado** que esteja na página da Qazando Shop  
**E** clique no botão "Cadastro"  
**Quando** informe campo de senha com letras, número e caracteres especiais
**E** informar os demais campos com dados válidos
**Então** o cadastro não será concluído
**E** o sistema deverá exibir mensagem de erro "O campo senha deve ter pelo menos 6 dígitos"
