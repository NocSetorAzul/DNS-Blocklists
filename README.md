# Repositório de Listas de Bloqueio de Domínios (Blocklists)

> ⚠️ **IMPORTANTE:** Este repositório e as suas listas foram desenvolvidos **exclusivamente para o Unbound DNS**. Os links abaixo entregam os domínios prontos para integração direta nas diretivas do Unbound.

Repositório focado na centralização e organização de listas de bloqueio de domínios para aumento de produtividade, otimização de banda e segurança de redes administradas via Unbound DNS.

---

## 📂 Categorias e Links Diretos (Raw)

Para utilizar no seu servidor ou firewall, basta copiar o link da coluna **Link Raw (Unbound DNS)** correspondente à categoria que deseja bloquear.

| Categoria | Descrição / Escopo do Bloqueio | Link Raw (Unbound DNS) |
| :--- | :--- | :--- |
| 💬 **Comunicação** | Redes sociais, plataformas de chat, comunidades e fóruns. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Comunicacao/redes%20sociais.txt) |
| 🎮 **Games** | Plataformas de jogos virtuais, lojas digitais e consoles. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Games/Consoles.txt) |
| ✈️ **Lojas: Importados** | Marketplaces de compras internacionais e importações. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Lojas/compras%20internacionais.txt) |
| 📚 **Lojas: Cursos** | Plataformas de infoprodutos, cursos digitais e e-books. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Lojas/cursos.txt) |
| 🏠 **Lojas: Decoração** | Portais de móveis, decoração, ferramentas e construção. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Lojas/decoracao.txt) |
| 💻 **Lojas: Eletrónicos** | E-commerces de informática, hardware, tecnologia e eletrodomésticos. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Lojas/eletronicos.txt) |
| 🛒 **Lojas: Marketplaces** | Grandes e-commerces e portais de varejo generalistas. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Lojas/marketplaces.txt) |
| 👗 **Lojas: Moda** | Lojas de vestuário, vestes, calçados e acessórios de moda. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Lojas/moda.txt) |
| 🍎 **Mercado** | Redes de supermercados e plataformas de varejo alimentar. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Mercado/mercado.txt) |
| 📰 **Notícias** | Portais de notícias informativas e cobertura desportiva. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Noticias/esportes.txt) |
| 🎬 **Streaming: Legal** | Serviços oficiais de streaming de vídeo, áudio e entretenimento. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Streaming/legal.txt) |
| ☠️ **Streaming: Pirata** | Plataformas de streaming ilegal, IPTV pirata e domínios de risco associados. | [Link](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Streaming/pirata.txt) |

> 📌 **Dica sobre Espaços em Branco:** Para os ficheiros que contêm espaços no nome (como `redes sociais.txt`), os links acima já utilizam o padrão `%20` exigido pelo GitHub para evitar quebras de URL.

---

## 🛠️ Como Utilizar no Unbound DNS

Pode injetar as listas diretamente nas configurações do seu Unbound (`unbound.conf`) utilizando as diretivas de controle de zonas locais ou RPZ (conforme a compilação do seu ambiente).

### Exemplo Prático com Zonas Locais (Local-Zone):

[https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Streaming/pirata.txt](https://raw.githubusercontent.com/NocSetorAzul/DNS-Blocklists/refs/heads/main/Streaming/pirata.txt)

## 🤝 Como Contribuir

Identificou um domínio que mudou ou quer adicionar novos sites à lista?
1. Faça um **Fork** deste repositório.
2. Adicione os domínios desejados ao arquivo correto (um domínio por linha, sem o protocolo `http://` ou `https://`).
3. Envie um **Pull Request** detalhando as adições.
