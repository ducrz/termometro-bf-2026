# Dicionário de colunas — termometro-bf-baseline.csv

Arquivo UTF-8 com BOM, separador vírgula, quebra de linha CRLF, 14 colunas, 300 linhas de dados. Valores monetários em reais (R$), ponto decimal. Significados marcados com [CONFERIR] foram deduzidos do nome e precisam de confirmação do dono.

| Coluna | Tipo | Significado |
|---|---|---|
| item_id | inteiro | Identificador do produto no catálogo do CupomDescontos.com. |
| store_slug | texto | Loja (identificador curto). Neste lote: `aliexpress`. |
| category | texto | Categoria do produto: Eletrônicos; Telefones e telecomunicações; Computador e escritório; Relógios. |
| title | texto | Título do anúncio como informado pela loja. |
| baseline_start | data (AAAA-MM-DD) | Início do período de referência da linha de base (31/08/2026). |
| baseline_end | data (AAAA-MM-DD) | Fim do período de referência (30/09/2026). |
| baseline_price_min | decimal (R$) | Menor preço registrado no período de referência. |
| baseline_price_avg | decimal (R$) | Preço médio registrado no período de referência. |
| baseline_price_max | decimal (R$) | Maior preço registrado no período de referência. |
| baseline_points | inteiro | Quantidade de registros de preço do produto na janela de referência (histórico de preços dos 30 dias anteriores à seleção); a seleção exige no mínimo 20 registros. |
| price_at_freeze | decimal (R$) | Preço informado pela loja no momento do congelamento (30/09/2026). |
| price_from_at_freeze | decimal (R$) | Preço "de" informado pela loja no momento do congelamento (o preço anunciado antes do desconto). Atenção: é o que a loja informa, não prova de preço anterior real; por isso o estudo compara com o histórico próprio (`baseline_price_*`). |
| selection_rank | inteiro | Posição do produto na seleção dentro da categoria (1 = primeiro). A ordem vem do ranking de mais vendidos recentes devolvido pela própria loja (AliExpress), depois de remover títulos repetidos. |
| frozen_at | data-hora (AAAA-MM-DD HH:MM:SS, UTC) | Momento do congelamento da amostra, gravado pelo banco em UTC (30/09/2026 18:11:54 UTC = 15:11:54 em Brasília). |

Observação: o arquivo traz apenas a linha de base congelada. As fotos diárias e os resultados (classificação em desconto real, sem mudança, mais caro, preço maquiado) serão publicados a partir de 28/11/2026 na página do estudo.
