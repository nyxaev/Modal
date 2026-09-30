# Modal
Modal Notes, bloco de notas HTML para anotações web.
# Modal Notes

Notas rápidas que abrem em um modal. Aperte **N**, escreva, salve.

Aplicativo web de arquivo único (HTML, CSS e JavaScript puros), sem dependências, sem build e sem servidor. As notas ficam salvas no próprio navegador.

## Recursos

- Criar, editar e excluir notas em um modal (usa o elemento nativo `<dialog>`)
- Cinco cores por nota, mostradas na faixa do card e do modal
- Busca instantânea por título e texto
- Exclusão com confirmação em dois cliques
- Tema claro e escuro automáticos, seguindo o sistema
- Layout responsivo, com navegação por teclado e foco visível
- Animações reduzidas para quem ativa "reduzir movimento" no sistema

## Atalhos

| Tecla | Ação |
| --- | --- |
| `N` | Abre uma nota nova |
| `/` | Foca a busca |
| `Ctrl` + `Enter` (ou `Cmd` + `Enter`) | Salva a nota no modal |
| `Esc` | Fecha o modal sem salvar |

## Como usar

**Localmente:** baixe o `index.html` e abra no navegador. Não precisa instalar nada.

**Online (GitHub Pages):**

1. Envie o `index.html` para um repositório no GitHub.
2. Vá em **Settings > Pages**.
3. Em **Source**, escolha **Deploy from a branch**, branch `main` e pasta `/ (root)`.
4. Em um ou dois minutos o app estará em `https://SEU_USUARIO.github.io/NOME_DO_REPOSITORIO/`.

## Onde ficam os dados

As notas são guardadas no `localStorage` do navegador, na chave `modal-notes:v1`.

- Os dados ficam só no seu aparelho e navegador. Nada é enviado para servidores.
- Limpar os dados do site apaga as notas.
- Outro navegador ou aparelho começa vazio.

## Personalização

Tudo está em `index.html`:

- **Cores das notas:** edite a lista `CORES` no começo do script.
- **Paleta e fontes da interface:** ajuste as variáveis CSS em `:root` (claro) e nos blocos de tema escuro.
- **Chave de armazenamento:** altere `KEY` se quiser separar os dados de outra instalação.

As fontes (Bricolage Grotesque e DM Sans) vêm do Google Fonts. Sem internet, o app usa fontes do sistema automaticamente.

## Estrutura

```
modal-notes/
├── index.html   # app completo (HTML + CSS + JS)
└── README.md
```

## Ideias para o futuro

- Fixar notas no topo
- Tags e filtros
- Exportar e importar notas em arquivo
- Sincronização entre aparelhos

## Licença

Defina a licença do seu projeto (por exemplo, MIT) e adicione um arquivo `LICENSE`.
