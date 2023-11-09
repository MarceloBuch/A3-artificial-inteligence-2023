## A3 – Previsão de Risco de Ataque Cardíaco

### Ideia Principal da Escolha do Dataset

O conjunto de dados de previsão de risco de ataque cardíaco serve como um recurso valioso para aprofundar a intrincada dinâmica da saúde cardíaca e seus preditores. Os ataques cardíacos, ou enfartes do miocárdio, continuam a ser um problema de saúde global significativo, necessitando de uma compreensão mais profunda de seus precursores e potenciais fatores atenuantes. Este conjunto de dados engloba uma ampla gama de atributos, incluindo idade, níveis de colesterol, pressão arterial, hábitos de fumar, padrões de exercício, preferências alimentares e muito mais, com o objetivo de elucidar a complexa interação dessas variáveis na determinação da probabilidade de um ataque cardíaco. Ao empregar análises preditivas e aprendizado de máquina neste conjunto de dados, podemos trabalhar em estratégias proativas para prevenção e gerenciamento de doenças cardíacas. O conjunto de dados é um testemunho dos esforços coletivos para melhorar a nossa compreensão da saúde cardiovascular e preparar o caminho para um futuro mais saudável.

Link do dataset: [Heart Attack Prediction Dataset](https://www.kaggle.com/datasets/iamsouravbanerjee/heart-attack-prediction-dataset)

### Dados Detalhados

- ID do paciente - identificador exclusivo de cada paciente (String)
- Idade - Idade do paciente (int)
- Sexo - Gênero do paciente (0: Feminino, 1: Masculino)
- Colesterol - Níveis de colesterol do paciente (int)
- Pressão Arterial - Pressão arterial do paciente (sistólica/diastólica)
- Frequência cardíaca - frequência cardíaca do paciente (int)
- Diabetes - Se o paciente tem diabetes (1: Sim, 0: Não)
- História Familiar - História familiar de problemas cardíacos (1: Sim, 0: Não)
- Tabagismo - Tabagismo do paciente (1: Fumante, 0: Não fumante)
- Obesidade - Status de obesidade do paciente (1: Obeso, 0: Não obeso)
- Consumo de álcool - Nível de consumo de álcool pelo paciente (1: Sim, 0: Não)
- Horas de exercício por semana - número de horas de exercício por semana (decimal)
- Dieta - Hábitos alimentares do paciente (Saudável/Médio/Não saudável)
- Problemas cardíacos anteriores - Problemas cardíacos anteriores do paciente (1: Sim, 0: Não)
- Uso de Medicamentos - Uso de medicamentos pelo paciente (1: Sim, 0: Não)
- Nível de Estresse - Nível de estresse relatado pelo paciente (int)
- Horas sedentárias por dia - Horas de atividade sedentária por dia
- Renda - nível de renda do paciente (int)
- IMC - Índice de Massa Corporal (IMC) do paciente (decimal)
- Triglicerídeos - Níveis de triglicerídeos do paciente (int)
- Dias de atividade física por semana - Dias de atividade física por semana (int)
- Horas de sono por dia - Horas de sono por dia (int)
- País - País do paciente (String)
- Risco de ataque cardíaco - Presença de risco de ataque cardíaco (1: Sim, 0: Não)

### Transformação dos Dados e Definição da Variável Target

Observando nosso dataset, percebemos que era necessário alterar a coluna de 'Sexo', que estava como 'Masculino/Feminino' para '0/1'. Outra mudança que optamos por fazer foi de excluir as colunas 'Continente' e 'Hemisfério', elas geram muita redudância para o que queremos realizar no projeto. O conjunto de dados culmina em um recurso de classificação binária crucial que denota a presença ou ausência de risco de ataque cardíaco, fornecendo um recurso abrangente para análise preditiva e pesquisa em saúde cardiovascular. Por isso, decidimos que a variável alvo para o desenvolvimento do projeto será a coluna "Risco de Ataque Cardíaco" (Heart Attack Risk).
