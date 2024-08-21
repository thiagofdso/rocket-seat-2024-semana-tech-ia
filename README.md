# Projeto de Análise de Preços e Notícias de Ações

Este projeto utiliza agentes de inteligência artificial para analisar preços de ações e notícias de mercado, gerando um relatório detalhado e uma newsletter informativa.

## Requisitos

- Python 3.8 ou superior
- Pacotes listados em `requirements.txt`

## Instalação

1. Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    cd seu-repositorio
    ```

2. Crie um ambiente virtual e ative-o:
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
    ```

3. Instale os pacotes necessários:
    ```bash
    pip install -r requirements.txt
    ```

## Configuração

1. Crie um arquivo `secrets.toml` na pasta `.streamlit` com a chave da API do OpenAI:
    ```toml
    [secrets]
    OPEN_API_KEY = "sua-chave-api"
    ```

## Execução

1. Execute o aplicativo Streamlit:
    ```bash
    streamlit run app.py
    ```

2. No navegador, insira o símbolo da ação que deseja pesquisar e clique em "Run Research".

## Estrutura do Código

- **fetch_stock_price(ticket)**: Função para buscar o preço das ações usando a API do Yahoo Finance.
- **yahoo_finance_tool**: Ferramenta para buscar preços de ações.
- **stockPriceAnalyst**: Agente para análise de preços de ações.
- **getStockPrice**: Tarefa para analisar o histórico de preços de ações.
- **search_tool**: Ferramenta de busca de notícias usando DuckDuckGo.
- **newsAnalyst**: Agente para análise de notícias de mercado.
- **get_news**: Tarefa para obter notícias de mercado.
- **stockAnalystWrite**: Agente para escrever análises de ações.
- **writeAnalyses**: Tarefa para escrever a análise de ações.
- **crew**: Equipe de agentes para executar as tarefas.
- **Streamlit Interface**: Interface para entrada do usuário e exibição dos resultados.

## Funcionalidades

- **Análise de Preços de Ações**: Busca e analisa o histórico de preços de ações.
- **Análise de Notícias de Mercado**: Busca e resume notícias de mercado relacionadas às ações.
- **Geração de Newsletter**: Cria uma newsletter informativa baseada na análise de preços e notícias.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).