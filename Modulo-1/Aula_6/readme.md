# Aula 6 – Criando um repositório no GitHub e conectando com o Git local

## 🎯 Objetivo
Aprender a criar um repositório no GitHub, conectar o repositório local ao remoto e enviar seus arquivos para a nuvem.

---

## 🧱 1. Criando um repositório no GitHub
1. Acesse [github.com](https://github.com) e faça login na sua conta.
2. Clique em **New repository** (ou **Novo repositório**).
3. Dê um nome ao projeto, ex: `meu-projeto-git`.
4. Escolha se será **público** ou **privado**.
5. **Desmarque** a opção de criar um README (pois já temos um repositório local).
6. Clique em **Create repository**.

---

## 🔗 2. Conectando seu projeto local ao GitHub
No terminal, dentro da pasta do seu projeto local, conecte ao repositório remoto:
```bash
git remote add origin https://github.com/seu-usuario/meu-projeto-git.git
```
(Substitua `seu-usuario` e o nome do repositório pelo seu usuário e projeto do GitHub)

---

## ☁️ 3. Enviando os arquivos para o GitHub
Envie seus commits locais para o repositório remoto:
```bash
git push -u origin main
```
Se o seu branch principal for chamado `master`, use `master` no lugar de `main`:
```bash
git push -u origin master
```

---

## 🔍 Verificando a conexão com o remoto
Para checar a URL do repositório remoto configurado:
```bash
git remote -v
```
Você verá algo como:
```
origin  https://github.com/seu-usuario/meu-projeto-git.git (fetch)
origin  https://github.com/seu-usuario/meu-projeto-git.git (push)
```

---

## 💡 Dicas Úteis
- O comando `git remote add origin ...` só precisa ser executado uma vez por projeto.
- Se precisar trocar a URL do remoto, use:
  ```bash
  git remote set-url origin https://github.com/novo-usuario/novo-repo.git
  ```
- Se aparecer erro de autenticação, verifique se está logado no GitHub e se está usando HTTPS ou SSH corretamente.
- Você pode criar repositórios privados para projetos pessoais.

---

## 🔗 Links Úteis
- [Criar um novo repositório no GitHub (Docs)](https://docs.github.com/pt/github/creating-cloning-and-archiving-repositories/creating-a-new-repository)
- [Documentação Oficial do Git – git remote](https://git-scm.com/docs/git-remote)
- [Como fazer push para o GitHub (Docs)](https://docs.github.com/pt/get-started/using-git/pushing-commits-to-a-remote-repository)

---

## ✅ Checklist de Tarefas
- [ ] Crie um novo repositório no GitHub com o nome `projeto-aula-git`
- [ ] Crie um projeto local simples (ex: `index.html`)
- [ ] Inicie o repositório local com `git init`, adicione e comite os arquivos
- [ ] Conecte com o repositório remoto usando `git remote add origin ...`
- [ ] Faça o `git push` para publicar o projeto no GitHub
- [ ] Verifique a conexão com `git remote -v`

---

Pronto! Agora você já sabe como publicar seus projetos no GitHub e compartilhar seu código com o mundo.

