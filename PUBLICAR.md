# Publicar em 3 passos

## 1. Criar o repositório

`github.com/new`
- Nome sugerido: `console-abm-datacentrics`
- **Public** (o Pages exige público fora do plano Enterprise)
- Não marcar "Add a README" — os arquivos já vêm prontos

> Se o repositório já existe de uma versão anterior, pule para o passo 2 e apenas
> substitua o `index.html`.

## 2. Subir os arquivos

**Pela interface web:**
1. Na página do repositório → **Add file → Upload files**
2. Arrastar `index.html`, `robots.txt`, `README.md` e `PUBLICAR.md`
3. Commit

O `.gitignore` precisa ser criado à parte: **Add file → Create new file**,
nome `.gitignore`, e colar o conteúdo do arquivo homônimo do pacote.

**Ou por linha de comando:**
```
git init
git add index.html robots.txt README.md PUBLICAR.md .gitignore
git commit -m "Console ABM DataCentrics V06"
git branch -M main
git remote add origin https://github.com/<usuario>/console-abm-datacentrics.git
git push -u origin main
```

> O arquivo tem 4,2 MB — abaixo do limite de 100 MB do GitHub.

## 3. Ligar o Pages

**Settings → Pages**
- Source: **Deploy from a branch**
- Branch: **main** · pasta **/ (root)**
- Save

Em 1 a 3 minutos o link aparece na própria página:
`https://<usuario>.github.io/console-abm-datacentrics/`

---

## Conferir depois de publicado

- [ ] Abre no **Mapa**, com o Brasil desenhado, a legenda por estado e o filtro do mapa
- [ ] **Contas** mostra os filtros e as 31 contas; clicar numa abre a página dela
- [ ] Dentro da conta, as abas **Comercial** e **Tecnologia** alternam
- [ ] **Decisores** filtra por conta, papel, senioridade e confiança de forma cumulativa
- [ ] Os avatares aparecem na lista de decisores
- [ ] No rail aparecem os quatro executivos: **Saucedo · Marissol · Ramos · Fagundes**, mais Outros
- [ ] Clicar em **Fagundes** mostra as 5 contas dele (Warren, Agibank, Ailos, Via Certa, Quanta)
- [ ] As 17 contas com DISC aparecem com etiqueta do executivo onde há dono
- [ ] A busca do topo devolve resultados de decisor, conta, produto e sinal
- [ ] O botão **↓ Pipedrive** baixa o CSV de um lead
- [ ] Só uma aba aparece por vez (sem sobreposição)

**Acessibilidade** — testar com o teclado, sem tocar no mouse:
- [ ] `/` foca a busca
- [ ] `↑ ↓` andam na lista de decisores e `Enter` abre a ficha
- [ ] `Tab` alcança as contas, os cartões de Sinais e os estados do mapa
- [ ] `Esc` fecha a ficha aberta

## Atualizar depois

Trocar o `index.html` no repositório. O Pages republica sozinho em 1–3 min.

## Se quiser fechar o acesso

O Pages é público por natureza. Para exigir login:
1. Adicionar o domínio ao **Cloudflare** (gratuito)
2. **Zero Trust → Access → Applications** → apontar para o Pages
3. Política: **e-mails permitidos**, listando quem da DCX pode entrar

Leva ~20 min e é gratuito até 50 usuários. O `noindex` já impede que o painel
apareça em busca, mas não impede acesso por quem tem o link.
