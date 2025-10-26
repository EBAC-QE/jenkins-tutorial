# Jenkins – Curso Prático com Node

Repositório de apoio às aulas práticas do curso **Integração Contínua com Jenkins**, com foco em projetos Node.js e automações de testes.

---

## 🎯 Objetivo do curso

Este curso apresenta de forma prática como usar o **Jenkins** para criar pipelines de CI/CD, integrando com projetos Node.js e Cypress.

Você aprenderá:
- Instalar e configurar o Jenkins no Windows e Mac
- Criar jobs *Freestyle* e *Declarativos*
- Executar testes automatizados no pipeline
- Trabalhar com variáveis de ambiente e relatórios
- Publicar resultados e logs

---

## ⚙️ Pré-requisitos gerais

Antes de começar, garanta que sua máquina possui:

```bash
java -version
git --version
node -v
npm -v
```

### Dependências básicas
- **Java 11 ou superior**
- **Git** (com opção “Add to PATH” habilitada)
- **Node.js e npm**
- **Navegador** (para acessar o Jenkins em `http://localhost:8080`)
- (Opcional) variável `NO_COLOR=1` para logs sem cores ANSI

---

## 🧩 Estrutura do repositório

| Aula | Título | Descrição |
|------|---------|------------|
| [Aula 1 – Freestyle Job](./aula-01-freestyle/README.md) | Criação do primeiro job no Jenkins e execução de um projeto Node |
| Aula 2 – Pipeline Declarativo | Introdução ao Jenkinsfile e pipeline automatizado |
| Aula 3 – Variáveis e Ambientes | Como parametrizar e isolar ambientes no Jenkins |
| Aula 4 – Publicação de Relatórios | Geração e publicação de relatórios de testes |
| Aula 5 – Boas Práticas CI/CD | Estrutura e estratégias de automação em pipeline |

---

## 🚀 Como usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/<seu-usuario>/jenkins-course.git
   ```

2. Acesse a aula desejada:
   ```bash
   cd jenkins-course/aula-01-freestyle
   ```

3. Siga o passo a passo do `README.md` de cada aula.

---

## 🔗 Recursos úteis

- [Documentação oficial do Jenkins](https://www.jenkins.io/doc/)
- [Download do Jenkins LTS](https://www.jenkins.io/download/)
- [Node.js](https://nodejs.org)
- [Git SCM](https://git-scm.com/downloads)
- [Cypress](https://www.cypress.io)

---

## 👨‍🏫 Autor

Curso criado por **Fábio Araújo** – QA Lead & Professor de Engenharia de Qualidade.  
Material voltado para o ensino prático e aplicação real em pipelines de integração contínua.
