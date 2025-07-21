# Aula 3 – Criando um repositório Git local

## 🎯 Objetivo
Aprender a criar um repositório Git local, entender o que é um repositório e realizar as primeiras operações básicas.

---

## 🗂️ O que é um repositório Git?
Um repositório é uma pasta monitorada pelo Git. Quando você transforma uma pasta em repositório, o Git passa a rastrear todas as mudanças nos arquivos dela, permitindo versionamento, histórico e colaboração.

---

## 🧪 Passo 1 – Criar uma pasta do projeto
No terminal (Git Bash, CMD ou Terminal do Linux/macOS), crie uma nova pasta e acesse-a:
```bash
mkdir meu-projeto
cd meu-projeto
```

---

## 🛠️ Passo 2 – Iniciar o Git na pasta
Para transformar a pasta em um repositório Git, execute:
```bash
git init
```
Você verá uma mensagem como:
```
Initialized empty Git repository in ...
```
O Git criou uma subpasta oculta chamada `.git`, onde ficam todas as informações de versionamento.

---

## 📄 Passo 3 – Criar um arquivo para teste
Crie um arquivo chamado `index.html`:
```bash
echo "<h1>Olá Git!</h1>" > index.html
```
Para conferir o conteúdo do arquivo:
```bash
cat index.html
```

---

## 🕵️ Passo 4 – Verificar o status do repositório
Veja o que o Git está monitorando:
```bash
git status
```
O Git mostrará que existe um arquivo "untracked" (não rastreado ainda). Isso significa que o arquivo foi criado, mas ainda não está sendo versionado pelo Git.

---

## 💡 Dicas Úteis
- O comando `git init` só precisa ser executado uma vez por projeto.
- A pasta `.git` é oculta. Não apague ou edite manualmente!
- Use `ls -a` para ver arquivos ocultos (Linux/macOS/Git Bash).
- Sempre use `git status` para acompanhar o que mudou no seu projeto.

---

## 🔗 Links Úteis
- [Documentação Oficial do Git – git init](https://git-scm.com/docs/git-init)
- [O que é um repositório? (GitHub Docs)](https://docs.github.com/pt/repositories/creating-and-managing-repositories/about-repositories)

---

## ✅ Checklist de Tarefas
- [ ] Crie a pasta do projeto com `mkdir meu-projeto`
- [ ] Acesse a pasta com `cd meu-projeto`
- [ ] Inicie o repositório com `git init`
- [ ] Crie um arquivo `index.html`
- [ ] Use `git status` para verificar a situação

---

Pronto! Agora você tem um repositório Git local criado e já pode começar a versionar seus arquivos.