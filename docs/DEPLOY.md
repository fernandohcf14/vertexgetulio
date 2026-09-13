# Deploy via GitHub + Vercel

## 1. Subir no GitHub

Crie um repositório novo e envie todo o conteúdo desta pasta para a raiz do repositório.

A raiz deve ficar assim:

```text
index.html
vercel.json
README.md
.gitignore
docs/
```

## 2. Importar na Vercel

No painel da Vercel:

1. Add New → Project.
2. Importe o repositório do GitHub.
3. Framework Preset: **Other**.
4. Root Directory: `./`.
5. Build Command: deixe vazio.
6. Output Directory: deixe vazio.
7. Clique em Deploy.

Como a LP é estática e autocontida, não é necessário npm, Node, framework ou etapa de build.

## 3. Domínio

Depois do deploy, em Settings → Domains, associe o domínio desejado. Se estiver substituindo um projeto antigo, remova o domínio do projeto antigo antes de associá-lo ao novo.

## 4. Testes após deploy

Valide:

- carregamento da página em desktop e celular;
- logo horizontal no cabeçalho;
- formulário de pré-cadastro;
- abertura do WhatsApp;
- presença de `Ref: VERTEX_GETULIO` na mensagem;
- Google Ads `AW-18445909721` no HTML;
- chamada para `capture-prelead` antes do WhatsApp.
