# LITENET

Plataforma LITENET — gestão empresarial, parceiros, LITEPAY, LITE-LIFE, LITE-GAMES, LITE-DRIVER e mais.
App instalável (PWA) para Android, iPhone e computador, com a máscara como ícone.

## Ficheiros
- `index.html` — a aplicação completa
- `manifest.webmanifest`, `sw.js`, `icons/`, `favicon.ico` — tornam-na instalável e rápida
- `.nojekyll` — diz ao GitHub para publicar os ficheiros tal como estão

## Publicar no ar (GitHub Pages) — uma vez só

1. Entra em https://github.com e cria conta (ou entra).
2. Clica em **New repository**. Nome: `litenet`. Deixa **Public**. Clica **Create repository**.
3. Na página do repositório clica em **uploading an existing file**.
4. Descompacta o ZIP no computador e arrasta **todos os ficheiros e a pasta `icons`**. Clica **Commit changes**.
5. Vai a **Settings → Pages**. Em *Build and deployment* escolhe **Deploy from a branch**, branch **main**, pasta **/ (root)** e clica **Save**.
6. Espera 1 a 2 minutos. O endereço aparece no topo da página, assim:
   `https://O-TEU-UTILIZADOR.github.io/litenet/`

## Passos obrigatórios no Supabase (senão o login por email e os pagamentos não voltam ao sítio certo)
Supabase → **Authentication → URL Configuration**:
- **Site URL**: `https://O-TEU-UTILIZADOR.github.io/litenet/`
- **Redirect URLs**: acrescenta o mesmo endereço e o mesmo com `**` no fim (`https://O-TEU-UTILIZADOR.github.io/litenet/**`).

Se usares login com Google: no Google Cloud acrescenta o endereço acima às origens autorizadas.

## Instalar no telemóvel e no computador
- **Android (Chrome):** abre o endereço e toca no botão **Instalar app** (canto inferior esquerdo da página inicial), ou menu ⋮ → *Instalar app*.
- **iPhone (Safari):** toca em **Partilhar → Adicionar ao ecrã principal → Adicionar**. A página mostra estes passos quando tocas em *Instalar app*.
- **Computador (Chrome/Edge):** clica no botão **Instalar app** ou no ícone de instalar na barra de endereço.

## Atualizar mais tarde
No repositório clica em `index.html` → **Upload files** → substitui pelo ficheiro novo → **Commit changes**.
Em 1 a 2 minutos o site e as apps instaladas passam a abrir a versão nova.
