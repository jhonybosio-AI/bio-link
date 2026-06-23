# Página de Links — bio.jhonybosio.com 🔗

Esta é a página oficial de links (Linktree Premium) do assessor de investimentos **Jhony Bosio**. Foi desenvolvida em HTML/CSS estático com design premium, responsivo e focado em dispositivos móveis, seguindo as diretrizes visuais da marca.

---

## 🚀 Como Publicar na Vercel (Deploy Instantâneo)

Como o projeto é composto apenas por arquivos estáticos (`index.html` e `avatar.jpg`), a publicação é simples e gratuita:

### Passo 1: Inicializar o Repositório no GitHub
No terminal do seu Mac, na pasta do projeto:
```bash
git init
git add .
git commit -m "feat: first release of bio-link"
```
*(Crie um repositório vazio no seu GitHub chamado `bio-link` e vincule-o para subir os arquivos).*

### Passo 2: Fazer o Deploy na Vercel
1. Acesse o painel da [Vercel](https://vercel.com/) e clique em **Add New > Project**.
2. Importe o repositório `bio-link` do seu GitHub.
3. Clique em **Deploy**. A Vercel publicará o site e gerará um link temporário (ex: `bio-link.vercel.app`).

---

## 🌐 Como Configurar o Subdomínio `bio.jhonybosio.com`

Para mapear o subdomínio personalizado `bio.jhonybosio.com` para o seu deploy da Vercel:

### Passo 1: Adicionar o Domínio na Vercel
1. No painel do seu projeto na Vercel, vá em **Settings > Domains**.
2. Digite `bio.jhonybosio.com` e clique em **Add**.
3. A Vercel indicará que o domínio está aguardando a configuração de DNS.

### Passo 2: Configurar o DNS (no Cloudflare ou Hostgator)
Acesse a sua zona de DNS onde o domínio `jhonybosio.com` está configurado e adicione a seguinte entrada:

*   **Tipo (Type):** `CNAME`
*   **Nome (Name/Host):** `bio`
*   **Destino (Target/Value):** `cname.vercel-dns.com`
*   **TTL:** Automático ou 3600
*   **Status de Proxy (se usar Cloudflare):** Desative o proxy (deixe apenas em "DNS Only" - nuvem cinza) para a Vercel gerenciar o certificado SSL automaticamente.

Após salvar, a propagação costuma levar entre 5 e 30 minutos. Assim que concluído, o site estará no ar em **`https://bio.jhonybosio.com`**!
