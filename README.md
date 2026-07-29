# Manual online — Mytragor

Leitor mobile-first do manual **Como Jogar Mytragor**, pronto para hospedagem estática no GitHub Pages.

## Recursos

- Uma página do manual por tela
- Botões grandes de Anterior e Próxima no celular
- Gesto de deslizar para os lados
- Setas laterais e teclado no computador
- Contador de páginas
- URL individual para cada página (`#pagina-1`, `#pagina-2` etc.)
- Carregamento progressivo das imagens
- Respeito à área segura de aparelhos iPhone

## Testar antes de publicar

Abra o arquivo `index.html` no navegador. Para uma simulação mais fiel, use um servidor local, por exemplo, a extensão **Live Server** do VS Code.

## Publicar em `mytragor.com.br/comojogar`

### Caso `mytragor.com.br` já seja um site no GitHub Pages

1. Copie esta pasta inteira para uma pasta chamada `comojogar` dentro do repositório do site principal.
2. Faça commit e envie para o GitHub.
3. Acesse `https://mytragor.com.br/comojogar/`.

A estrutura no repositório principal ficará assim:

```text
/
├── index.html              # página inicial de mytragor.com.br
└── comojogar/
    ├── index.html
    ├── styles.css
    ├── script.js
    ├── manual_capa.png
    └── manual_pg1.png ... manual_pg17.png
```

### Caso ainda não exista um site principal

1. Crie um repositório para o site principal do domínio.
2. Ative o GitHub Pages em **Settings → Pages**.
3. Configure o domínio personalizado como `mytragor.com.br`.
4. No provedor onde comprou o domínio, configure os registros DNS indicados pelo GitHub.
5. Coloque estes arquivos na pasta `comojogar` desse repositório.

> O campo **Custom domain** do GitHub aceita somente o domínio (`mytragor.com.br`), não um caminho como `/comojogar`. O caminho é criado pela pasta dentro do site.

## Arquivos importantes

- `index.html`: estrutura da página
- `styles.css`: visual responsivo, com prioridade para celular
- `script.js`: navegação entre as páginas
- `manual_*.png`: páginas do manual

Não renomeie as imagens sem atualizar a lista `pages` no início do arquivo `script.js`.
