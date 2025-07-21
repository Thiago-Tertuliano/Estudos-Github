# Aula 1 – O que são Git e GitHub?

## 🎯 Objetivo
Compreender o conceito de controle de versão, o papel do Git localmente e do GitHub na nuvem, além de aprender os primeiros comandos práticos.

---

## 🧠 Conceitos Fundamentais

### O que é Controle de Versão?
Controle de versão é um sistema que registra todas as alterações feitas em um arquivo ou conjunto de arquivos ao longo do tempo. Isso permite que você volte para versões anteriores, compare mudanças e colabore com outras pessoas sem perder nada.

### Git
- **Definição:** Sistema de controle de versão distribuído, criado por Linus Torvalds.
- **Para que serve:** Salvar “fotos” (commits) do seu código ao longo do tempo, facilitando o acompanhamento e a reversão de mudanças.
- **Onde roda:** Localmente, no seu computador.

### GitHub
- **Definição:** Plataforma online para hospedar repositórios Git.
- **Para que serve:** Backup, colaboração, portfólio público, gerenciamento de projetos.
- **Onde roda:** Na nuvem (web).

---

## 🛠️ Vantagens do Git
- Histórico completo do código
- Reversão de erros facilmente
- Trabalho em equipe sem sobrescrever código
- Organização por versões e ramificações (branches)
- Integração com diversas ferramentas

## 🛠️ Vantagens do GitHub
- Armazenamento gratuito de projetos
- Portfólio público para mostrar seu trabalho
- Pull Requests para colaboração e revisão de código
- Issues e Wiki para organização e documentação
- Integração com CI/CD, páginas web, entre outros

---

## ✅ Exemplo da Vida Real
Pense no Git como um “Ctrl+S” inteligente: além de salvar, ele guarda versões e permite voltar no tempo. Imagine escrever um livro e poder recuperar qualquer capítulo antigo, mesmo depois de várias alterações.

---

## 💻 Primeiros Passos Práticos

### 1. Crie sua conta no GitHub
Acesse: [github.com](https://github.com) e siga as instruções para criar sua conta gratuita.

### 2. Instale o Git
Baixe e instale em: [git-scm.com](https://git-scm.com)

### 3. Configure o Git no seu computador
Abra o terminal e execute:
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

### 4. Comandos Básicos do Git
- `git init` – Inicia um novo repositório Git na pasta atual
- `git status` – Mostra o status dos arquivos
- `git add <arquivo>` – Adiciona arquivos para serem versionados
- `git commit -m "mensagem"` – Salva as alterações com uma mensagem
- `git log` – Mostra o histórico de commits
- `git remote add origin <url>` – Conecta seu repositório local ao GitHub
- `git push -u origin main` – Envia seu código para o GitHub

### 5. Fluxo Básico de Trabalho
1. Faça alterações no código
2. Adicione as mudanças: `git add .`
3. Faça um commit: `git commit -m "Descreva o que mudou"`
4. Envie para o GitHub: `git push`

---

## 💡 Dicas Úteis
- Commits pequenos e frequentes facilitam o controle do projeto.
- Sempre escreva mensagens de commit claras e objetivas.
- Use branches para desenvolver novas funcionalidades sem afetar o código principal.
- Explore o GitHub: siga projetos, contribua, leia documentações.

---

## 🔗 Links Úteis
- [Documentação Oficial do Git](https://git-scm.com/doc)
- [Guia do GitHub para Iniciantes](https://docs.github.com/pt/get-started/quickstart)
- [GitHub Learning Lab](https://lab.github.com/)

---

## 📌 Tarefa
- [ ] Crie sua conta no GitHub (se ainda não tem)
- [ ] Instale o Git
- [ ] Configure seu nome e e-mail no Git
- [ ] Inicie um repositório local e faça seu primeiro commit
- [ ] Crie um repositório no GitHub e envie seu código para lá

