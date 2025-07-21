# Aula 2 – Instalando e Configurando o Git

## 🎯 Objetivo
Aprender a instalar o Git no seu sistema operacional, realizar a configuração inicial e verificar se tudo está funcionando corretamente.

---

## 🛠️ Passo 1 – Instalar o Git

### Windows
- Acesse: [git-scm.com](https://git-scm.com)
- Clique em **Download for Windows**.
- Execute o instalador baixado.
- Durante a instalação, mantenha as opções padrão (especialmente a opção "Git Bash Here").

### macOS
- Acesse: [git-scm.com](https://git-scm.com)
- Clique em **Download for macOS** e siga as instruções.
- Alternativamente, você pode instalar via Homebrew:
  ```bash
  brew install git
  ```

### Linux (Ubuntu/Debian)
- Abra o terminal e execute:
  ```bash
  sudo apt update
  sudo apt install git
  ```

---

## 🛠️ Passo 2 – Verificar se o Git foi instalado
Abra o terminal (ou Git Bash no Windows) e digite:
```bash
git --version
```
Se aparecer algo como `git version 2.43.0`, está tudo certo!

---

## 🧾 Passo 3 – Configurar seu usuário (global)
Digite os comandos abaixo no terminal, substituindo pelo seu nome e e-mail do GitHub:
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```
💡 Essa configuração define quem você é nos commits. Use o mesmo e-mail cadastrado no GitHub para associar seus commits ao seu perfil.

---

## 📄 Ver suas configurações
Para conferir se está tudo certo, digite:
```bash
git config --list
```
Você verá algo como:
```
user.name=Seu Nome
user.email=seu@email.com
```

---

## 💡 Dicas Úteis
- Sempre utilize o mesmo e-mail do seu GitHub para garantir que seus commits sejam reconhecidos na plataforma.
- Se precisar alterar o nome ou e-mail depois, basta rodar novamente os comandos de configuração.
- O Git Bash no Windows oferece um terminal mais amigável para comandos Git.
- No Linux/macOS, o terminal padrão já é suficiente.

---

## 🔗 Links Úteis
- [Download do Git](https://git-scm.com/downloads)
- [Documentação Oficial do Git](https://git-scm.com/doc)
- [Configurações do GitHub](https://github.com/settings/profile)

---

## ✅ Checklist de Tarefas
- [ ] Instale o Git no seu sistema operacional
- [ ] Abra o terminal (ou Git Bash)
- [ ] Configure seu nome e e-mail com os comandos acima
- [ ] Teste o comando `git --version`
- [ ] Teste o comando `git config --list`

---

Pronto! Agora você está com o Git instalado e configurado para começar a versionar seus projetos.