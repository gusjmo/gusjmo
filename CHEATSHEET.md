# 📋 Git Cheatsheet — Guia de Referência Rápida

> Consulta rápida dos comandos Git mais usados no dia a dia.

---

## ⚙️ Configuração (só uma vez)

| Comando | O que faz |
|---|---|
| `git config --global user.name "Nome"` | Define seu nome nos commits |
| `git config --global user.email "email"` | Define seu e-mail |

---

## 🚀 Começando

| Comando | O que faz |
|---|---|
| `git init` | Inicia um repositório Git na pasta atual |
| `git clone <url>` | Baixa um repositório do GitHub para o computador |

---

## 🔄 Ciclo do dia a dia

| Comando | O que faz | Quando usar |
|---|---|---|
| `git status` | Mostra o que foi modificado | Sempre, antes de tudo |
| `git add .` | Adiciona todas as mudanças para staging | Antes do commit |
| `git add arquivo.py` | Adiciona um arquivo específico | Quando quer commitar só parte |
| `git commit -m "mensagem"` | Salva as mudanças localmente | Após o add |
| `git push origin main` | Envia commits para o GitHub | Após o commit |
| `git pull origin main` | Baixa mudanças do GitHub | Ao começar a trabalhar |

---

## 📜 Histórico

| Comando | O que faz |
|---|---|
| `git log` | Mostra histórico completo de commits |
| `git log --oneline` | Histórico resumido (uma linha por commit) |
| `git diff` | Mostra o que mudou nos arquivos (não commitado ainda) |

---

## 🌿 Branches

| Comando | O que faz |
|---|---|
| `git branch nome` | Cria uma nova branch |
| `git switch nome` | Muda para outra branch |
| `git checkout -b nome` | Cria e já muda para a branch |
| `git merge nome` | Une a branch na branch atual |
| `git branch` | Lista todas as branches |

---

## ↩️ Desfazendo erros

| Comando | O que faz | Risco |
|---|---|---|
| `git restore arquivo.py` | Descarta mudanças não salvas | ⚠️ Irreversível |
| `git reset --soft HEAD~1` | Desfaz último commit, mantém arquivos | Baixo |
| `git reset --hard HEAD~1` | Desfaz último commit e apaga mudanças | 🔴 Alto |

---

## ✅ Mensagens de commit (padrão profissional)

| Prefixo | Quando usar |
|---|---|
| `feat:` | Nova funcionalidade |
| `fix:` | Correção de bug |
| `docs:` | Atualização de documentação |
| `chore:` | Configurações, dependências |
| `test:` | Adição ou ajuste de testes |
| `refactor:` | Refatoração de código |

---

## 🗺️ Fluxo resumido

```
Editar arquivo
     ↓
git add .          → staging (área de preparo)
     ↓
git commit -m ""   → salvo localmente
     ↓
git push           → enviado pro GitHub
```

---

## 💡 Conceitos para entrevista

| Conceito | Definição |
|---|---|
| **Commit** | Snapshot do código em determinado momento |
| **Branch** | Linha de desenvolvimento paralela, sem afetar a main |
| **Merge** | Juntar duas branches |
| **Push/Pull** | Sincronizar com o repositório remoto |
| **Staging area** | Área intermediária entre editar e commitar (git add) |
| **Origin** | Nome padrão do repositório remoto (GitHub) |
