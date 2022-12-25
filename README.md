# O laboratório LAB_SAÚDE deseja informatizar o atendimento a seus clientes. O diretor de tecnologia passou as seguintes especificações para a construção de um sistema:

## 1. Será necessário efetuar um cadastro dos pacientes onde devem ser informados:
- Cadastro de Pessoa Física (CPF)
- Nome completo
- Endereço
- Telefone
- Idade
- *Os dados devem ser armazenados em arquivo.*

## 2. Na entrada do laboratório há um funcionário que consulta o CPF do paciente. Caso o mesmo esteja cadastrado, é encaminhado para a fila de atendimento. Caso contrário, é feito o cadastramento de acordo com os dados acima e só depois é encaminhado para a fila de atendimento.

## 3. O paciente entra na fila de atendimento inicial obedecendo a prioridade de idade e tempo de espera na fila. A fila deve ser implementada usando a estrutura de dados fila contendo CPF do paciente, idade e tempo de espera, que deve ser iniciado com zero.

## 4. No atendimento inicial o atendente chama o próximo da fila e informa o número da sua mesa.Sempre deve ser chamado o paciente com maior prioridade.Deve ser definido um critério para que as pessoas mais novas possam ser atendidas mesmo havendo pessoas mais velhas a serem atendidas, por causa do tempo de permanência na fila. A cada nova chamada de um paciente, os demais devem ter seu tempo de permanência acrescido deuma unidade e deve ser reorganizada a fila de prioridades de acordo com os critérios definidos por vocês, devendo a fila estar ordenada por prioridade.
- *sugestão para essa opção:*
- façam a leitura de todos os pacientes na fila e coloquem seus dados em memória (vetores),
acrescentando uma unidade no tempo de espera e recalculando a prioridade
- ordenem esses vetores por prioridade, mantendo a correspondência entre os dados e a prioridade
- esvaziem a fila, liberando todos os elementos da memória
- insiram os elementos com base na ordem dos dados do vetor

## 5. No atendimento o atendente preenche a quantidade de exames a efetuar, se é convênio ou particular e a data de entrega dos exames.

## 6. Na conclusão do atendimento o paciente é retirado da fila de atendimento e deve ser incluído nafila de espera para coleta, sendo armazenados o CPF do paciente, idade, tempo de espera (aqui também iniciado com zero), quantidade de exames, se é convênio ou particular e a hora do atendimento. A prioridade será determinada pela idade, o tempo de espera e a quantidade de exames. Como só haverá uma enfermeira para coleta do material, a quantidade de exames deve ser um critério de desempate. Para definir a prioridade deve-se usar o mesmo critério do atendimento inicial.

## 7.A enfermeira sempre chamará o primeiro da fila. Na chamada para coleta devem ser armazenados, em arquivo, o CPF do paciente, a data do atendimento, a hora do atendimento, a hora da coleta e a quantidade de exames. O paciente deve ser retirado da fila de coleta e a mesma deve ser reordenada, como especificado acima.

## 8. O diretor de tecnologia sugere a seguinte apresentação do sistema:
### 1. Cadastrar paciente
### 2. Atendimento inicial
### 3. Chamar para atendimento
### 4. Chamar para coleta
### 5. Mostrar fila para atendimento
### 6. Mostrar fila para coleta
### 7. Mostrar atendimento do dia.
