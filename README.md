# Repositório de Listas de Bloqueio de Domínios (Blocklists)

Este repositório contém listas de bloqueio de domínios organizadas por categorias específicas para otimizar o gerenciamento de tráfego, produtividade e segurança de rede. As listas estão estruturadas no formato de texto puro (planilha de domínios ou hosts), sendo ideais para integração com ferramentas de filtragem DNS como **Pi-hole**, **AdGuard Home**, **pfBlockerNG (pfSense)**, **OPNsense**, ou firewalls corporativos.

## 📂 Organização e Categorias

As listas estão divididas nos seguintes grupos estruturados:

| Identificador do Grupo | Descrição / Escopo do Bloqueio |
| :--- | :--- |
| `GRP_COMPRAS_MARKETPLACES_VAREJO_GERAL` | Grandes e-commerces, marketplaces e lojas de varejo generalista. |
| `GRP_COMPRAS_MODA_ACESSORIOS` | Lojas de vestuário, moda, roupas, calçados e acessórios em geral. |
| `GRP_COMPRAS_ELETRONICOS_TECNOLOGIA` | Portais de venda de eletrônicos, componentes de informática e tecnologia. |
| `GRP_COMPRAS_GAMES_CONSOLES` | Plataformas, lojas de jogos virtuais, consoles e e-commerces de games. |
| `GRP_COMPRAS_CASA_MOVEIS_DECORACAO` | Lojas de móveis, itens de decoração, materiais de construção e ferramentas. |
| `GRP_COMPRAS_SUPERMERCADO_VAREJO_ALIMENTAR`| Redes de supermercados e plataformas de e-commerce de alimentos. |
| `GRP_COMPRAS_IMPORTADOS_INTERNACIONAIS` | Sites e marketplaces focados em compras e importações internacionais. |
| `GRP_COMPRAS_CURSOS_DIGITAIS_INFOPRODUTOS`| Plataformas de cursos online, livrarias, infoprodutos e bens digitais. |
| `GRP_COMPRAS_COSMETICOS_PERFUMARIA` | E-commerces de cosméticos, produtos de beleza, maquiagem e perfumaria. |
| `GRP_COMUNICACAO_REDES_SOCIAIS` | Redes sociais, plataformas de comunicação, comunidades e fóruns, e streaming de música de uso social. |
| `GRP_NOTICIAS_PORTAIS_ESPORTES` | Portais informativos, sites de notícias gerais e cobertura esportiva. |
| `GRP_STREAMING_VIDEO_AUDIO` | Serviços de streaming legítimos de vídeo, áudio, TV por internet e entretenimento. |
| `GRP_PIRATARIA_STREAMING_ILEGAL` | Portais de distribuição pirata, plataformas de streaming ilegal (IPTV não oficial) e domínios de alto risco associados. |

---

## 🛠️ Como Utilizar

Cada grupo acima corresponde a um arquivo `.txt` na raiz ou na pasta correspondente deste repositório (ex: `GRP_COMPRAS_MARKETPLACES_VAREJO_GERAL.txt`).

### Exemplos de Integração:

#### 1. Pi-hole / AdGuard Home
Basta copiar a URL do arquivo no modo **Raw** do GitHub e adicioná-la nas configurações de *Adlists* (Pi-hole) ou *Filtros DNS* (AdGuard Home).

#### 2. pfBlockerNG / OPNsense
Configure um novo alias do tipo **DNSBL** apontando para a URL Raw do grupo desejado para automatizar o download e o bloqueio periódico de toda a categoria.

---

## 🤝 Como Contribuir

Identificou um domínio que mudou ou quer adicionar novos sites à lista?
1. Faça um **Fork** deste repositório.
2. Adicione os domínios desejados ao arquivo correto (um domínio por linha, sem o protocolo `http://` ou `https://`).
3. Envie um **Pull Request** detalhando as adições.
