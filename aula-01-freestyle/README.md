# Aula 1 – Jenkins Freestyle Job (Windows e Mac)

## 🎯 Objetivo
Apresentar a execução do Jenkins em ambiente local e criar o primeiro job do tipo *Freestyle*, integrando com um projeto Node.js.

---

## 🧰 Pré-requisitos locais

### 1. Java 11 ou superior
Necessário para o Jenkins rodar.
```bash
java -version
```

### 2. Git
Necessário para clonar repositórios durante o build.  
Baixe em [https://git-scm.com/downloads](https://git-scm.com/downloads)
```bash
git --version
```
Marque a opção *Add Git to PATH* na instalação.

### 3. Node.js e npm
Para executar projetos Node (Cypress ou API tests).  
Baixe em [https://nodejs.org](https://nodejs.org)
```bash
node -v
npm -v
```

### 4. Variável NO_COLOR (opcional)
Remove cores ANSI dos logs.
- **Windows (cmd):**
  ```bash
  set NO_COLOR=1
  ```
- **macOS/Linux (zsh/bash):**
  ```bash
  export NO_COLOR=1
  ```

### 5. Verificação geral
```bash
java -version && git --version && node -v && npm -v
```

---

## ⚙️ Executando o Jenkins

### macOS (Homebrew)
```bash
brew services start jenkins-lts
```
Acesse [http://localhost:8080](http://localhost:8080)

### Windows
```bash
net start jenkins
```
Acesse [http://localhost:8080](http://localhost:8080)

Primeiro acesso → senha em:  
- macOS: `/Users/<usuario>/.jenkins/secrets/initialAdminPassword`  
- Windows: `C:\Program Files\Jenkins\secrets\initialAdminPassword`

Cole na tela inicial e instale os *plugins sugeridos*.

---

## 🧱 Criando o primeiro Freestyle Job

1. Painel → **New Item**
2. Tipo **Freestyle project**
3. Nome: `freestyle-node-demo`
4. *Source Code Management* → **Git** → URL do repositório
5. *Build Steps* → **Execute shell** (mac) ou **Execute Windows batch command**
6. Comandos:
   ```bash
   npm install
   npm test
   ```
7. **Save**
8. **Build Now**

---

## ✅ Validando a execução

No console:
- O repositório foi clonado.
- As dependências foram instaladas.
- Os testes rodaram com sucesso.

Se houver erros:
- Verifique se o **Git** e o **Node** estão no PATH.  
- Garanta que o Jenkins tenha acesso à internet.

---

## 🏁 Conclusão

Nesta aula você:
- Configurou o Jenkins localmente (Windows e macOS)
- Criou o primeiro job Freestyle
- Rodou um projeto Node de forma automatizada

➡️ Próxima aula: **Pipeline Declarativo com Jenkinsfile**
