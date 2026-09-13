# FHC-IA — Integrações relacionadas à LP

## Supabase

Projeto: `fhc-ia`
Região: São Paulo (`sa-east-1`)

A LP envia o pré-cadastro para:

`https://lhbsxhthxbvpddhakqbf.supabase.co/functions/v1/capture-prelead`

A função salva um pré-lead e retorna um código `VX-...` quando a captura é bem-sucedida.

## WhatsApp / YCloud

Identificador comercial da LP:

`VERTEX_GETULIO`

Webhook do FHC-IA usado no YCloud:

`https://lhbsxhthxbvpddhakqbf.supabase.co/functions/v1/ycloud-ingest`

O webhook secret NÃO está incluído neste pacote.

## Google Calendar

Regra comercial definida para o FHC-IA:

- segunda a sábado;
- das 09h às 18h;
- compromissos devem ser criados no calendário principal `Corretor`;
- antes de oferecer horário ao lead, a automação deve consultar conflitos nos calendários relevantes.

## Segurança

As tabelas do CRM usam RLS. A LP não deve receber service role key nem qualquer segredo de backend. O acesso sensível fica nas Edge Functions.
