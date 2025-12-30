# Alertas
O relatório Alertas apresenta todos os parâmetros legais que não foram cumpridos no período selecionado, identificando de forma detalhada os colaboradores em incumprimento e a natureza exata de cada violação legal.
Para cada ocorrência, o relatório indica:
•	o colaborador a que o incumprimento diz respeito;
•	o parâmetro legal que não foi respeitado;
•	o valor legal definido para esse parâmetro;
•	o valor efetivamente aplicado;
•	o valor de incumprimento, ou seja, em quantas unidades o valor aplicado excedeu o limite legal.
Adicionalmente, o relatório disponibiliza informação de auditoria relativa à última alteração efetuada, incluindo:
•	o utilizador que realizou a alteração;
•	a data em que essa alteração ocorreu;
•	e a indicação de troca, sempre que tenha existido alguma intervenção desse tipo.
No cabeçalho, o relatório apresenta claramente a loja/unidade e o período de análise selecionados pelo utilizador.
Os resultados encontram-se organizados por secção, sendo que a primeira entrada da tabela corresponde à secção escolhida no momento da extração.
A tabela do relatório é composta por 11 colunas:
1.	Número Mecanográfico – número identificativo do colaborador
2.	Colaborador – nome do colaborador
3.	Parâmetro Legal – parâmetro legal avaliado
4.	Valor Legal – limite legal definido
5.	Data Início – data de início do incumprimento
6.	Data Fim – data de fim do incumprimento
7.	Valor Aplicado – valor efetivamente registado
8.	Valor de Incumprimento – diferença entre o valor aplicado e o valor legal
9.	Utilizador – utilizador responsável pela última alteração
10.	Data – data da última alteração
11.	Troca – indicação de troca, caso exista
 
## Configurações do relatório
•	i_fk_unit → unidades (multi-seleção)
•	i_fk_section → secções (multi-seleção)
•	i_fk_employee → colaboradores (multi-seleção)
•	i_legal_params → parâmetros legais (drop-down / configuração)
•	i_start_date / i_end_date → período
## Filtros do relatório:
•	Unidades: multi-seleção (OBRIGATÓRIO)
•	Secções: multi-seleção
•	Colaboradores: multi-seleção
•	Parametros legais: drop-down
•	Período
•	Ordenação: radio button
 
## Informação técnica
•	Nome do relatório: Alertas
•	Função: S_PCK_CORE_REPORTS.GET_ALERTS
•	Local de impressão: Módulo “relatórios”
•	Formatos disponíveis: Excel, PDF
# Algoritmo de Descansos -Horas anuais

# Alterações à Escala
O relatório Alterações à Escala apresenta todas as alterações efetuadas às escalas de trabalho dos colaboradores no período selecionado, permitindo acompanhar de forma detalhada o histórico de mudanças de horário e carga horária.
Para cada alteração registada, o relatório identifica:
•	o colaborador afetado;
•	a data em que ocorreu a alteração da escala;
•	o horário e carga anteriores à alteração;
•	o horário e carga atuais, após a alteração;
•	o motivo da alteração, conforme selecionado no momento da execução;
•	os utilizadores responsáveis pela criação e pela alteração da escala;
•	as datas de criação e de alteração;
•	o número da troca, quando aplicável;
•	e o estado da troca, permitindo perceber em que fase do processo se encontra.
No cabeçalho, o relatório apresenta a unidade, o período e a secção selecionados, bem como o total de alterações encontradas para os critérios definidos.
Os resultados são organizados por secção, apresentando de forma cronológica todas as alterações realizadas aos horários dos colaboradores.
A tabela do relatório é composta por 12 colunas:
1.	Matrícula – número identificativo do colaborador
2.	Nome do Colaborador – nome completo do colaborador
3.	Data – dia em que a escala foi alterada
4.	Anterior – Horário / Carga – horário e respetiva carga antes da alteração
5.	Atual – Horário / Carga – horário e respetiva carga após a alteração
6.	Motivo da Alteração – motivo selecionado para a alteração da escala
7.	Utilizador de Criação – utilizador que criou a alteração
8.	Data de Criação – data em que a alteração foi criada
9.	Utilizador de Alteração – utilizador que efetuou a última alteração
10.	Data de Alteração – data da última alteração registada
11.	Nº Troca – número identificativo da troca
12.	Estado da Troca – estado atual da troca
 
Configurações do relatório
•	i_fk_unit → unidades (multi-seleção)
•	i_fk_section → secções (multi-seleção)
•	i_fk_employee → colaboradores (multi-seleção)
•	i_begin_date / i_end_date → período
•	i_status → estado(s) da troca (multi-seleção)
•	i_show_history → mostrar histórico de alterações (flag)
•	i_only_workflow → apenas alterações em workflow (flag)

Filtros do relatório:
•	Unidades: multi-seleção (OBRIGATÓRIO)
•	Secções: multi-seleção
•	Colaboradores: multi-seleção
•	Estado da troca: multi-seleção
•	Histórico de alterações: check-box
•	Período
•	Ordenação: radio button
 
Informação técnica
•	Nome do relatório: Alterações à Escala
•	Key: ScheduleExchanges
•	Função: S_PCK_CORE_REPORTS.GET_CHANGE_SCHEDULE
•	Local de impressão: Módulo “relatórios”
•	Formatos disponíveis: Excel, PDF
