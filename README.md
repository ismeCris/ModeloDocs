<<<<<<< HEAD
# Site de Documentação da Equipe

Site de documentação criado com [MkDocs](https://www.mkdocs.org/) +
tema [Material](https://squidfunk.github.io/mkdocs-material/). Gratuito,
em Markdown, publicável no GitHub Pages.

## Rodar localmente

```bash
pip install -r requirements.txt
mkdocs serve
```

Abra `http://localhost:8000`.

## Publicar na web (GitHub Pages, grátis)

1. Crie um repositório novo no GitHub e suba esta pasta inteira para ele:
   ```bash
   git init
   git add .
   git commit -m "Primeira versão da documentação"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/NOME-DO-REPO.git
   git push -u origin main
   ```
2. No GitHub, vá em **Settings → Pages** e selecione a branch `gh-pages` como
   fonte (ela é criada automaticamente no primeiro deploy).
3. Edite o `site_url` no `mkdocs.yml` para o link real do seu GitHub Pages.
4. Pronto — a partir de agora, **todo `git push` na branch `main` publica o
   site sozinho** (via GitHub Actions, já configurado em
   `.github/workflows/deploy.yml`).

O site ficará disponível em algo como:
`https://SEU-USUARIO.github.io/NOME-DO-REPO/`

## Estrutura do projeto

```
documentacao/
├── mkdocs.yml              → configurações do site (título, menu, cores)
├── requirements.txt        → dependências
├── docs/
│   ├── index.md             → página inicial
│   ├── primeiros-passos.md
│   ├── arquitetura.md
│   ├── como-contribuir.md
│   ├── faq.md
│   └── assets/
│       └── imagens/         → TODAS as imagens do projeto ficam aqui
└── .github/workflows/deploy.yml → publica o site automaticamente
```

## Adicionar uma página nova

1. Crie o arquivo `.md` em `docs/`
2. Adicione o nome dela em `mkdocs.yml`, dentro de `nav:`

## Área Dev protegida por senha

A página `docs/dev/index.md` é criptografada com o plugin
`mkdocs-encryptcontent-plugin`. Só quem tem a senha consegue ler o conteúdo —
mesmo abrindo o HTML da página, o texto não aparece.

**Antes de publicar, troque a senha padrão!** Abra `mkdocs.yml` e mude:

```yaml
- encryptcontent:
    global_password: "TROQUE-ESTA-SENHA"
```

Para uma senha forte, de sua escolha. Depois compartilhe essa senha só com
quem precisa (ex: time de dev), por um canal seguro (não no próprio site).

Para criar mais páginas protegidas, basta adicionar no topo do arquivo `.md`:

```yaml
---
encrypted: true
---
```

## Adicionar uma imagem

1. Salve o arquivo em `docs/assets/imagens/`
2. Referencie na página: `![Descrição](assets/imagens/arquivo.png)`

Assim as imagens nunca ficam espalhadas pelo projeto — tudo centralizado numa
única pasta.
=======
# ModeloDocs
Paginas de documentação com mkdocs
>>>>>>> ad1edbed1815d7a3ba4291623689310282bf54d4
