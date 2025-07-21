# Aula 10 – Boas Práticas e Fluxos Profissionais com Git/GitHub

## 🎯 Objetivo
Conhecer boas práticas, padrões profissionais e fluxos de trabalho recomendados para equipes que utilizam Git e GitHub.

---

## 🚦 1. Fluxo de trabalho Git para equipes (Git Flow Simplificado)
Um fluxo muito comum em times é:
- **main**: branch de produção (código estável)
- **develop**: branch principal de desenvolvimento
- **feature/***: novas funcionalidades (ex: `feature/login`)
- **fix/***: correções de bugs (ex: `fix/erro-login`)
- **hotfix/***: correções emergenciais na produção

### Exemplo de criação de branch:
```bash
git checkout develop
git checkout -b feature/pagina-login
```

---

## 📁 2. Organização dos Commits
- Commits devem ser claros e descritivos:
  - ✅ `git commit -m "Adiciona validação no formulário de login"`
  - 🚫 `git commit -m "alteração"`
- Use prefixos para facilitar a leitura do histórico:
  - `feat:` nova funcionalidade
  - `fix:` correção de bug
  - `refactor:` refatoração de código
  - `style:` ajustes de formatação/estilo
  - `docs:` documentação
  - `test:` testes

---

## 🔐 3. .gitignore é essencial
Evite versionar arquivos sensíveis ou desnecessários para o projeto. Exemplo de `.gitignore`:
```
node_modules/
.env
.DS_Store
dist/
```

---

## 🔄 4. Pull Requests (PRs) com revisão
- Faça push da branch no GitHub.
- Abra um PR no GitHub e explique o que foi feito.
- Peça revisão e comentários de colegas.
- Após aprovação, faça o merge.

---

## 🔒 5. Proteja sua branch main
No GitHub:
1. Vá em **Settings > Branches > Add Rule**.
2. Proteja a branch `main` para impedir push direto.
3. Exija aprovação de PR para merge.

---

## 💡 Dicas Finais
- Sempre atualize sua branch antes de abrir um PR: `git pull origin main`.
- Escreva mensagens de commit e PRs claras e objetivas.
- Use issues para organizar tarefas e bugs.
- Revise o código dos colegas e peça revisão do seu.

---

## 🔗 Links Úteis
- [Git Flow explicado (Atlassian)](https://www.atlassian.com/br/git/tutorials/comparing-workflows/gitflow-workflow)
- [Boas práticas de Git e GitHub (GitHub Docs)](https://docs.github.com/pt/get-started/quickstart/github-flow)
- [Como criar um .gitignore](https://git-scm.com/docs/gitignore)

---

## ✅ Checklist de Tarefas
- [ ] Crie branches seguindo o padrão `feature/`, `fix/`, `hotfix/`
- [ ] Escreva commits claros e com prefixos
- [ ] Use `.gitignore` para evitar arquivos desnecessários
- [ ] Abra PRs e peça revisão
- [ ] Proteja a branch `main` no GitHub

---

## 🎯 Resumo final do curso
Você aprendeu a:
- Criar repositórios locais e remotos
- Trabalhar com commits, branches e merges
- Resolver conflitos
- Usar GitHub com pull requests
- Aplicar boas práticas de versionamento

Parabéns por concluir o módulo! 🚀

