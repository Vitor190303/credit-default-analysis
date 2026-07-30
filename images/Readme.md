# Análise de Inadimplência em Clientes de Cartão de Crédito

Projeto de análise exploratória de dados desenvolvido para investigar características e comportamentos financeiros associados à inadimplência de clientes de cartão de crédito.

O trabalho apresenta todo o processo de leitura, exploração, limpeza, transformação, visualização e interpretação dos dados utilizando Python.

## Objetivo

Responder à seguinte pergunta:

> Quais características e comportamentos financeiros estão mais associados à inadimplência dos clientes?

A variável `default` representa a situação do cliente:

- `0`: cliente adimplente;
- `1`: cliente inadimplente.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Git e GitHub

## Etapas do projeto

1. Leitura e exploração inicial dos dados;
2. análise da variável de inadimplência;
3. identificação de dados ausentes;
4. transformação das colunas monetárias;
5. tratamento e limpeza da base;
6. análise exploratória;
7. criação de visualizações;
8. interpretação dos resultados;
9. elaboração de conclusões e recomendações.

## Visão geral dos dados

A base original continha 10.127 registros de clientes.

Após a remoção dos registros com dados ausentes, a análise principal foi realizada com 7.081 clientes.

## Principais resultados

A análise sugere que a inadimplência está mais associada ao comportamento de utilização do cartão do que às características demográficas isoladas.

Os clientes inadimplentes apresentaram, em geral:

- menor quantidade de transações;
- menor valor total movimentado;
- maior período de inatividade;
- menor quantidade de produtos contratados;
- maior quantidade de interações com a instituição.

Esses indicadores podem auxiliar na identificação antecipada de clientes com maior risco de inadimplência.

## Visualizações

### Distribuição dos clientes

![Distribuição dos clientes](images/01_distribuicao_clientes.png)

### Dados ausentes

![Dados ausentes](images/02_dados_ausentes.png)

### Quantidade de transações

![Quantidade de transações](images/03_quantidade_transacoes.png)

### Valor das transações

![Valor das transações](images/04_valor_transacoes.png)

### Inadimplência por quantidade de produtos

![Inadimplência por quantidade de produtos](images/05_taxa_por_produtos.png)

### Inadimplência por quantidade de interações

![Inadimplência por quantidade de interações](images/06_taxa_por_interacoes.png)

### Inadimplência por período de inatividade

![Inadimplência por inatividade](images/07_taxa_por_inatividade.png)

### Inadimplência por sexo

![Inadimplência por sexo](images/08_taxa_por_sexo.png)

### Inadimplência por escolaridade

![Inadimplência por escolaridade](images/09_taxa_por_escolaridade.png)

### Inadimplência por faixa salarial

![Inadimplência por salário](images/10_taxa_por_salario.png)

### Matriz de correlação

![Matriz de correlação](images/11_matriz_correlacao.png)

## Conclusões

Os resultados indicam que sinais de redução no relacionamento financeiro podem funcionar como alertas de risco.

Uma instituição financeira poderia acompanhar clientes que apresentem:

- redução brusca na quantidade de transações;
- diminuição do valor total movimentado;
- aumento do período de inatividade;
- aumento da quantidade de interações;
- baixa utilização dos produtos disponíveis.

Possíveis ações incluem campanhas de reativação, contato preventivo, renegociação e análise dos motivos das interações mais frequentes.

## Limitações

- A análise identifica associações, mas não comprova causalidade;
- registros com valores ausentes foram removidos;
- o conjunto de dados não informa o motivo das interações;
- não foi desenvolvido um modelo de aprendizado de máquina;
- o projeto possui finalidade educacional e exploratória.

## Estrutura do projeto

```text
projeto-inadimplencia/
├── images/
├── projeto_inadimplencia.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## Como executar

Clone o repositório:

```bash
git clone LINK_DO_SEU_REPOSITORIO
```

Entre na pasta:

```bash
cd projeto-inadimplencia
```

Crie um ambiente virtual:

```bash
python -m venv .venv
```

Ative o ambiente no Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

Coloque o arquivo de dados original na pasta principal com o nome:

```text
Python_M11_support material.csv
```

Abra o notebook:

```bash
jupyter notebook projeto_inadimplencia.ipynb
```

## Notebook

[Acessar o notebook completo](projeto_inadimplencia.ipynb)

## Autor

**Vitor Campos**

Estudante de Ciência de Dados com foco em Python, análise exploratória, visualização de dados e geração de insights para negócios.