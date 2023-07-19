# regress-o_3case-

Projeto de Regressão: Previsão de Preços de Imóveis nos EUA

Este é um projeto de regressão usando Python para prever os preços de imóveis nos Estados Unidos com base em um conjunto de características. Utilizamos técnicas de análise exploratória de dados, visualização e modelagem de regressão linear para criar um modelo preditivo.

Dados
Os dados utilizados neste projeto estão armazenados em um arquivo CSV chamado "USA_Housing.csv". O arquivo contém as seguintes colunas:

Avg. Area Income: Renda média da área em que o imóvel está localizado.
Avg. Area House Age: Idade média das casas na área.
Avg. Area Number of Rooms: Número médio de cômodos nas casas da área.
Avg. Area Number of Bedrooms: Número médio de quartos nas casas da área.
Area Population: População da área.
Price: Preço de venda do imóvel.
Address: Endereço do imóvel.
Pré-requisitos
Antes de executar o projeto, é necessário ter instalado o Python e algumas bibliotecas importantes. Para instalar as dependências, você pode usar o pip:

perl
Copy code
%pip install pandas seaborn numpy plotly cufflinks chart-studio
Análise Exploratória
Carregamos os dados do arquivo CSV usando a biblioteca pandas.
Renomeamos as colunas para eliminar espaços e tornar o nome mais amigável.
Removemos a coluna "Address", pois não é relevante para a modelagem.
Realizamos uma análise estatística descritiva dos dados.
Criamos gráficos de dispersão e boxplots para visualizar as relações entre as variáveis.
Modelo de Regressão Linear
Dividimos os dados em um conjunto de treinamento (70%) e um conjunto de teste (30%).
Utilizamos a biblioteca scikit-learn para criar um modelo de regressão linear.
Treinamos o modelo usando o conjunto de treinamento.
Avaliamos o desempenho do modelo usando o coeficiente de determinação (R²) com o conjunto de teste.
Previsão
Com base no modelo treinado, podemos fazer previsões de preços para novos imóveis. Por exemplo:

Suponha que temos os seguintes valores das características para um novo imóvel:
Avg_Area_Income = 50
Avg_Area_House_Age = 30
Avg_Area_Number_of_Rooms = 7
Avg_Area_Number_of_Bedrooms = 5
Area_Population = 200
Usando o modelo de regressão linear, prevemos o preço do imóvel:

python
Copy code
Avg_Area_Income = 50
Avg_Area_House_Age = 30
Avg_Area_Number_of_Rooms = 7
Avg_Area_Number_of_Bedrooms = 5
Area_Population = 200

entrada = [[Avg_Area_Income, Avg_Area_House_Age, Avg_Area_Number_of_Rooms, Avg_Area_Number_of_Bedrooms, Area_Population]]
preco_previsto = lm.predict(entrada)[0]
print(f"O preço previsto do imóvel é: ${preco_previsto:.2f}")
Contribuição
Contribuições são bem-vindas! Se você encontrou algum problema, tem sugestões para melhorar o projeto ou deseja adicionar novos recursos, fique à vontade para abrir uma issue ou enviar um pull request.

Licença
Este projeto está licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

Contato
Se você tiver alguma dúvida ou precisar de mais informações, você pode me contatar em:

Email: contato.guilhermebc@icloud.com
LinkedIn: https://www.linkedin.com/in/guilhermebcorreia/
