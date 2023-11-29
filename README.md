## A3 – Previsão de Risco de Ataque Cardíaco

### Ideia Principal da Escolha do Dataset

O conjunto de dados de previsão de risco de ataque cardíaco serve como um recurso valioso para aprofundar a intrincada dinâmica da saúde cardíaca e seus preditores. Os ataques cardíacos, ou enfartes do miocárdio, continuam a ser um problema de saúde global significativo, necessitando de uma compreensão mais profunda de seus precursores e potenciais fatores atenuantes. Este conjunto de dados engloba uma ampla gama de atributos, incluindo idade, níveis de colesterol, pressão arterial, hábitos de fumar, padrões de exercício, preferências alimentares e muito mais, com o objetivo de elucidar a complexa interação dessas variáveis na determinação da probabilidade de um ataque cardíaco. Ao empregar análises preditivas e aprendizado de máquina neste conjunto de dados, podemos trabalhar em estratégias proativas para prevenção e gerenciamento de doenças cardíacas. O conjunto de dados é um testemunho dos esforços coletivos para melhorar a nossa compreensão da saúde cardiovascular e preparar o caminho para um futuro mais saudável.

Link do dataset: [Heart Attack Prediction Dataset](https://www.kaggle.com/datasets/iamsouravbanerjee/heart-attack-prediction-dataset)

### Dados Detalhados

- Patient ID (ID do paciente) - identificador exclusivo de cada paciente (String)
- Age (Idade) - Idade do paciente (int) 
- Sex (Sexo) - Gênero do paciente (0: Masculino, 1: Feminino)
- Cholesterol (Colesterol) - Níveis de colesterol do paciente (int) 
- Blood Pressure (Pressão Arterial) - Pressão arterial do paciente (sistólica/diastólica) 
- Heart Rate (Frequência cardíaca) - frequência cardíaca do paciente (int)
- Diabetes - Se o paciente tem diabetes (1: Sim, 0: Não)
- Family History (História Familiar) - História familiar de problemas cardíacos (1: Sim, 0: Não) 
- Smoking (Tabagismo) - Tabagismo do paciente (1: Fumante, 0: Não fumante) 
- Obesity (Obesidade) - Status de obesidade do paciente (1: Obeso, 0: Não obeso) 
- Alcohol Consumption (Consumo de álcool) - Nível de consumo de álcool pelo paciente (1: Sim, 0: Não) 
- Exercise Hours Per Week (Horas de exercício por semana) - número de horas de exercício por semana (decimal) 
- Diet (Dieta) - Hábitos alimentares do paciente (Não saudável: 0, Médio: 1, Saudável: 2) 
- Previous Heart Problems (Problemas cardíacos anteriores) - Problemas cardíacos anteriores do paciente (1: Sim, 0: Não)
- Medication Use (Uso de Medicamentos) - Uso de medicamentos pelo paciente (1: Sim, 0: Não)
- Stress Level (Nível de Estresse) - Nível de estresse relatado pelo paciente (int)
- Sedentary Hours Per Day (Horas sedentárias por dia) - Horas de atividade sedentária por dia
- Income (Renda) - nível de renda do paciente (int)
- BMI (IMC) - Índice de Massa Corporal (IMC) do paciente (decimal)
- Triglycerides (Triglicerídeos) - Níveis de triglicerídeos do paciente (int)
- Physical Activity Days Per Week (Dias de atividade física por semana) - Dias de atividade física por semana (int) 
- Sleep Hours Per Day (Horas de sono por dia) - Horas de sono por dia (int) 
- Country (País) - País do paciente (String)
- Continent (Continente) - Continente do paciente (String)
- Hemisphere (Hemisfério) - Hemisfério do paciente (String)
- Heart Attack Risk (Risco de ataque cardíaco) - Presença de risco de ataque cardíaco (1: Sim, 0: Não)

### Transformação dos Dados e Definição da Variável Target

Observando nosso dataset, percebemos que era necessário alterar a coluna de 'Sexo', que estava como 'Masculino/Feminino' para '0/1', alteremos também a coluna 'Dieta' que estava como 'Saudável/Médio/Não saudável' para '0/1/2'. Criamos duas colunas para separar a coluna 'Pressão Arterial', separando ela em 'systolic' e 'diastolic'. Outra mudança que optamos por excluir as colunas : 'Patient ID', 'Sex', 'Heart Rate', 'Previous Heart Problems','Medication Use','Stress Level', 'Sedentary Hours Per Day', 'Blood Pressure', 'Country', 'Continent', 'Hemisphere','Income', 'BMI', 'Triglycerides'. Elas foram removidas no tratamento dos dados pois dentro da analise da nossa base, percebemos que muitas delas geram redudância, ou em alguns casos uma certa parcialidade para o algoritmo, podendo gerar erros nas predições.  
O conjunto de dados culmina em um recurso de classificação binária crucial que denota a presença ou ausência de risco de ataque cardíaco, fornecendo um recurso abrangente para análise preditiva e pesquisa em saúde cardiovascular. Por isso, decidimos que a variável alvo para o desenvolvimento do projeto será a coluna "Risco de Ataque Cardíaco" (Heart Attack Risk).
