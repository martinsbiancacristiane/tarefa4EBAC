arefa M4 - Análise de PVL (Dados Simulados)
Este projeto contém a solução para a Tarefa do Módulo 4, focada na manipulação de dados com a biblioteca Pandas e na estruturação de código com funções Python, simulando a interação com a API do Tesouro Nacional (SICONFI).

💡 Sobre o Projeto
A tarefa consiste em dois blocos principais:

Manipulação Básica de Dados: Filtragem, contagem de frequências e extração de informações temporais a partir de dados de Pedidos de Verificação de Limites (PVL) de Municípios do Rio de Janeiro.

Modularização e Filtros: Criação de uma função para encapsular o processo de carregamento de dados e aplicação de filtros complexos (ex: contar status específicos em MG, encontrar o município da BA com mais deferimentos).

⚠️ Solução Adotada (Mock/Simulação)
Devido à instabilidade e erros de conexão (como o URLError) da API real do SICONFI, todas as soluções foram implementadas usando DataFrames Simulados (Mock Data). Isso garante que a lógica de programação em Pandas e a estrutura da função sejam validadas sem falhas de conexão externa.

🛠️ Tecnologias Utilizadas
Python 3.x

Pandas: Biblioteca essencial para manipulação e análise de dados.

Jupyter Notebook/Lab: Ambiente ideal para execução célula a célula.

⚙️ Como Rodar a Solução
Baixe o arquivo Profissão Cientista de Dados M4 - Tarefa aulas 06 a 08.ipynb.

Certifique-se de ter as bibliotecas pandas instaladas no seu ambiente Python.

Execute as células do notebook sequencialmente.

A solução é apresentada em ordem, com o código de cada item isolado para demonstrar os passos e o resultado (print) de cada análise.

📋 Resumo dos Exercícios Resolvidos
Bloco	Item	Descrição da Análise	Ferramenta Principal
1	1.1	Carregar e filtrar dados de Municípios do RJ.	df[máscara]
1	1.2/1.4	Contar frequências de status e ano_status.	value_counts()
1	1.3	Criar a coluna ano_status.	.str.slice()
2	2.1	Definir a função modular de carregamento (carregar_pvl).	def function()
2	2.2	Contar solicitações de MG com status 'Arquivado por decurso de prazo'.	len(df[máscara])
2	2.3	Encontrar o Município da BA com mais solicitações 'Deferidas'.	value_counts().index[0]
2	2.4	Salvar dados do Estado da BA em um arquivo CSV.	df.to_csv()
