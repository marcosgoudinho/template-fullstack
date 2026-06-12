# Template Fullstack

Template base para criação de projetos fullstack com foco em boas práticas de desenvolvimento, organização de código, versionamento, automação e escalabilidade.

## Objetivo

Este repositório serve como ponto de partida para novos projetos, reduzindo o tempo de configuração inicial e garantindo uma estrutura consistente entre aplicações.

Os componentes e tecnologias específicas serão adicionados conforme a necessidade de cada projeto, mantendo a flexibilidade para utilização com diferentes stacks.

---

## Estrutura do Projeto

```text
.
├── .github/
│   └── workflows/
├── docs/
├── frontend/
├── backend/
├── infra/
├── scripts/
├── .editorconfig
├── .gitignore
├── .env.example
├── README.md
└── LICENSE
```

### Diretórios

| Diretório  | Descrição                                                            |
| ---------- | -------------------------------------------------------------------- |
| `.github`  | Configurações de GitHub Actions, templates de issues e pull requests |
| `docs`     | Documentação do projeto                                              |
| `frontend` | Aplicação frontend                                                   |
| `backend`  | Aplicação backend                                                    |
| `infra`    | Arquivos de infraestrutura, deploy e containers                      |
| `scripts`  | Scripts auxiliares para desenvolvimento e automação                  |

---

## Fluxo de Branches

Este projeto utiliza uma adaptação simplificada do Git Flow.

### Branches Principais

| Branch    | Finalidade                                        |
| --------- | ------------------------------------------------- |
| `main`    | Código estável e pronto para uso                  |
| `develop` | Integração das funcionalidades em desenvolvimento |

### Branches Temporárias

#### Feature

Utilizada para desenvolvimento de novas funcionalidades.

```bash
git switch develop
git switch -c feature/nome-da-feature
```

Exemplo:

```text
feature/project-structure
feature/docker
feature/github-actions
```

#### Release

Utilizada para preparação de uma nova versão.

```bash
git switch develop
git switch -c release/v1.0.0
```

---

## Convenções

### Commits

Sugestão baseada em Conventional Commits:

```text
feat: adiciona autenticação
fix: corrige erro de validação
docs: atualiza documentação
refactor: reorganiza estrutura do projeto
test: adiciona testes unitários
chore: atualiza dependências
```

### Nomenclatura de Branches

```text
feature/nome-da-feature
release/vX.Y.Z
```

---

## Arquivos de Configuração

### .env.example

Utilizado como referência para criação do arquivo `.env`.

Nunca versionar arquivos contendo informações sensíveis.

### .editorconfig

Responsável pela padronização de formatação entre diferentes editores e IDEs.

### .gitignore

Define arquivos e diretórios que não devem ser versionados.

---

## Roadmap Inicial

* [x] Estrutura base do projeto
* [ ] Padronização de commits
* [ ] GitHub Actions
* [ ] Docker
* [ ] Testes automatizados
* [ ] Qualidade de código
* [ ] Observabilidade
* [ ] Deploy automatizado

---