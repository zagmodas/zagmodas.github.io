# Zag Modas — Biosite

Página de links da **Zag Modas** — *A moda dos que vivem*. Endereço:
**https://zagmodas.github.io**

| Botão | Ação |
| --- | --- |
| Salvar contato | Abre `contato.vcf` — (14) 99105-1907, Instagram e logo. No iPhone mostra direto "Criar Novo Contato"; no Android baixa o arquivo e o toque em *Abrir* leva aos Contatos |
| Pix | Abre painel com a chave (14) 99105-1907 e botão "Copiar chave" |
| Instagram | https://www.instagram.com/zagmodass/ |
| Avalie no Google | https://share.google/eHjguiUz6idRV6Bau |

## Funciona sem internet

A página é um app instalável (`manifest.webmanifest`) com service worker
(`sw.js`) que guarda a página, o contato e as imagens no aparelho. Depois de
abrir uma vez com internet, a tela inicial, o painel do Pix e o "Salvar contato"
funcionam offline; Instagram e Google avisam que precisam de conexão.

Para instalar no celular:
- **Android (Chrome):** menu ⋮ → *Instalar app* (ou *Adicionar à tela inicial*).
- **iPhone (Safari):** botão Compartilhar → *Adicionar à Tela de Início*.

## Ao alterar algo

Troque a versão em `CACHE` no `sw.js` (ex.: `zagmodas-v2`) para os celulares
baixarem a versão nova. A página confere se há versão nova toda vez que abre com
internet e, quando há, recarrega sozinha uma vez para já mostrá-la.

## Publicação

GitHub Pages a partir do branch `main`, pasta `/ (root)`. O repositório precisa
ser **público** e se chamar `zagmodas.github.io` para o endereço ficar na raiz.
