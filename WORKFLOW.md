Workflow do Projeto — Wiki de Projetos de Curso

1. Objetivo

Workflow de desenvolvimento e a política de commits do projeto **Wiki de Projetos de Curso**.

O projeto é dividido principalmente nas seguintes seções:

- **Índice:** página inicial com a listagem e navegação entre os projetos.
- **Páginas de Projetos:** páginas com informações detalhadas sobre cada projeto.
- **Contribua:** seção com orientações para alunos e colaboradores adicionarem ou atualizarem projetos.

----------------------

2. Modelo de Workflow

Será utilizado o **GitHub Flow**.

O GitHub Flow é um modelo baseado em uma branch principal (`main`) e branches de curta duração para desenvolvimento de funcionalidades ou correções.

O fluxo será:

main
  │
  ├── feature/nova-funcionalidade
  │          │
  │          └── Pull Request
  │                    │
  │                    ↓
  └───────────────→ main
----------------------

3. Estratégia de Branches

O projeto terá uma única branch principal:

main

Todas as alterações deverão ser desenvolvidas em branches separadas.

3.1 Tipos de branches

| Tipo | Padrão | Utilização |
|---|---|---|
| `feature/` | `feature/<descricao>` | Nova funcionalidade |
| `fix/` | `fix/<descricao>` | Correção de problema |
| `docs/` | `docs/<descricao>` | Alteração de documentação |
| `refactor/` | `refactor/<descricao>` | Refatoração do código |


As branches devem:

- ser criadas a partir da `main` atualizada;
- possuir nomes curtos e objetivos;
- utilizar letras minúsculas;
- utilizar `-` para separar palavras;
- representar uma única tarefa ou objetivo.

4. Origem e Destino dos Merges

O destino de todas as branches será a `main`.

main
  ↓
feature/*
  ↓
Pull Request
  ↓
Code Review
  ↓
main

Não será permitido realizar alterações diretamente na `main`.

----------------------

5. Atualização da Branch Principal

Antes de iniciar uma nova tarefa, o colaborador deverá atualizar sua cópia local da `main`:

git checkout main
git pull origin main

Depois disso, deverá criar sua branch:

git checkout -b feature/nome-da-funcionalidade

Durante o desenvolvimento, a branch deverá ser atualizada com a `main` quando houver alterações relevantes no projeto.

Antes de abrir ou finalizar um Pull Request, o colaborador deve verificar se sua branch está atualizada.

----------------------

6. Política de Revisão

Cada Pull Request deverá ser revisado por pelo menos 1 integrante do time antes do merge.

O revisor deverá verificar:

- se a funcionalidade atende ao requisito;
- se o código está organizado;
- se a alteração não causa problemas nas demais páginas;
- se os links estão funcionando;
- se a documentação está adequada;
- se os padrões definidos pelo projeto foram respeitados.

O autor deverá corrigir os problemas identificados antes da aprovação.

----------------------

7. Integração na `main`

O merge somente poderá ser realizado quando:

- o Pull Request estiver aprovado;
- os testes necessários tiverem sido executados;
- não existirem conflitos pendentes;
- os comentários importantes da revisão tiverem sido resolvidos.

Após o merge, a branch deverá ser excluída.

----------------------

8. Política de Commits Semânticos

Os commits deverão seguir o padrão:

tipo(escopo opcional): descrição

O escopo deve representar a seção ou parte do projeto afetada.

Escopos:

indice
projeto
contribua

----------------------


9. Tipos de Commit

9.1 Tipos convencionais

 Tipo - Quando utilizar 

`perf`   - Melhoria de desempenho
`build`  - Alterações relacionadas ao processo de build
`ci`     - Alterações na integração ou entrega contínua
`revert` - Reversão de uma alteração anterior

----------------------

10. Exemplos de Commits do Projeto

10.1 Índice

feat(indice): adiciona listagem de projetos

10.2 Página de projeto

feat(projeto): cria página do projeto de biblioteca

10.3 Contribua

docs(contribua): adiciona guia de contribuição