# Agenda Semanal

Um app simples de agenda/planner semanal — em um único arquivo HTML, sem backend, sem dependências para instalar. Os dados ficam salvos no navegador (`localStorage`).

## Funcionalidades

- Adicionar tarefas com **dia da semana, horário, categoria e notas**
- Repetir a mesma tarefa em vários dias de uma vez
- Marcar como concluída / remover
- Contador de tarefas pendentes por dia (nas abas) e total (no topo)
- Dados persistem entre sessões (localStorage do navegador)

## Como usar localmente

Basta abrir o arquivo `index.html` no navegador — não precisa de servidor nem instalação.

```bash
# Linux/Mac
open index.html
# ou
xdg-open index.html
```

## Como colocar no GitHub

1. Crie um repositório novo no GitHub (pelo site, sem README, sem .gitignore).
2. No terminal, dentro desta pasta:

```bash
git init
git add .
git commit -m "Primeira versão da agenda semanal"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/NOME-DO-REPO.git
git push -u origin main
```

Troque `SEU-USUARIO/NOME-DO-REPO` pelo endereço do seu repositório.

## Como publicar de graça (GitHub Pages)

Depois de subir o código:

1. No repositório, vá em **Settings → Pages**.
2. Em "Source", selecione a branch `main` e a pasta `/ (root)`.
3. Salve. Em alguns minutos seu app estará disponível em:
   `https://SEU-USUARIO.github.io/NOME-DO-REPO/`

Assim você acessa a agenda de qualquer dispositivo pelo navegador (os dados ficam salvos por navegador/dispositivo, já que usam localStorage — não sincronizam entre aparelhos diferentes).

## Possíveis melhorias futuras

- Sincronizar entre dispositivos (precisaria de um backend/banco de dados)
- Notificações/lembretes
- Visão mensal, além da semanal
- Exportar/importar tarefas em JSON
