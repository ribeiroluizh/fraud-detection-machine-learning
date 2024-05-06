# Detecção de Fraudes em Transações de E-commerce

## Sobre o Projeto

Este projeto faz parte do Módulo V do curso de Data Science da escola Ada Tech, em colaboração com o projeto Santander Coders. O objetivo é desenvolver um modelo de machine learning capaz de identificar transações fraudulentas em uma plataforma de e-commerce, utilizando um dataset sintético disponível no Kaggle. Este projeto aborda desde a análise exploratória dos dados até a modelagem preditiva, otimização de hiperparâmetros e validação dos modelos.

## Descrição do Dataset

O dataset "Fraudulent E-Commerce Transactions" é sintético, gerado utilizando a biblioteca Faker do Python, e simulando padrões realistas de transações e cenários fraudulentos. Contém 1.472.952 transações na versão 1 e 23.634 na versão 2, com aproximadamente 5% das transações classificadas como fraudulentas.

### Características do Dataset
- **Transaction ID**: Identificador único para cada transação.
- **Customer ID**: Identificador único para cada cliente.
- **Transaction Amount**: Valor total da transação.
- **Transaction Date**: Data e hora da transação.
- **Payment Method, Product Category, Quantity**: Detalhes do método de pagamento, categoria do produto e quantidade envolvida.
- **Customer Age, Location, Device Used, IP Address**: Informações demográficas e técnicas sobre o cliente.
- **Shipping Address, Billing Address**: Endereços de envio e de cobrança.
- **Is Fraudulent**: Indicador binário de fraude.
- **Account Age Days, Transaction Hour**: Idade da conta e hora da transação.

## Metodologia

### Análise Exploratória de Dados
Realizamos uma análise exploratória para entender as distribuições das variáveis, identificar outliers e verificar padrões e correlações nos dados.

### Pré-Processamento de Dados
Inclui limpeza de dados, tratamento de valores ausentes, codificação de variáveis categóricas e normalização.

### Modelagem e Avaliação
Utilizamos dois estimadores principais: Random Forest e AdaBoost. O desempenho dos modelos foi avaliado com base em métricas como precisão, recall e F1-score, com especial atenção ao recall de transações fraudulentas devido à natureza crítica das mesmas.

### Otimização de Hiperparâmetros
Aplicamos técnicas como Grid Search e Random Search para encontrar a melhor configuração de hiperparâmetros para os modelos.

## Resultados e Discussão

Os modelos mostraram um desempenho promissor, mas ainda insuficiente para um lançamento em produção, principalmente devido a baixa precisão e recall abaixo de 90% para transações fraudulentas. Isso indica a necessidade de coleta de mais dados e possivelmente explorar outras técnicas de modelagem ou balanceamento de dados.

## Conclusões

O projeto demonstrou a complexidade da detecção de fraudes em transações de e-commerce e destacou a importância de um modelo bem ajustado e de um dataset equilibrado. Recomendamos a continuação da pesquisa com uma coleta de dados mais abrangente e o teste de novos modelos e técnicas de balanceamento.

## Como Executar

1. Clone o repositório:
   ```
   git clone [URL do Repositório]
   ```
2. Instale as dependências:
   ```
   pip install -r requirements.txt
   ```
3. Execute o Jupyter Notebook:
   ```
   jupyter notebook
   ```

## Contato

Para dúvidas ou sugestões, por favor, entre em contato com algum dos membros do grupo:

- Laura
- Guilherme Araujo
- Guilherme Almeida
- Carlos Eduardo
- Luiz Henrique

Professor: Tiago Marto

---

Agradecemos a atenção e o interesse pelo nosso projeto!

```

Este README é completo e cobre todas as seções essenciais para descrever detalhadamente o projeto, incluindo contexto, metodologia, resultados, conclusões e instruções para execução, tornando-o uma excelente adição ao seu portfólio.