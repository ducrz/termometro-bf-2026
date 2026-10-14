# Termômetro Black Friday 2026 — dataset aberto

Linha de base de preços de uma amostra fixa de 300 produtos, congelada em 30/09/2026, antes da Black Friday 2026 (27/11/2026). O objetivo é medir, depois da Black Friday, quanto do desconto anunciado é real e quanto é preço maquiado.

Página oficial e metodologia completa: https://cupomdescontos.com/termometro-black-friday-2026

## O que é
- Amostra de produtos de programas de afiliados dos quais o CupomDescontos.com participa. **Não é o varejo todo.**
- 300 produtos, 1 loja (AliExpress), 4 categorias: Eletrônicos (97), Telefones e telecomunicações (96), Computador e escritório (61), Relógios (46).
- Linha de base: 31/08/2026 a 30/09/2026. Base congelada em 30/09/2026; a lista não muda depois.
- Coleta: uma foto de preço por dia (preço que a loja informa ao sistema). Última conferência feita em 14/10/2026: 238 de 300 produtos com preço reconfirmado no dia.

## Metodologia (resumo fiel à página)
Na Black Week (23 a 30/11/2026) compara-se o menor preço da semana com as médias dos 30 e 60 dias anteriores e classifica-se cada produto em desconto real, sem mudança relevante, mais caro ou preço maquiado, com limiares de 10%, 5% e 3% descritos na página. Dia sem reconfirmação de preço conta como "sem dado". A amostra foi escolhida por regra automática (até 100 produtos por categoria, mais vendidos segundo a loja, sem farmácia, sem preços "de/por" inconsistentes, apenas lojas que atualizam preço).

## Resultados
**Ainda não existem.** Só serão divulgados a partir de 28/11/2026 (parcial) e fechados após a Cyber Monday (30/11/2026). Este repositório não contém estimativas nem prévias.

## Arquivos
- `termometro-bf-baseline.csv` — as 300 linhas da linha de base (também em https://api.cupomdescontos.com/termometro-bf.csv)
- `amostra.csv` — as 20 primeiras linhas, para ver o formato
- `DICIONARIO-COLUNAS.md` — descrição das 14 colunas
- `CITATION.cff`, `LICENSE`

## Limites (leia antes de citar)
- Amostra concentrada em AliExpress e em 4 categorias; não generalizar para o comércio brasileiro.
- Marketplace: cada anúncio é de um vendedor; mede-se o comportamento dos anúncios, não uma política da plataforma.
- Preço informado ao afiliado pode diferir do preço no aplicativo (cupom, moedas, frete, impostos de importação não são medidos).
- Preço de produto importado é convertido para reais pela loja; parte da variação pode ser câmbio.
- Uma foto por dia: ofertas-relâmpago curtas podem não ser registradas.
- Limiares (10%, 5%, 3%) são escolha do autor; o CSV permite aplicar outro critério.

## Licença
CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). Uso livre, inclusive comercial, com crédito e link para a página do estudo.

## Como citar
Monteiro, Eduardo. *Termômetro Black Friday 2026*. CupomDescontos.com, 2026. https://cupomdescontos.com/termometro-black-friday-2026 (CC BY 4.0). Ver `CITATION.cff`.

## Aviso
O CupomDescontos.com (cupomdescontos.com) não é afiliado a sites de nome parecido ou com domínios semelhantes.
