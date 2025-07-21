# Aula 4 – Adicionando arquivos e criando o primeiro commit

## 🎯 Objetivo
Aprender a adicionar arquivos ao controle de versão do Git e realizar o primeiro commit, entendendo o que cada etapa representa.

---

## 🔍 O que é um commit?
Um commit é como um “salvamento” do seu projeto. Cada commit armazena o estado dos arquivos naquele momento, junto com uma mensagem explicando o que foi feito. Assim, você pode acompanhar o histórico de mudanças e reverter se necessário.

---

## 🧪 Etapas para fazer um commit

### 1. Verifique o status do repositório
Veja quais arquivos foram modificados ou criados:
```bash
git status
```
Você verá algo como:
```
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
```

### 2. Adicione o arquivo ao staging area
Inclua o arquivo que deseja versionar:
```bash
git add index.html
```
Esse comando diz: "Quero incluir esse arquivo no próximo commit".

### 3. Verifique o status novamente
Confira se o arquivo está pronto para ser commitado:
```bash
git status
```
Agora você verá:
```
Changes to be committed:
  new file:   index.html
```

### 4. Faça o commit
Salve oficialmente o arquivo no histórico do Git:
```bash
git commit -m "Adiciona arquivo index.html"
```
A flag `-m` serve para escrever a mensagem de commit direto no terminal. Escreva mensagens claras e objetivas!

---

## 🧠 Dicas Importantes
- `git add` → seleciona arquivos para o próximo commit (staging area).
- `git commit` → salva oficialmente os arquivos adicionados no histórico do repositório.
- Você pode adicionar vários arquivos de uma vez: `git add .` (adiciona todos os arquivos modificados/criados).
- Use mensagens de commit que expliquem claramente o que foi feito.

---

## 🔗 Links Úteis
- [Documentação Oficial do Git – git add](https://git-scm.com/docs/git-add)
- [Documentação Oficial do Git – git commit](https://git-scm.com/docs/git-commit)
- [Como escrever boas mensagens de commit (em inglês)](https://cbea.ms/git-commit/)

---

## ✅ Checklist de Tarefas
- [ ] Verifique o status com `git status`
- [ ] Adicione o arquivo `index.html` com `git add index.html`
- [ ] Faça seu primeiro commit com uma mensagem clara usando `git commit -m "mensagem"`
- [ ] Use `git status` novamente para ver se o diretório está limpo

---

Pronto! Agora você já sabe como adicionar arquivos e criar commits no seu repositório Git.