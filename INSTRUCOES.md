# Literatura na Escola

Este é um projeto de livro digital utilizando **mdBook**.

## Como usar localmente

Para visualizar o livro no seu computador enquanto escreve:

1. Abra o terminal na pasta do projeto.
2. Execute o comando:
   ```bash
   ../bin/mdbook serve --open
   ```
3. O livro abrirá no seu navegador em `http://localhost:3000`.

## Estrutura do Projeto

- `src/`: Contém os arquivos Markdown (.md) dos capítulos.
- `src/SUMMARY.md`: Define a ordem e o título dos capítulos na barra lateral.
- `book.toml`: Configurações gerais do livro.
- `book/`: Pasta gerada com o site final (não editar manualmente).

## Fluxo de Trabalho Antigravity (IA)

Toda vez que o Sérgio solicitar escrever, editar ou enviar:
1. **Editar/Criar**: Modificar os arquivos `.md` dentro de `src/`.
2. **Sumário**: Se um novo capítulo for criado, adicioná-lo ao `src/SUMMARY.md`.
3. **Build Local**: Rodar `../bin/mdbook build` para garantir que não há erros.
4. **Deploy**: Usar `git add .`, `git commit -m "mensagem"` e `git push origin main`.
   - **Nota**: As credenciais do GitHub já estão configuradas no ambiente local.

---
Desenvolvido por Prof. Sérgio Araújo - 2026
