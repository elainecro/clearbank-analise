# ClearBank — Análise Financeira com Python

Desafio final do módulo de Análise de Dados com IA (Pós Rocketseat).
Notebook que lê um arquivo de transações financeiras (`transacoes.csv`), valida e limpa
os dados, calcula métricas mensais, identifica transações suspeitas (acima de R$ 10.000,00)
e exporta o resultado em JSON.

## Como executar

1. Abra `desafio-final.ipynb` no Google Colab ou Jupyter (Python 3.10+).
2. Execute todas as células em ordem (`Runtime → Run all` no Colab).
3. O próprio notebook gera o arquivo de dados `transacoes.csv` através da função
   `gerar_csv_transacoes()` — a quantidade de linhas é configurável pela variável
   `QTD_LINHAS_CSV` (mínimo 30).

Dependências opcionais (apenas para as células extras): `pip install pandas matplotlib`.

## Saídas geradas

- **Terminal (saída das células):** resumo da limpeza dos dados, período analisado,
  relatório mensal (créditos, débitos, saldo, média, maior/menor valor) e lista de
  transações suspeitas.
- **`relatorio.json`:** relatório completo da análise em JSON.
- **`grafico.png`:** gráfico de barras com o saldo mensal (requisito opcional).
- **`analise_pandas.py`:** versão alternativa da análise com pandas (requisito opcional).

## Estrutura do repositório

- `desafio-final.ipynb` — notebook principal com todas as saídas salvas
- `analise_pandas.py` — análise alternativa com pandas (opcional)
- `grafico.png` — gráfico do saldo mensal (opcional)
- `README.md` — este arquivo
