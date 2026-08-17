# ABM DataCentrics — Console de decisores

Painel de inteligência do programa ABM 360°, entregue pela Esparta à DataCentrics.
Arquivo único, sem dependência externa — abre offline com duplo clique.

## Conteúdo

- **Mapa** — distribuição das 31 contas por estado e região
- **Contas** — comitê, roteamento, evidência de nuvem e stack por conta
- **Decisores** — 606 pessoas com papel, senioridade e ficha de abordagem
- **Contas com DISC** — 12 contas e 68 decisores com perfil comportamental,
  esteira de toques e copy pronta
- **Referência** — catálogo DCX v10, copy por papel, Challenger, battlecard,
  regra de stack, método WAR, cobertura, technográfico e geografia

## Como publicar

### GitHub Pages
1. Criar repositório e subir `index.html`, `robots.txt` e `.gitignore`
2. Settings → Pages → Source: `main` / root
3. O link fica em `https://<usuario>.github.io/<repo>/`

O `robots.txt` e a meta tag `noindex` impedem que o painel apareça em busca.
O link continua acessível a quem o tiver.

### Com controle de acesso (recomendado)
- **Cloudflare Access** na frente do Pages — gratuito até 50 usuários,
  libera por e-mail com código de uso único
- **Netlify** ou **Vercel** — arrastar o arquivo e ativar proteção por senha

## Procedência dos dados

| Camada | Origem |
|---|---|
| Decisores e cargos | LinkedIn (Apify), 07 e 16–17/08/2026 |
| Diretoria estatutária | RI oficial, 6-K/SEC e imprensa especializada |
| Evidência de nuvem | DNS de subdomínios de aplicação e serviços internos |
| Produtividade e SaaS | registros SPF e MX do domínio |
| Sinais de timing | troca de liderança, notícias e vagas abertas |
| DISC | análise comportamental por decisor (12 contas) |

## Limites declarados

- **O papel é inferido do cargo**, exceto os marcados como `validado`
  (fonte oficial ou curadoria manual). A coluna Confiança indica onde confiar.
- **Sinal de timing expira**: liderança 6 meses · M&A e captação 9–12 ·
  incidente 6 · vaga 3. Sem rescore mensal, a lista envelhece.
- **CDN mascara a origem**: onde há Akamai ou Cloudflare, o DNS não revela a
  nuvem. Nesses casos vale a declaração de quem opera.

## Governança

Dados de decisores tratados sob legítimo interesse para prospecção B2B,
com finalidade restrita à abordagem comercial. Não há decisão automatizada que
afete direitos do titular — o score prioriza a fila; a decisão de abordar é humana.

---
Esparta · Confidencial — DataCentrics
