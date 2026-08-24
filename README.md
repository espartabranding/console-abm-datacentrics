# ABM DataCentrics — Console de Decisores (V06)

Painel de inteligência do programa ABM 360°, entregue pela Esparta à DataCentrics.
Arquivo único de 4,2 MB, sem dependência externa — abre offline com duplo clique.

## O que tem dentro

| Camada | Volume |
|---|---|
| Decisores com papel, senioridade e confiança | **606** em 31 contas |
| Avatares embutidos | 555 |
| Contas com comitê, roteamento e evidência de nuvem | **31** |
| Contas com perfil DISC completo | **17** · 117 decisores |
| Executivos responsáveis | 4 — Saucedo, Ramos, Fagundes e Marissol |
| Produtos do Catálogo DCX v10 | 13 |
| Copy por papel · Challenger · frameworks | 13 papéis |
| Contatos de CRM | 108 |

### Carteira DISC por executivo

| Executivo | Contas | Decisores |
|---|---|---|
| **Ramos** | 5 — Ademicon, Banco Pine, Banco Mercantil, Vialaser, AGI Tecnologia | 40 |
| **Fagundes** | 5 — Warren, Banco Agibank, Ailos, Via Certa, Quanta Previdência | 38 |
| **Saucedo** | 5 — Appmax, Banco Randon/Rands, Marcopolo, Grupo Argenta, Fruki | 27 |
| **Marissol** | 1 — ANDRA Electric Solutions | 7 |
| sem dono | 1 — Banco Bari | 5 |

## Abas

- **Mapa** — distribuição das contas por estado e região, com mapa interativo do Brasil e filtro próprio
- **Contas** — filtros por conta, região, porte, segmento, nuvem, roteamento e sinal;
  cada conta abre com comitê, ordem de entrada, roteamento e a aba de Tecnologia
- **Decisores** — busca e filtros cumulativos por conta, papel, senioridade e confiança;
  cada pessoa tem ficha de abordagem e exportação para Pipedrive
- **Sinais** — contas ordenadas pela força do gatilho, com o evento que abre a janela
- **Executivos** (no rail) — Saucedo, Marissol, Ramos, Fagundes e Outros; abre a carteira DISC de cada um
- **Referência** — catálogo, copy, Challenger, battlecard, regra de stack, método WAR,
  cobertura, technográfico e geografia

## Acessibilidade

Esta versão traz uma camada aditiva de acessibilidade:

- **Navegação por teclado** nos elementos que antes só respondiam ao mouse —
  conta no mapa e na lista, cartão de Sinais, estado no mapa, filtro lateral
- **Seleção exposta a leitor de tela** na lista de decisores
- **Atalhos visíveis**: `/` busca · `↑ ↓` andam na lista · `Enter` abre a ficha · `Esc` sai

A navegação por teclado que já existia na lista de decisores foi preservada — a
camada nova sai da frente dela em vez de sobrescrever.

## Procedência dos dados

| Camada | Origem |
|---|---|
| Decisores e cargos | LinkedIn via Apify, 07 e 16–17/08/2026 |
| Diretoria estatutária | RI oficial, 6-K/SEC e imprensa especializada |
| Evidência de nuvem | DNS de subdomínios de aplicação e de serviços internos |
| Produtividade e SaaS | registros SPF e MX do domínio |
| Sinais de timing | troca de liderança, notícias e vagas abertas |
| DISC | análise comportamental por decisor |

## Limites declarados

- **O papel é inferido do cargo**, exceto os marcados como `validado` (fonte oficial
  ou curadoria manual). A coluna Confiança indica onde confiar — e a validação por
  amostra ainda não foi feita.
- **Sinal de timing expira**: liderança 6 meses · M&A e captação 9–12 · incidente 6 ·
  vaga 3. Sem rescore mensal, a lista envelhece.
- **CDN mascara a origem**: onde há Akamai ou Cloudflare, o DNS não revela a nuvem.
  Nesses casos vale a declaração de quem opera, e o console diz isso na conta.
- **Cobertura atual: 31 de 400 contas** previstas em contrato.

## Publicar

1. Subir `index.html`, `robots.txt` e `.gitignore` na raiz do repositório
2. **Settings → Pages** → Source: `main` / root → Save
3. O link sai em `https://<usuario>.github.io/<repo>/`

A meta tag `noindex` e o `robots.txt` impedem que o painel apareça em busca.
O link segue acessível a quem o tiver.

Para exigir login, colocar **Cloudflare Access** na frente do Pages — gratuito
até 50 usuários, libera por e-mail com código de uso único.

## Governança

Dados de decisores tratados sob legítimo interesse para prospecção B2B, com
finalidade restrita à abordagem comercial. O perfilamento comportamental usa apenas
informação pública e profissional. Não há decisão automatizada que afete direitos do
titular — o score prioriza a fila; a decisão de abordar é humana.

---
Esparta · Confidencial — DataCentrics
