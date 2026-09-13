# Vertex Getúlio — Landing Page Final

Versão final e autocontida da landing page do **Vertex Getúlio**, de Fernando Hamilton — Corretor de Imóveis, CRECI 25619.

## Estrutura

- `index.html` — página completa. CSS, JavaScript, imagens principais e favicon estão embutidos no próprio HTML.
- `vercel.json` — configuração mínima para deploy estático na Vercel.
- `.gitignore` — arquivos locais que não devem ir para o repositório.
- `docs/DEPLOY.md` — passo a passo para GitHub + Vercel.
- `docs/FHC-IA.md` — documentação das integrações atuais da LP com o FHC-IA.

## Integrações da página

- WhatsApp comercial: +55 75 98217-8857
- Identificador de origem comercial: `VERTEX_GETULIO`
- Google Ads: `AW-18445909721`
- Pré-cadastro FHC-IA: `https://lhbsxhthxbvpddhakqbf.supabase.co/functions/v1/capture-prelead`

## Pré-cadastro

Antes de abrir o WhatsApp, a página tenta salvar o formulário no FHC-IA. Quando o backend responde corretamente, a mensagem é aberta com uma referência no formato:

`Ref: VERTEX_GETULIO | Cadastro: VX-XXXXXXXXXX`

Se o backend estiver indisponível, o WhatsApp continua abrindo com `Ref: VERTEX_GETULIO`.

## Observação

Nenhuma senha, chave secreta do Supabase ou webhook secret do YCloud está incluída neste repositório.
