# TrybeWarts 🧙‍♂️✨

Projeto de estudo desenvolvido durante a formação em **Desenvolvimento Web da Trybe**.  
Uma aplicação backend que simula a lógica de uma escola de magia inspirada em Harry Potter, com regras de personagens, casas e interações.

---

## ⚡ Sobre o projeto

O *TrybeWarts* é uma API construída em **Node.js** que permite:

✔️ Criar e listar personagens  
✔️ Distribuir personagens em casas  
✔️ Aplicar regras e validações da lógica de sistema  
✔️ Filtrar por características (casa, nome, etc.)  
✔️ Retornar respostas consistentes com boas práticas de API

Esse projeto foi desenvolvido para consolidar:

- Manipulação de dados via rotas REST  
- Lógica de negócio expressa em funções claras  
- Validações e tratamento de erros  
- Testes automatizados  
- Estruturação de projeto backend

---

## 🛠️ Tecnologias utilizadas

- **Node.js**
- **JavaScript**
- **Express**
- **Testes** (Jest / Mocha & Chai / Sinon, conforme implementação)
- **ESLint** (configuração de estilo)

---

## 🚀 Como rodar localmente

### 1. Clone o repositório

```bash
git clone https://github.com/Thaisvc/Poject-TrybeWarts.git
cd Poject-TrybeWarts
````

---

### 2. Instale as dependências

```bash
npm install
```

ou

```bash
yarn install
```

---

### 3. Inicie o servidor

```bash
npm start
```

ou

```bash
npm run dev
```

A API deverá estar disponível em:

```
http://localhost:3000
```

---

## 📡 Endpoints e exemplos de uso

### 🔹 Listar personagens

**GET /characters**

**Resposta**

```json
[
  {
    "id": 1,
    "name": "Harry Potter",
    "house": "Gryffindor"
  }
]
```

---

### 🔹 Buscar personagem por ID

**GET /characters/:id**

**Resposta**

```json
{
  "id": 3,
  "name": "Hermione Granger",
  "house": "Gryffindor"
}
```

---

### 🔹 Criar personagem

**POST /characters**

**Requisição**

```json
{
  "name": "Luna Lovegood",
  "house": "Ravenclaw"
}
```

**Resposta**

```json
{
  "id": 6,
  "name": "Luna Lovegood",
  "house": "Ravenclaw"
}
```

---

### 🔹 Filtrar por casa

**GET /characters?house=Slytherin**

---

## 🔑 Regras de validação (exemplos)

✔️ `name`: obrigatória e não vazia
✔️ `house`: deve ser uma casa válida
✔️ IDs devem ser numéricos
✔️ Erros retornam status apropriado e mensagem clara

---

## 🧪 Testes

Para rodar os testes automatizados:

```bash
npm test
```

Os testes cobrem:

✔️ Rotas principais  <br>
✔️ Validações de entrada  <br>
✔️ Comportamento esperado em casos válidos  <br>
✔️ Tratamento de erros e respostas adequadas  <br>

---

## 📚 Aprendizado

Com esse projeto praticou:

✔️ Construção de API REST com Node.js  <br>
✔️ Organização de rotas e lógica backend  <br>
✔️ Tratamento de erros e mensagens consistentes  <br>
✔️ Cobertura de testes automatizados  <br>

Esses conhecimentos são aplicáveis em APIs reais e sistemas backend robustos.

---

