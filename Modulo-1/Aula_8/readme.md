# Aula 8 – Colaborando com Pull Requests no GitHub

## 🎯 Objetivo
Entender o que é um Pull Request, como criar, revisar e mesclar PRs no GitHub, promovendo colaboração, revisão de código e boas práticas em projetos.

---

## 🤔 O que é um Pull Request?
Um Pull Request (ou PR) é um pedido para que as mudanças de uma branch sejam revisadas e mescladas na branch principal (geralmente `main`). Isso permite revisões, comentários e testes antes que o código entre de fato no projeto oficial. É fundamental para colaboração em equipe!

---

## 🔄 Fluxo típico de trabalho com Pull Request
1. Crie uma branch (ex: `feature/login`)
2. Faça mudanças, commite e suba para o GitHub
3. No GitHub, clique em **Compare & pull request**
4. Escreva um título e uma descrição do que mudou
5. Abra o PR e aguarde revisão (ou revise você mesmo em projetos solos)
6. Após aprovado, clique em **Merge pull request**

---

## 📌 Exemplo prático
No terminal:
```bash
git checkout -b feature/contato
```
Faça mudanças no HTML/CSS/JS.

Adicione e comite:
```bash
git add .
git commit -m "Adiciona página de contato"
```
Suba a branch para o GitHub:
```bash
git push origin feature/contato
```
No GitHub, você verá a opção de abrir um Pull Request. Clique nela, escreva um bom título e descrição, e confirme.

Mescle o PR ou aguarde revisão de outro colaborador.

---

## 💡 Dicas de Ouro
- Nunca desenvolva direto na branch `main`. Use sempre branches + PRs.
- Escreva títulos e descrições claras nos PRs, explicando o que mudou e por quê.
- Use os comentários do PR para discutir melhorias ou dúvidas.
- PRs facilitam a revisão, testes e evitam conflitos no código.

---

## 🔗 Links Úteis
- [Documentação Oficial do GitHub – Pull Requests](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
- [Como criar um Pull Request (GitHub Docs)](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- [Boas práticas para Pull Requests (em inglês)](https://www.atlassian.com/git/tutorials/making-a-pull-request)

---

## ✅ Checklist de Tarefas
- [ ] Crie uma nova branch chamada `feature/sobre`
- [ ] Adicione uma seção "Sobre" ao seu projeto
- [ ] Comite e suba para o GitHub
- [ ] Abra um Pull Request e preencha título e descrição
- [ ] Mescle o PR no `main` após revisão

---

Pronto! Agora você já sabe como colaborar de forma profissional usando Pull Requests no GitHub.