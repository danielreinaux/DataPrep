# Projeto Titanic - Preparação de Dados (DataPrep)

## Descrição do Projeto
Neste projeto, nosso foco será exclusivamente a preparação dos dados (DataPrep) para garantir que estejam prontos para análise e modelagem. Não realizaremos análises descritivas nem estatísticas nesta etapa. Além disso, como nosso conjunto de dados já está separado em conjuntos de treino e teste, abordaremos apenas a preparação dos dados no nosso dataset de treino, que já está separado. Todo o processo de DataPrep será realizado diretamente neste conjunto de dados de treino.

## Estrutura do Projeto
1.Análise dos Metadados
2. Tratamento de Valores Nulos
3. Análise de Cardinalidade
4. Codificação One-Hot/Label
5. Normalização

## Etapas da Preparação dos Dados
### 1. Análise Inicial
![image](https://github.com/danielreinaux/DataPrep/assets/91274263/4be9e2ae-9c39-49c9-80f7-b37e0c9c7939)

#### 1.1 Ajustes nas Colunas:
Antes de iniciar qualquer etapa de preparação dos dados, é essencial retirar a coluna alvo (Target). Além disso, identificamos colunas que não são necessárias para o nosso modelo e que podem introduzir ruído ou redundância (no nosso caso, 'PassengerID' e 'Ticket'.
![image](https://github.com/danielreinaux/DataPrep/assets/91274263/5b12466c-6e53-4284-a1d6-98540bf44d74)

Ademais, criamos uma coluna vindo da classe 'Name', onde tratamos ela e retiramos uma informação mais valiosa, o seu título (Mr, Mrs, Miss, Dr)
![image](https://github.com/danielreinaux/DataPrep/assets/91274263/1d36fdc1-cd2f-4d6f-878e-a75ffc84cfb4)


### 2. Análise dos Metadados
Examinamos os metadados do conjunto de dados para entender a estrutura, tipos de dados e identificar possíveis desafios na preparação dos dados.
![image](https://github.com/danielreinaux/DataPrep/assets/91274263/f0ac9bbf-d8df-4c33-a6f2-dd77a1da2b26)

### 3. Tratamento de Valores Nulos
Tratamos os valores nulos de acordo com a natureza das variáveis:
- Variáveis Numéricas: Preenchemos os valores nulos com a média.
- Variáveis Categóricas: Preenchemos os valores nulos com a moda (o valor que mais aparece).
![image](https://github.com/danielreinaux/DataPrep/assets/91274263/0db25afe-5fe4-4911-81a4-85032880925d)

### 4. Codificação One-Hot/Label:
Implementamos técnicas de codificação para transformar variáveis categóricas em um formato que possa ser utilizado pelos algoritimos de Machine Learning:
![image](https://github.com/danielreinaux/DataPrep/assets/91274263/6e2be327-bb9d-46bc-9f78-dd3db4e93283)

* No nosso caso, nenhuma coluna ocorreu o uso do LabelEncoder, devido a baixa cardinalidade delas

### 5. Normalização:
Optamos pela normalização dos dados numéricos para garantir que todas as variáveis contribuam de maneira equilibrada para a análise.
![image](https://github.com/danielreinaux/DataPrep/assets/91274263/e63d144e-dd96-4cda-8945-d7bd710377c8)



