# Aula 7 – Branches: criando e gerenciando ramificações no Git

## 🎯 Objetivo
Aprender a criar, alternar, listar, deletar e mesclar branches (ramificações) no Git, entendendo sua importância para o desenvolvimento colaborativo e seguro.

---

## 🌿 O que é uma branch?
Uma branch (ramificação) é uma linha de desenvolvimento separada. Com ela, você pode trabalhar em funcionalidades, correções ou testes isoladamente, sem impactar o código principal (geralmente o `main` ou `master`). Isso facilita o trabalho em equipe e a organização do projeto.

---

## 🛠️ Comandos principais de branch

### 📌 Criar uma nova branch
```bash
git branch nome-da-branch
```

### 🔄 Mudar para outra branch
```bash
git checkout nome-da-branch
```

### 🚀 Criar e já mudar para a nova branch
```bash
git checkout -b nome-da-branch
```

### 🔍 Listar todas as branches
```bash
git branch
```
A branch atual aparece com `*` ao lado.

### 🧹 Deletar uma branch
```bash
git branch -d nome-da-branch
```

---

## 🤝 Merge: unindo branches
Depois de trabalhar em uma branch, você pode mesclar (merge) ela com o `main`:
```bash
git checkout main
git merge nome-da-branch
```
Se houver conflitos, o Git avisará e você precisará resolvê-los manualmente.

---

## 💡 Exemplo prático
```bash
# Crie uma nova branch
git checkout -b feature/cabecalho

# Faça mudanças no projeto (ex: adicione um cabeçalho no index.html)

# Adicione e comite
git add .
git commit -m "Adiciona cabeçalho"

# Volte para o main
git checkout main

# Mescle a nova branch com o main
git merge feature/cabecalho
```

---

## 💡 Dicas Úteis
- Use nomes descritivos para suas branches, como `feature/nome-da-funcionalidade` ou `bugfix/descricao`.
- Sempre faça o merge de branches que já foram revisadas/testadas.
- Para deletar uma branch remota: `git push origin --delete nome-da-branch`
- Para subir uma branch nova para o GitHub: `git push -u origin nome-da-branch`

---

## 🔗 Links Úteis
- [Documentação Oficial do Git – Branches](https://git-scm.com/book/pt-br/v2/Ramifica%C3%A7%C3%A3o-Branching-no-Git)
- [Como usar branches no GitHub (Docs)](https://docs.github.com/pt/github/collaborating-with-issues-and-pull-requests/about-branches)

---

## ✅ Checklist de Tarefas
- [ ] Crie uma branch chamada `feature/rodape`
- [ ] Adicione um rodapé no seu projeto
- [ ] Comite as alterações
- [ ] Volte para o `main` e faça o merge da branch
- [ ] Suba as alterações para o GitHub com `git push`
- [ ] (Opcional) Delete a branch local se não precisar mais dela

---

Pronto! Agora você já sabe como criar, gerenciar e mesclar branches no Git, tornando seu fluxo de trabalho mais seguro e organizado.

