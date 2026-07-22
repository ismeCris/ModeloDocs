# Perguntas Frequentes

### O site atualiza sozinho quando eu edito?
Sim, se você configurou o deploy automático via GitHub Actions (veja o
`README.md` do projeto). Toda vez que alguém aprova um Pull Request, o site é
publicado de novo automaticamente.

### Preciso saber programar para editar?
Não. Basta escrever em Markdown, que é bem parecido com texto normal. Você
pode inclusive editar direto pelo site do GitHub, sem instalar nada.

### Onde ficam as imagens?
Em `docs/assets/imagens/`. Todas centralizadas ali, então não há risco de
espalhar arquivos soltos pelo projeto.

### Como faço uma página só minha equipe ver?
O MkDocs gera um site estático público por padrão. Se precisar de acesso
restrito, publique num repositório privado do GitHub com GitHub Pages (plano
pago) ou hospede internamente (ex: intranet da empresa).
