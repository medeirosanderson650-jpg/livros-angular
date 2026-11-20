# Livros Angular — Trabalho Prático DGT2809

Catálogo de livros desenvolvido em **Angular** para a disciplina *Aprofundamento em Desenvolvimento Front-End*.

## Funcionalidades

- **Catálogo** (`/lista`): tabela de livros com título, resumo, editora e autores, e botão de exclusão.
- **Novo** (`/dados`): formulário de cadastro de livro, com validação HTML5 (`ngNativeValidate`).
- Navegação interna com `routerLink` e `router-outlet`.
- Layout com **Bootstrap 5**.

## Estrutura

| Arquivo | Descrição |
|---|---|
| `src/app/editora.ts` | Classe `Editora` (codEditora, nome) |
| `src/app/livro.ts` | Classe `Livro` (codigo, codEditora, titulo, resumo, autores) |
| `src/app/controle-editora.service.ts` | Serviço com `getEditoras` e `getNomeEditora` |
| `src/app/controle-livros.service.ts` | Serviço com `obterLivros`, `incluir` e `excluir` |
| `src/app/livro-lista/` | Componente `LivroListaComponent` |
| `src/app/livro-dados/` | Componente `LivroDadosComponent` |
| `src/app/app-routing.module.ts` | Rotas `lista`, `dados` e rota padrão |
| `src/app/app.module.ts` | Módulo principal (FormsModule e providers) |

## Como executar

```bash
npm install
ng serve
```

Acesse `http://localhost:4200/` no navegador.
