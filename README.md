# Vice Burguer

Cardápio estático em HTML, CSS e JavaScript, com Vite. Os arquivos em `src/` contêm o código do cardápio, os estilos e as imagens. O Pixel da Meta usa o ID `3383402028501768` e registra o evento `PageView`.

## Rodar no computador

Use Node.js 24 e execute na pasta do projeto:

```sh
npm ci
npm run dev
```

Para gerar e conferir a versão de produção:

```sh
npm run build
npm run preview
```

## GitHub e Vercel

1. Extraia o ZIP e envie o conteúdo da pasta do projeto para um repositório no GitHub. O arquivo `package.json` deve ficar na raiz do repositório. Inclua também `package-lock.json` e `.gitignore`.
2. Na Vercel, importe o repositório pelo GitHub. Use a pasta que contém `package.json` e `vercel.json` como raiz do projeto e selecione o preset **Vite**. Desative as substituições manuais de **Build Command**, **Install Command** e **Output Directory** para usar o `vercel.json`. O build executa `npm ci --include=dev && npm run build` e publica `dist`. A instalação faz parte do build, por isso o comando de instalação separado está vazio.
3. Publique e abra a URL gerada pela Vercel para conferir a página.
4. No projeto da Vercel, abra **Settings → Domains**, adicione o seu domínio e configure no provedor do domínio os registros DNS indicados pela Vercel. Aguarde o painel confirmar o domínio e o HTTPS.
5. Use a URL HTTPS do seu domínio nos anúncios. No Gerenciador de Eventos da Meta, abra **Testar eventos** e acesse essa URL para confirmar o recebimento do `PageView`.

[Vite na Vercel](https://vercel.com/docs/frameworks/frontend/vite) · [Configurar domínio próprio](https://vercel.com/docs/domains/working-with-domains/add-a-domain)
