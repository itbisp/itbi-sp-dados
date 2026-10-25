# Preços reais de venda de imóveis em São Paulo (ITBI, 2006–2026)

Quanto vale um imóvel em São Paulo? Este repositório traz o **preço real do m²** de imóveis residenciais vendidos na cidade, por **distrito, rua e prédio, ano a ano desde 2006**, calculado a partir das guias de ITBI pagas na compra e publicadas pela Prefeitura de São Paulo.

São preços **declarados na compra**, não preços de anúncio. Para ver cada prédio, rua e bairro com mapa, histórico e estimativa de valor, use **[itbisp.com — Quanto vale meu imóvel?](https://itbisp.com/quanto-vale-meu-imovel)**.

## Arquivos

| Arquivo | O que tem | Linhas |
|---|---|---|
| [`dados/cidade_por_ano.csv`](dados/cidade_por_ano.csv) | Cidade inteira por ano: vendas, m² mediano, m² corrigido pelo IPCA, valor mediano | 21 |
| [`dados/m2_por_distrito_ano.csv`](dados/m2_por_distrito_ano.csv) | 96 distritos × ano (mínimo 10 vendas) | 1.994 |
| [`dados/m2_por_rua_ano.csv`](dados/m2_por_rua_ano.csv) | Rua × ano (mínimo 5 vendas) | 59.012 |
| [`dados/predios_resumo.csv`](dados/predios_resumo.csv) | Prédios com 5+ vendas desde 2006: total de vendas, primeira e última venda, m² mediano desde 2019 | 27.867 |

Cada linha tem uma coluna `pagina` com o link da página correspondente no itbisp.com (histórico, últimas vendas e estimativa de valor).

## Números da cidade

| Ano | Vendas residenciais | m² mediano | Valor mediano |
|---|---|---|---|
| 2024 | 77.582 | R$ 4.627 | R$ 460.000 |
| 2025 | 80.511 | R$ 4.852 | R$ 470.000 |
| 2026 (até 07/09) | 53.664 | R$ 5.000 | R$ 470.000 |

## Como foi calculado

- **Fonte:** "Guias de ITBI pagas", dados abertos da Secretaria Municipal da Fazenda de São Paulo, cruzados com o cadastro do IPTU e o GeoSampa.
- **Vendas consideradas:** compras e vendas de mercado de imóveis residenciais. Ficam de fora doações, heranças, permutas, transferências entre parentes e preços fora da faixa plausível.
- **Área:** área construída do cadastro do IPTU, que em apartamento inclui a fração das áreas comuns. Por isso o m² aqui fica abaixo do m² de anúncio, que usa a área privativa.
- **Mediana** sobre vendas individuais. **IPCA:** valores corrigidos até setembro de 2026.
- Metodologia completa: [itbisp.com/analise](https://itbisp.com/analise).

## Licença e citação

Dados sob [CC BY 4.0](LICENSE). Pode usar, inclusive comercialmente, citando a fonte:

> ITBI SP — Quanto vale meu imóvel? Preços reais de venda de imóveis em São Paulo a partir das guias de ITBI. https://itbisp.com

Este projeto não é afiliado à Prefeitura de São Paulo.

---

**English:** Real residential sale prices per m² in São Paulo, Brazil, by district, street and building, yearly since 2006, from the city's open ITBI (property transfer tax) records. Browse every building at [itbisp.com](https://itbisp.com). CC BY 4.0.
