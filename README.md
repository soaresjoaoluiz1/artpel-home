# Art Pel — Home (artpelembalagens.com.br)

Página router da raiz do domínio. Hero split 50/50 que direciona o visitante pra uma das duas LPs:
- **Indústria** → `/industria/` (atendimento B2B sob medida)
- **Lojas e atacado** → `/lojas/` (revenda, linhas prontas)

## Stack

- HTML + CSS inline + JS vanilla (zero build)
- Tracking: Meta Pixel + Google Ads Tag — **somente PageView**, sem evento `Lead`/conversão (home é router, qualificação acontece nas LPs internas)
- SEO completo: Organization + LocalBusiness + WebSite schema, canonical, hreflang, sitemap unificado, manifest PWA

## Deploy

Pasta hospedada em `~/public_html/` (raiz) do user cPanel `artpelembalagens` na VPS HostGator.

```
sudo -u artpelembalagens -H bash -lc 'cd ~/public_html && git pull'
```

As duas LPs internas (`/industria/` e `/lojas/`) são repositórios separados clonados nas respectivas subpastas.
