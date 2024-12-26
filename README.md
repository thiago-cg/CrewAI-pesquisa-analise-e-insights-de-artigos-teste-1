# Projeto de Pesquisa Científica Automatizada com CrewAI e LangChain

## Descrição

Este projeto demonstra como automatizar um processo de pesquisa científica utilizando a biblioteca CrewAI para orquestrar agentes inteligentes e a LangChain para interagir com modelos de linguagem. O objetivo é realizar buscas, filtrar e selecionar artigos científicos relevantes sobre um tema específico.

## Funcionamento

O código define quatro agentes, cada um com um papel específico na pesquisa:

1. **Agente de Geração de Palavras-chave (keywords_agent):**
    - Responsável por gerar palavras-chave relevantes para o tema da pesquisa.
    - Utiliza processamento de linguagem natural e análise semântica.
2. **Agente de Busca de Artigos (search_agent):**
    - Realiza buscas em bases de dados científicas utilizando as palavras-chave geradas.
    - Utiliza ferramentas como SerperDevTool e EXASearchTool.
3. **Agente de Filtragem de Artigos (filter_agent):**
    - Aplica filtros para selecionar os artigos mais relevantes.
    - Considera critérios como impacto, atualidade e metodologia.
4. **Agente de Seleção Final de Artigos (selection_agent):**
    - Realiza a curadoria final dos artigos, selecionando os mais importantes.
    - Analisa título, abstract e potencial de contribuição.

Esses agentes são organizados em uma equipe (Crew) que executa as seguintes tarefas:

1. **Geração de Palavras-chave:** Gera palavras-chave relevantes para o tema.
2. **Varredura de Bases de Dados:** Busca artigos em bases de dados científicas.
3. **Aplicação de Filtros:** Filtra os artigos com base em critérios de relevância.
4. **Curadoria Final de Artigos:** Seleciona os artigos mais importantes para a pesquisa.

## Utilização

1. **Instalação:**
    - Instale as bibliotecas necessárias: `pip install -q crewai crewai_tools langchain_community`
2. **Configuração:**
    - Configure as chaves de API para OpenAI, Serper e EXA.
3. **Execução:**
    - Defina o tema da pesquisa na variável `tema_pesquisa`.
    - Execute o código para iniciar o processo de pesquisa.
4. **Resultados:**
    - Os resultados da pesquisa serão exibidos no formato Markdown.

## Observações

- Este projeto é um exemplo de como automatizar a pesquisa científica.
- As ferramentas e os agentes podem ser personalizados para atender às necessidades específicas de cada pesquisa.
- É importante ter cuidado ao interpretar os resultados e realizar uma análise crítica dos artigos selecionados.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir um pull request ou issue no repositório do projeto.

## Autores

Thiago Correia Gonzaga
