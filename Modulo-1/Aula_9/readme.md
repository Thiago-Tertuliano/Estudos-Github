# Aula 9 – Lidando com Conflitos de Merge

## 🎯 Objetivo
Entender o que são conflitos de merge, como provocá-los, identificá-los e resolvê-los de forma segura no Git.

---

## 🧨 O que é um conflito?
Um conflito de merge acontece quando duas branches modificam a mesma parte de um arquivo de maneiras diferentes, e o Git não consegue decidir automaticamente qual mudança manter. É comum em trabalhos colaborativos e precisa ser resolvido manualmente.

---

## 📌 Exemplo prático de conflito
1. Estando na `main`, crie uma nova branch:
   ```bash
   git checkout -b feature/frase1
   ```
2. No arquivo `index.html`, adicione:
   ```html
   <p>Frase 1: Git é incrível!</p>
   ```
3. Faça commit e push:
   ```bash
   git add .
   git commit -m "Adiciona frase 1"
   git push origin feature/frase1
   ```
4. Volte para `main` e crie outra branch:
   ```bash
   git checkout main
   git checkout -b feature/frase2
   ```
5. No mesmo lugar do arquivo, adicione:
   ```html
   <p>Frase 2: GitHub facilita tudo!</p>
   ```
6. Commit e push:
   ```bash
   git add .
   git commit -m "Adiciona frase 2"
   git push origin feature/frase2
   ```
7. Tente mesclar as duas branches no `main` (primeiro uma, depois a outra). O Git vai mostrar um conflito.

---

## 🧩 Como o Git mostra o conflito?
Quando há conflito, o Git marca o trecho assim:
```html
<<<<<<< HEAD
<p>Frase 1: Git é incrível!</p>
=======
<p>Frase 2: GitHub facilita tudo!</p>
>>>>>>> feature/frase2
```
Você deve editar manualmente, escolhendo qual versão quer manter — ou fundindo as duas:
```html
<p>Frase 1: Git é incrível!</p>
<p>Frase 2: GitHub facilita tudo!</p>
```
Depois disso:
```bash
git add index.html
git commit -m "Resolve conflito entre frases"
```

---

## 💡 Dicas Úteis
- Sempre leia com atenção os marcadores de conflito (`<<<<<<<`, `=======`, `>>>>>>>`).
- Teste o projeto após resolver conflitos para garantir que tudo funciona.
- Comunique-se com o time para decidir a melhor resolução.
- Ferramentas como VS Code, GitKraken e Sourcetree facilitam a visualização e resolução de conflitos.

---

## 🔗 Links Úteis
- [Documentação Oficial do Git – Conflitos de Merge](https://git-scm.com/docs/git-merge#_merge_conflicts)
- [Como resolver conflitos no GitHub (Docs)](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts)

---

## ✅ Checklist de Tarefas
- [ ] Provoque um conflito de propósito seguindo os passos acima
- [ ] Resolva o conflito manualmente editando o arquivo
- [ ] Faça commit da resolução
- [ ] Teste o projeto para garantir que está funcionando

---

Pronto! Agora você já sabe como identificar e resolver conflitos de merge no Git.

