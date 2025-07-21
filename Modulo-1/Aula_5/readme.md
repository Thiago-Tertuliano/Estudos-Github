# Aula 5 – Visualizando o histórico de commits

## 🎯 Objetivo
Aprender a visualizar o histórico de commits, entender as diferenças entre versões e utilizar comandos para acompanhar a evolução do projeto.

---

## 📜 1. Ver o histórico completo de commits
Veja todos os commits feitos no repositório, do mais recente ao mais antigo:
```bash
git log
```
Esse comando exibe detalhes como hash do commit, autor, data e mensagem.

Exemplo de saída:
```
commit e5a4c3b2f2d5c4d1a1a4b2e7...
Author: Thiago <thiago@email.com>
Date:   Mon Jul 21 10:00 2025 -0300

    Adiciona arquivo index.html
```

---

## 🔍 2. Log com resumo (mais limpo)
Para ver um histórico mais compacto, use:
```bash
git log --oneline
```
Exemplo de saída:
```
e5a4c3b Adiciona arquivo index.html
```

---

## 📆 3. Ver mudanças entre commits
Veja as diferenças entre o último commit e o estado atual dos arquivos:
```bash
git diff
```
- Antes de um commit: mostra o que foi alterado desde o último commit.
- Após um commit: mostra a diferença entre o último commit e o estado atual.

Você também pode comparar dois commits específicos:
```bash
git diff <hash1> <hash2>
```

---

## 🧠 Dicas Importantes
- Use as setas do teclado para navegar no `git log` (pressione `q` para sair).
- O comando `git add .` adiciona todas as mudanças de uma vez (arquivos novos e modificados).
- Use sempre mensagens de commit claras para facilitar o entendimento do histórico.

---

## 🔗 Links Úteis
- [Documentação Oficial do Git – git log](https://git-scm.com/docs/git-log)
- [Documentação Oficial do Git – git diff](https://git-scm.com/docs/git-diff)
- [Entendendo o histórico de commits (GitHub Docs)](https://docs.github.com/pt/get-started/using-git/viewing-the-history-of-a-repository)

---

## ✅ Checklist de Tarefas
- [ ] Crie um novo arquivo `style.css`
- [ ] Use `git status` para verificar as mudanças
- [ ] Use `git add .` para adicionar tudo
- [ ] Faça um commit com uma mensagem clara
- [ ] Execute `git log` e `git log --oneline` para visualizar o histórico
- [ ] Use `git diff` para ver as diferenças entre versões

---

Pronto! Agora você já sabe como acompanhar o histórico e as mudanças do seu projeto com o Git.