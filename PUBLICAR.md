# Publicar em 3 passos

## 1. Criar o repositório

`github.com/new`
- Nome sugerido: `console-abm-datacentrics`
- **Public** (o Pages exige público fora do plano Enterprise)
- Não marcar "Add a README" — os arquivos já vêm prontos

## 2. Subir os arquivos

**Pela interface web:**
1. Na página do repositório novo → **uploading an existing file**
2. Arrastar `index.html`, `robots.txt`, `README.md` e `PUBLICAR.md`
3. Commit

O `.gitignore` precisa ser criado à parte: **Add file → Create new file**,
nome `.gitignore`, e colar o conteúdo do arquivo homônimo do pacote.

**Ou por linha de comando:**
```
git init
git add index.html robots.txt README.md PUBLICAR.md .gitignore
git commit -m "Console ABM DataCentrics V3"
git branch -M main
git remote add origin https://github.com/<usuario>/console-abm-datacentrics.git
git push -u origin main
```

> O arquivo tem 3,6 MB. Está bem abaixo do limite de 100 MB do GitHub, mas
> acima dos 50 MB o aviso aparece — não é o caso aqui.

## 3. Ligar o Pages

**Settings → Pages**
- Source: **Deploy from a branch**
- Branch: **main** · pasta **/ (root)**
- Save

Em 1 a 3 minutos o link aparece na própria página:
`https://<usuario>.github.io/console-abm-datacentrics/`

---

## Conferir depois de publicado

- [ ] Abre no **Mapa**, com o Brasil desenhado e a legenda por estado
- [ ] **Contas** mostra os filtros e as 31 contas; clicar numa abre a página dela
- [ ] Dentro da conta, as abas **Comercial** e **Tecnologia** alternam
- [ ] **Decisores** filtra por conta, papel, senioridade e confiança de forma cumulativa
- [ ] **Contas com DISC** abre com as 12, com etiqueta do executivo onde há dono
- [ ] Clicar em **Saucedo** ou **Marissol** no rail filtra as contas daquele executivo
- [ ] A busca do topo devolve resultados de decisor, conta, produto e sinal
- [ ] O botão **↓ Pipedrive** baixa o CSV de um lead

## Atualizar depois

Trocar o `index.html` no repositório. O Pages republica sozinho em 1–3 min.

## Se quiser fechar o acesso

O Pages é público por natureza. Para exigir login:
1. Adicionar o domínio ao **Cloudflare** (gratuito)
2. **Zero Trust → Access → Applications** → apontar para o Pages
3. Política: **e-mails permitidos**, listando quem da DCX pode entrar

Leva ~20 min e é gratuito até 50 usuários. O `noindex` já impede que o painel
apareça em busca, mas não impede acesso por quem tem o link.
