## Alertas

O relatório **Alertas** apresenta todos os **parâmetros legais que não foram cumpridos** no período selecionado, identificando de forma detalhada os colaboradores em incumprimento e a natureza exata de cada violação legal.

Para cada ocorrência, o relatório indica:
- o **colaborador** a que o incumprimento diz respeito;
- o **parâmetro legal** que não foi respeitado;
- o **valor legal definido** para esse parâmetro;
- o **valor efetivamente aplicado**;
- o **valor de incumprimento**, ou seja, em quantas unidades o valor aplicado excedeu o limite legal.

Adicionalmente, o relatório disponibiliza informação de auditoria relativa à **última alteração efetuada**, incluindo:
- o **utilizador** que realizou a alteração;
- a **data** em que essa alteração ocorreu;
- e a indicação de **troca**, sempre que tenha existido alguma intervenção desse tipo.

No cabeçalho, o relatório apresenta claramente a loja/unidade e o período de análise selecionados pelo utilizador.
Os resultados encontram-se organizados por secção, sendo que a primeira entrada da tabela corresponde à secção escolhida no momento da extração.
A tabela do relatório é composta por **11 Colunas:**
1.  **Número Mecanográfico** -- número identificativo do colaborador
2.  **Colaborador** -- nome do colaborador
3.  **Parâmetro Legal** -- parâmetro legal avaliado
4.  **Valor Legal** -- limite legal definido
5.  **Data Início** -- data de início do incumprimento
6.  **Data Fim** -- data de fim do incumprimento
7.  **Valor Aplicado** -- valor efetivamente registado
8.  **Valor de Incumprimento** -- diferença entre o valor aplicado e o valor legal
9.  **Utilizador** -- utilizador responsável pela última alteração
10. **Data** -- data da última alteração
11. **Troca** -- indicação de troca, caso exista

<img width="1884" height="604" alt="image" src="https://github.com/user-attachments/assets/29bf8083-d1d4-4494-9004-2ee56291030b" />


**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidades (multi-seleção)
- **i_fk_section** → secções (multi-seleção)
- **i_fk_employee** → colaboradores (multi-seleção)
- **i_legal_params** → parâmetros legais (drop-down / configuração)
- **i_start_date** / i_end_date → período

**Filtros do relatório** 

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Parametros legais:** drop-down
*	**Período**
*	**Ordenação:** radio button

<img width="1358" height="645" alt="image" src="https://github.com/user-attachments/assets/01e37f34-c373-49c2-a390-3daf9ab6a168" />


**Informação técnica**

- **Nome do relatório:** Alertas
- **Função:** S_PCK_CORE_REPORTS.GET_ALERTS
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Algoritmo de Descansos -Horas anuais

*(conteúdo não fornecido)*

---

## Alterações à Escala

O relatório **Alterações à Escala** apresenta todas as **alterações efetuadas às escalas de trabalho** dos colaboradores no período selecionado, permitindo acompanhar de forma detalhada o histórico de mudanças de horário e carga horária.

Para cada alteração registada, o relatório identifica:
* o colaborador afetado
* a data em que ocorreu a alteração da escala;
* o horário e carga anteriores à alteração;
* o horário e carga atuais, após a alteração;
* o motivo da alteração, conforme selecionado no momento da execução;
* os utilizadores responsáveis pela criação e pela alteração da escala;
* as datas de criação e de alteração;
* o número da troca, quando aplicável;
* e o estado da troca, permitindo perceber em que fase do processo se encontra.
  
No **cabeçalho**, o relatório apresenta a **unidade**, o **período** e a **secção** selecionados, bem como o **total de alterações** encontradas para os critérios definidos.

Os resultados são organizados por **secção**, apresentando de forma cronológica todas as alterações realizadas aos horários dos colaboradores.

A tabela do relatório é composta por **12 colunas**:

1.  **Matrícula** -- número identificativo do colaborador
2.  **Nome do Colaborador** -- nome completo do colaborador
3.  **Data** -- dia em que a escala foi alterada
4.  **Anterior – Horário / Carga** -- horário e respetiva carga antes da alteração
5.  **Atual – Horário / Carga** -- horário e respetiva carga após a alteração
6.  **Motivo da Alteração** -- motivo selecionado para a alteração da escala
7.  **Utilizador de Criação** -- utilizador que criou a alteração
8.  **Data de Criação** -- data em que a alteração foi criada
9.  **Utilizador de Alteração** -- utilizador que efetuou a última alteração
10. **Data de Alteração** -- data da última alteração registada
11. **Nº Troca** -- número identificativo da troca
12. **Estado da Troca** -- estado atual da troca

<img width="1853" height="476" alt="image" src="https://github.com/user-attachments/assets/dbc90cd2-a082-4d59-aa8c-383f95b166e7" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidades (multi-seleção)
- **i_fk_section** → secções (multi-seleção)
- **i_fk_employee** → colaboradores (multi-seleção)
- **i_begin_date / i_end_date** → período
- **i_status** → estado(s) da troca (multi-seleção)
- **i_show_history** → mostrar histórico de alterações (flag)
- **i_only_workflow** → apenas alterações em workflow (flag)

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Estado da troca:** multi-seleção
*	**Histórico de alterações:** check-box
*	**Período**
*	**Ordenação:** radio button

<img width="1358" height="644" alt="image" src="https://github.com/user-attachments/assets/09b30f0b-b5fc-42b3-b6a8-eec1aa3d0d6e" />

**Informação técnica**

- **Nome do relatório:** Alterações à Escala
- **Key:** ScheduleExchanges
- **Função:** S_PCK_CORE_REPORTS.GET_CHANGE_SCHEDULE
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Alterações de Carga Horária

O relatório **Alterações de Carga Horária** apresenta todas as modificações efetuadas à carga horária contratual dos colaboradores, permitindo acompanhar quando essas alterações foram criadas, qual a nova carga atribuída e o respetivo período de vigência.

Para cada registo, o relatório identifica o colaborador, a data em que a alteração foi criada, a nova carga horária definida, bem como a data de início e de fim em que essa carga horária se encontra ativa. É ainda apresentado o estado da alteração, permitindo distinguir, por exemplo, alterações processadas ou ainda pendentes.

No cabeçalho, o relatório apresenta a unidade e a secção selecionadas, servindo de enquadramento aos dados listados.

Os resultados são apresentados de forma tabular e o relatório é composto por **7 colunas**:

1.  **Matrícula** -- número identificativo do colaborador
2.  **Nome do Colaborador** -- nome completo do colaborador
3.  **Data Criação CH** -- data em que a alteração da carga horária foi criada
4.  **Nova Carga Horária** -- nova carga horária atribuída ao colaborador
5.  **Data Início CH** -- data a partir da qual a nova carga horária entra em vigor
6.  **Data Fim CH** -- data em que termina a vigência da nova carga horária
7.  **Estado** -- estado atual da alteração da carga horária

<img width="1906" height="495" alt="image" src="https://github.com/user-attachments/assets/2ad199be-e6ea-4909-82bb-576206a9623f" />


**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi-seleção)
- **I_FK_SECTION** → secções (multi-seleção)
- **I_FK_EMPLOYEE** → colaboradores (multi-seleção)
- **I_BEGIN_DATE / I_END_DATE** → período de criação / alteração
- **I_FK_CONTRACT_NUMBER** → número de contrato (multi-seleção)
- **I_STATUS** → estado da alteração (string / lista)

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATORIO)
*	**Secção:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Tipo de contrato:** multi-seleção
*	**Estado:** drop-down
*	**Período de criação/alteração**
*	**Ordenação:** radio button

<img width="1373" height="657" alt="image" src="https://github.com/user-attachments/assets/24aae661-8cf1-4119-b0a2-6f9ce6736557" />


**Informação técnica**

- **Nome do relatório:** Alterações de Carga Horária
- **Key:** WorkloadChange
- **Função:** S_PCK_CORE_REPORTS.GET_WORKLOAD_CHANGE
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Ausências Classificadas

O relatório **Ausências Classificadas** apresenta todas as ausências registadas e classificadas por código, por colaborador, num determinado período. Este relatório permite analisar, de forma detalhada, o tipo de ausência ocorrida, a sua duração e o processo de classificação associado.

Para cada ausência registada, o relatório identifica o colaborador, a data em que a ausência ocorreu, o dia da semana correspondente, o código e a descrição da ausência, bem como o tempo total em horas e a duração em dias. Adicionalmente, é possível saber quem efetuou a classificação da ausência e em que data essa classificação foi realizada, garantindo rastreabilidade e controlo do processo.

No cabeçalho, o relatório apresenta o período, a unidade e a secção selecionados, enquadrando a informação apresentada.

Os dados são apresentados em formato tabular e o relatório é composto por 10 colunas:

1.  **Matrícula** -- número identificativo do colaborador
2.  **Nome** -- nome completo do colaborador
3.  **Data** -- data em que ocorre a ausência classificada
4.  **Dia da Semana** -- dia da semana correspondente à data da ausência
5.  **Código da Ausência** -- código associado ao tipo de ausência
6.  **Ausência** -- descrição do tipo de ausência
7.  **Tempo** -- duração da ausência em horas
8.  **Dias** -- duração da ausência em dias
9.  **Classificado por** -- utilizador que efetuou a classificação da ausência
10. **Classificado em** -- data em que a ausência foi classificada

<img width="1861" height="468" alt="image" src="https://github.com/user-attachments/assets/a4ced93d-3800-4c33-8757-90ef4b45c263" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi)
- **I_FK_SECTION** → secções (multi)
- **I_FK_EMPLOYEE**→ colaboradores (multi)
- **I_BEGIN_DATE / I_END_DATE** → período
- **I_ABSENCE_REASON** → motivo (1 / código)

**Filtros do relatório**

* **Unidades:** multi-seleção (OBRIGATORIO)
* **Secções:** multi-seleção
* **Colaboradores:** multi-seleção
* **Motivo de Ausência:** drop-down
* **Período**

<img width="1370" height="656" alt="image" src="https://github.com/user-attachments/assets/b9ef0fec-d9d2-43a0-b443-410d8cb41c80" />

**Informação técnica**

- **Nome do relatório:** Ausências Classificadas
- **Key:** ClassifiedAbsences
- **Função:** S_PCK_CORE_EXECUTION_REPORTS.Get_absence
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Banco de horas

O relatório **Banco de Horas** apresenta todas as informações relativas à gestão do banco de horas dos colaboradores, organizadas por unidade, secção e colaborador, para um determinado **ano e trimestre de referência**. Este relatório permite acompanhar, de forma detalhada, os saldos acumulados, as compensações efetuadas ao longo do trimestre e a eventual existência de horas pendentes de pagamento.

Para cada colaborador, o relatório disponibiliza dados contratuais relevantes, como a data de admissão, categoria profissional e, quando aplicável, a data de demissão, bem como informação específica do banco de horas, incluindo a quota anual atribuída, os saldos anuais e trimestrais, as compensações mensais e o total de horas a pagar ou já pagas.

No cabeçalho, o relatório apresenta a unidade, a secção e o período selecionado, correspondente ao trimestre dentro do ano definido.

Os dados são apresentados em formato tabular e o relatório é composto por 16 colunas:

- **Nº Mecanográfico** -- número identificativo do colaborador
- **Nome** -- nome completo do colaborador
- **Data de Admissão** -- data de entrada do colaborador na empresa
- **Data de Demissão** -- data de saída do colaborador, quando aplicável
- **Categoria** -- categoria profissional do colaborador
- **Quota Anual de BH** -- total anual de horas atribuídas ao banco de horas
- **Saldo Quota Anual de BH** -- saldo disponível da quota anual
- **Saldo Atual de BH** -- saldo atual acumulado no banco de horas
- **Saldo do Trimestre** -- saldo correspondente ao trimestre selecionado
- **Compensação – Início do Trimestre** -- saldo inicial do trimestre
- **Compensação – Saldo 1º Mês** -- saldo após o primeiro mês do trimestre
- **Compensação – Saldo 2º Mês** -- saldo após o segundo mês do trimestre
- **Compensação – Saldo 3º Mês** -- saldo após o terceiro mês do trimestre
- **Ausência Prolongada** -- indicação da existência de ausências prolongadas
- **Horas a Pagar de BH** -- total de horas de banco de horas a pagar
- **Horas Pagas** -- total de horas de banco de horas já pagas

<img width="1879" height="410" alt="image" src="https://github.com/user-attachments/assets/e3cb74d2-d786-4581-b9d0-569cfaf9ec7e" />



**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi-seleção)
- **I_FK_SECTION** → secções (multi-seleção)
- **I_FK_EMPLOYEE** → colaboradores (multi-seleção)
- **I_YEAR** → ano de referência
- **I_TRIMESTER** → trimestre (valores de 1 a 4)
- **I_ISACTIVE** → estado do colaborador (ativos / todos)

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATORIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Colaboradores ativos:** check-box

<img width="1372" height="655" alt="image" src="https://github.com/user-attachments/assets/40abc426-a607-4c06-a0b8-47305e4886cb" />


**Informação técnica**

- **Nome do relatório:** Banco de Horas
- **Key:** TimeBank
- **Função:** S_PCK_CORE_REPORTS.GET_TIMEBANK
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Cálculo de ausências para prémio

Este relatório é um mapa de controlo e apuramento de ausências com impacto no cálculo de prémios, utilizado para identificar e quantificar as horas de ausência dos colaboradores num determinado período, bem como comparar essas horas com as horas potenciais elegíveis para prémio.

O relatório apresenta uma tabela consolidada com informação mensal por colaborador, permitindo analisar o impacto das ausências no apuramento do prémio.

A tabela inclui os seguintes campos:

-	**Data de Atualização** – data em que o cálculo ou extração da informação foi atualizado no sistema
-	**Ano** – ano de referência do cálculo
-	**Mês** – mês a que os dados dizem respeito
-	**Empresa** – entidade empresarial associada ao colaborador
-	**Unidade** – unidade operacional onde o colaborador está alocado
- **Secção** – área funcional ou departamento do colaborador
- **Nº Mecan.** – número interno de identificação do colaborador
-	**Colaborador** – nome completo do colaborador
-	**Motivo de Ausência** – código ou classificação do motivo da ausência registada
-	**Horas Mês** – total de horas de ausência registadas no período considerado
-	**Horas Potenciais** – total de horas elegíveis para prémio no mesmo período
-	**Estado da GT** – estado de tratamento ou validação da gestão de tempos (ex.: Tratado, Por Tratar)

Cada linha corresponde ao registo de ausências de um colaborador para um determinado motivo e período mensal, permitindo analisar o impacto dessas ausências na elegibilidade ou cálculo do prémio.

<img width="945" height="267" alt="image" src="https://github.com/user-attachments/assets/aa83f9b8-4750-46be-8dc5-cf4629591213" />

**Parâmetros do relatório (back-end)**

-	**I_FK_UNIT** → unidades (multi-seleção)
-	**I_FK_SECTION** → secções (multi-seleção)
-	**I_FK_EMPLOYEE** → colaboradores (multi-seleção)
-	**I_MONTH** → mês de referência (DATE)
-	**I_ISACTIVE** → estado do colaborador (ativos / todos)
  
**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATORIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Colaboradores ativos:** check-box
*	**Mês:** drop-down
*	**Ano:** drop-down

<img width="1361" height="650" alt="image" src="https://github.com/user-attachments/assets/36a109dd-2f0e-4464-b65b-0a43cbc242e1" />

**Informação técnica**

-	**Nome do relatório:** Cálculo de Ausências para Prémio
-	**Key:** AbsenceCalculation
-	**Função:** S_PCK_CORE_EXECUTION_REPORTS.Get_Absences_Prm_Calculation
-	**Local de impressão:** Módulo “relatórios”
-	**Formatos disponíveis:** Excel

---

## Colaboradores Demitidos

O relatório **Colaboradores Demitidos** apresenta a listagem dos colaboradores que cessaram vínculo com a empresa num determinado período, organizados por **secção** e por **mês de demissão**. Este relatório permite acompanhar não só a informação contratual associada à demissão, como também o estado da Gestão de Tempos no mês da demissão e no mês imediatamente anterior.

Para cada colaborador demitido, o relatório identifica a data de admissão, a data de demissão e os respetivos estados da Gestão de Tempos e do envio da Gestão de Tempos, garantindo controlo e validação do processo administrativo associado à saída do colaborador.

No cabeçalho, o relatório apresenta a unidade, o período e a secção selecionados, contextualizando a informação apresentada.

Os dados são apresentados em tabelas separadas por secção e por mês, facilitando a análise cronológica e organizacional das demissões.

O relatório é composto por 8 colunas:
- **Nº Mecanográfico** -- número identificativo do colaborador
- **Nome** -- nome completo do colaborador
- **Data de Admissão** -- data de entrada do colaborador na empresa
- **Data de Demissão** -- data de cessação do vínculo laboral
- **Estado da Gestão de Tempos** -- estado da gestão de tempos no mês da demissão
- **Estado Envio da Gestão de Tempos** -- estado do envio da gestão de tempos no mês da demissão
- **Estado da Gestão de Tempos (Mês Anterior)** -- estado da gestão de tempos no mês anterior à demissão
- **Estado Envio da Gestão de Tempos (Mês Anterior)** -- estado do envio da gestão de tempos no mês anterior à demissão

<img width="1868" height="249" alt="image" src="https://github.com/user-attachments/assets/c47201de-ad89-49b1-b249-d83645674e26" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi-seleção)
- **I_FK_SECTION** → secções (multi-seleção)
- **I_FK_EMPLOYEE** → colaboradores (multi-seleção)
- **I_BEGIN_DATE / I_END_DATE** → período
- **I_IDIOMA** → idioma

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Período**
*	**Ordenação:** radio-button

<img width="1373" height="658" alt="image" src="https://github.com/user-attachments/assets/54a4a582-fc0a-433f-bb26-7d9e0b20418c" />

**Informação técnica**

- **Nome do relatório:** Colaboradores Demitidos
- **Key:** FiredCollaborators
- **Função:** S_PCK_CORE_EXECUTION_REPORTS.Get_Fired_Collaborators
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Colaboradores e Carga Mensal

O relatório **Colaboradores e Carga Mensal** apresenta, para um determinado período, a informação mensal dos colaboradores, permitindo analisar de forma integrada a função desempenhada, o tipo de contrato, a carga horária atribuída e as ausências ocorridas.

Este relatório possibilita uma visão consolidada da situação contratual e operacional dos colaboradores, cruzando dados de enquadramento organizacional (unidade e secção), carga horária prevista e eventuais ausências registadas no período selecionado, bem como as respetivas datas.

Para cada colaborador, é possível identificar a função exercida, o contrato em vigor (em horas), a carga horária associada e, sempre que aplicável, o motivo da ausência e o intervalo temporal em que esta ocorreu.

No cabeçalho, o relatório apresenta o período inicial e final selecionados, permitindo enquadrar temporalmente a informação apresentada.

Os dados são apresentados em formato tabular e o relatório é composto por 13 colunas:

- **Período Início** -- data inicial do período selecionado
- **Período Final** -- data final do período selecionado
- **Unidade** -- unidade onde o colaborador se encontra afeto
- **Secção** -- secção/departamento do colaborador
- **Código do Operador** -- código interno do operador
- **Nº Mecanográfico** -- número mecanográfico do colaborador
- **Colaborador** -- nome completo do colaborador
- **Função** -- função desempenhada pelo colaborador
- **Contrato** -- tipologia de contrato associada (em horas)
- **Carga (h)** -- carga horária do colaborador no período
- **Motivo da Ausência** -- motivo da ausência, quando existente
- **Início da Ausência** -- data de início da ausência
- **Fim da Ausência** -- data de fim da ausência

<img width="1854" height="611" alt="image" src="https://github.com/user-attachments/assets/def2eea3-56fc-4763-a248-2090fc06db3d" />

**Parâmetros do relatório (back-end)**

- **Unidades** → seleção por *drop-down* (**obrigatório**)
- **Secções** → seleção por *drop-down*
- **Colaboradores** → seleção por *drop-down*
- **Período** → definição do período inicial e final

**Filtros do relatório**

*	**Unidades:** drop-down  (OBRIGATÓRIO)
*	**Secção:** drop-down
*	**Colaboradores:** drop-down
*	**Período**
  
<img width="1371" height="657" alt="image" src="https://github.com/user-attachments/assets/4bda73b7-1a6b-492a-bd24-5f9a96acdcff" />


**Informação técnica**

- **Nome do relatório:** Colaboradores e Carga Mensal
- **Key:** CollaboratorWorkload 
- **Função:** PCK_CORE_REPORTS.GET_COLAB_DIF_CARGA
- **Módulo:** Relatórios
- **Formato de saída:** Excel

---

## Colaboradores por Motivos de Ausência

O relatório **Colaboradores por Motivos de Ausência** apresenta todas as ausências registadas por colaborador, organizadas de acordo com o motivo da ausência, num determinado período de tempo. Este relatório permite analisar de forma detalhada os períodos de ausência, o respetivo enquadramento regulamentar e o impacto na dedução de dias.

Para cada ausência registada, o relatório identifica o colaborador, o intervalo temporal da ausência (data de início e data de fim), o motivo associado, o número total de dias marcados e o número de dias efetivamente deduzidos, de acordo com as regras de contagem definidas (por exemplo, regras de dedução de contingente). Adicionalmente, é possível identificar a origem do registo da ausência, o utilizador responsável pela sua marcação e a data em que a ausência foi criada no sistema.

O relatório encontra-se organizado por secção, permitindo uma leitura clara e estruturada da informação por área organizacional.

No cabeçalho, o relatório apresenta a unidade, o período selecionado e o motivo de ausência, enquadrando a informação apresentada.

Os dados são apresentados em formato tabular e o relatório é composto pelas seguintes colunas:

- **Nº Mecanográfico** -- número mecanográfico do colaborador
- **Colaborador** -- nome completo do colaborador
- **Data Início** -- data de início da ausência
- **Data Fim** -- data de fim da ausência
- **Motivo de Ausência** -- motivo associado à ausência
- **Nº Tot. Dias** -- número total de dias marcados para a ausência
- **Nº Dias Deduzidos** -- número de dias efetivamente deduzidos, de acordo com as regras de contagem aplicáveis
- **Tempo** -- duração da ausência em horas, quando aplicável
- **Origem** -- origem do registo da ausência (ex.: Planeamento, Gestão de Tempos)
- **Utilizador** -- utilizador que efetuou o registo da ausência
- **Data Criação** -- data em que a ausência foi registada no sistema

<img width="1872" height="150" alt="image" src="https://github.com/user-attachments/assets/e559b332-9a21-4a12-b278-72500c69b113" />


**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidades (multi-seleção)
- **i_fk_section** → secções (multi-seleção)
- **i_fk_employee** → colaboradores (multi-seleção)
- **i_absence_reason** → motivo de ausência (código/valor)
- **i_begin_date / i_end_date** → período
- **i_has_timemanagement** → com ou sem Gestão de Tempos (flag)

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Motivo de ausência**: drop-down
*	**Período**

<img width="1364" height="656" alt="image" src="https://github.com/user-attachments/assets/24039938-5939-4d56-b281-869406206d70" />


**Informação técnica**

- **Nome do relatório:** Colaboradores por Motivos de Ausência
- **Key:** Absences
- **Função:** S_PCK_CORE_REPORTS.GET_ABSENCES
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Colaboradores por Motivos de Compensação

O relatório **Colaboradores por Motivos de Compensação** apresenta todas as compensações atribuídas aos colaboradores, organizadas por motivo de compensação, num determinado período de tempo. Este relatório funciona como um mapa de controlo, permitindo acompanhar e analisar compensações de tempo de trabalho, tais como **Banco de Horas**, **Trabalho Suplementar Compensado** ou outros tipos de compensação definidos no sistema.

Para cada registo de compensação, o relatório identifica o colaborador, a data em que a compensação foi registada, o motivo associado, o tempo planeado inicialmente e o tempo efetivamente executado. Adicionalmente, é possível identificar a origem do registo (por exemplo, Planeamento ou Execução), bem como o utilizador responsável pela criação do registo e a respetiva data de criação, garantindo rastreabilidade e controlo do processo.

O relatório encontra-se organizado por secção, sendo apresentada uma tabela distinta para cada secção, o que facilita a análise por área organizacional.

No cabeçalho, o relatório apresenta a unidade, o período analisado e a secção selecionada, contextualizando a informação apresentada.

Os dados são apresentados em formato tabular e o relatório é composto pelas seguintes colunas:

- **Matrícula** -- número interno de identificação do colaborador
- **Colaborador** -- nome completo do colaborador
- **Data** -- data em que a compensação foi registada
- **Motivo de Compensação** -- tipo de compensação atribuída (ex.: Banco de Horas, Trabalho Suplementar)
- **Total Planeado** -- tempo de compensação inicialmente previsto
- **Total Executado** -- tempo de compensação efetivamente realizado
- **Origem** -- origem do registo da compensação (ex.: Planeamento, Execução)
- **Utilizador** -- utilizador ou sistema que efetuou o registo
- **Data de Criação** -- data em que o registo de compensação foi criado
Cada linha da tabela corresponde a um registo individual de compensação associado a um colaborador.

<img width="1874" height="144" alt="image" src="https://github.com/user-attachments/assets/efc737fd-f8a2-43e0-abee-909aa756b3c6" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidades (multi-seleção)
- **i_fk_section** → secções (multi-seleção)
- **i_fk_employee** → colaboradores (multi-seleção)
- **i_compensation_reason** → motivo de compensação (NUMBER)
- **i_is_active** → apenas colaboradores ativos / todos (flag)
- **i_begin_date / i_end_date** → período
- **i_has_timemanagement** → com ou sem Gestão de Tempos (flag)

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secção:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Motivo de Compensação:** drop-down
*	**Período**
*	**Colaborador ATIVOS/INATIVOS:** radio button

<img width="1361" height="649" alt="image" src="https://github.com/user-attachments/assets/cff52051-258e-4bce-94e0-32e0c3cadf73" />

**Informação técnica**

- **Nome do relatório:**  por Motivos de Compensação
- **Key:** CompensatoryDaysOff
- **Função:** S_PCK_CORE_REPORTS.GET_COMPENSATIONS
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Contingentes

O relatório **Contingentes** apresenta os contingentes atribuídos aos , permitindo analisar, de forma detalhada, quais os contingentes aplicados, a que períodos dizem respeito, qual o direito atribuído, o que já foi deduzido e o saldo disponível.

Este relatório é utilizado para controlo de contingentes como Férias, Banco de Horas, Faltas Injustificadas, Folgas por excesso de horas, entre outros, possibilitando acompanhar a evolução da utilização ao longo do tempo, bem como os períodos de validade e dedução associados.

Para cada colaborador, o relatório identifica o tipo de contingente aplicado, as datas de início e fim da sua vigência, o total de dias ou horas atribuídos (direito), o total já deduzido e o saldo remanescente. Adicionalmente, é possível visualizar o período exato em que ocorreram as deduções, assegurando transparência e rastreabilidade.

O relatório encontra-se organizado por secção e por período, sendo apresentada uma tabela distinta para cada conjunto de resultados.

No cabeçalho, o relatório apresenta a empresa, a secção e o período selecionado, contextualizando a informação apresentada.

Os dados são apresentados em formato tabular e o relatório é composto pelas seguintes colunas:

- **Matrícula** -- número identificativo do colaborador
- **Nome** -- nome completo do colaborador
- **Tipo** -- código identificativo do contingente
- **Contingente** -- designação do contingente aplicado
- **Data Início** -- data de início da aplicação do contingente
- **Data Fim** -- data de fim da aplicação do contingente
- **Direito** -- total de dias ou horas atribuídos ao contingente
- **Dedução** -- total de dias ou horas já deduzidos
- **Saldo** -- saldo disponível após deduções
- **Início da Dedução** -- data de início do período de dedução
- **Fim da Dedução** -- data de fim do período de dedução

Cada linha da tabela corresponde a um contingente específico aplicado a um colaborador.

<img width="1858" height="496" alt="image" src="https://github.com/user-attachments/assets/cecedd41-b381-454d-9e7a-5bdf7fa6d09a" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi-seleção)
- **I_FK_SECTION** → secções (multi-seleção)
- **I_FK_EMPLOYEE** → colaboradores (multi-seleção)
- **I_YEAR** → ano(s) de referência (lista)
- **I_CONTINGENT** → contingente(s) (lista)
- **I_ACTIVE_COLLABS** → apenas colaboradores ativos / todos (flag)
- **I_FILTERY_BY** → critério de filtragem (ex.: data de validade ou data de dedução)
- **I_SPECIFIC_YEAR** → utilizar apenas o ano específico selecionado (flag)

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Contingentes:** multi-seleção
*	**Ano:** multi-seleção
*	**Contingente exclusivo do ano:** check-box
*	**Filtro por data de validade /data de dedução:** radio-button
*	**Colaborador ATIVOS/INATIVOS:** radio button

<img width="1359" height="645" alt="image" src="https://github.com/user-attachments/assets/b6d21e94-e483-4ba0-9d10-71a69ce89049" />

**Informação técnica**

- **Nome do relatório:** Contingentes
- **Key:** Contingent
- **Função:** S_PCK_CORE_REPORTS.Get_contingents
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Contratações e Demissões

O relatório **Contratações e Demissões** apresenta todos os colaboradores que foram **contratados e/ou demitidos** no período selecionado, permitindo acompanhar os movimentos de entrada e saída de colaboradores na organização.

Os dados são organizados por empresa e secção, sendo apresentada uma tabela distinta para cada secção, o que facilita a leitura e a análise por área organizacional.

No cabeçalho, o relatório apresenta o período selecionado, contextualizando temporalmente a informação apresentada.


Os dados são apresentados em formato tabular e o relatório é composto por 9 colunas:

- **Nº Mecanográfico** -- número identificativo interno do colaborador
- **Nome** -- nome completo do colaborador
- **Número de Contribuinte** -- número de identificação fiscal do colaborador
- **Data de Nascimento** -- data de nascimento do colaborador
- **Segurança Social** -- número de identificação na Segurança Social
- **Data de Admissão** -- data em que o colaborador foi admitido
- **Data de Demissão** -- data em que o colaborador foi demitido
- **Cargo** -- função/cargo desempenhado pelo colaborador
- **Carga Semanal** -- carga horária semanal contratual

Cada linha da tabela corresponde a um colaborador contratado ou demitido no período selecionado.

<img width="1860" height="485" alt="image" src="https://github.com/user-attachments/assets/b192d5f6-acc5-445d-8bd3-a87182b305e9" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (seleção única)
- **I_FK_SECTION** → secções
- **I_FK_EMPLOYEE** → colaboradores
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

*	**Unidades:** drop-down
*	**Secções:** drop-down
*	**Colaboradores:** drop-down
*	**Período**

<img width="1371" height="658" alt="image" src="https://github.com/user-attachments/assets/a00b373d-48e7-4fcd-91b9-9ecae94f79d6" />


**Informação técnica**

- **Nome do relatório:** Contratações e Demissões
- **Key:** EmployeeHiring
- **Função:** S_PCK_CORE_REPORTS.GET_EMPLOYEEHIRING
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Contratos dos Colaboradores

O relatório **Contratos dos Colaboradores** apresenta informação detalhada sobre os **contratos de trabalho associados a cada colaborador**, permitindo analisar o tipo de contrato em vigor, o respetivo período de validade, a carga horária semanal e as condições associadas ao regime de trabalho.

A informação encontra-se organizada por unidade e secção, sendo apresentadas tabelas distintas para cada secção, facilitando a leitura e análise por área organizacional.

No cabeçalho, o relatório apresenta a unidade, a secção e o tipo de contrato selecionados, bem como a data de extração, contextualizando a informação apresentada.

Os dados são apresentados em formato tabular e o relatório é composto por 10 colunas:

- **Nº Mecanográfico** -- número identificativo interno do colaborador
- **Nome** -- nome completo do colaborador
- **Contrato** -- tipo de contrato atribuído ao colaborador
- **Data do Contrato** -- período de vigência do contrato
- **Contrato de Adaptabilidade** -- indicação de existência e tipo de adaptabilidade contratual
- **Carga Semanal** -- carga horária semanal contratual
- **Intervalo de Refeição** -- intervalo de refeição, apresentado com valores de **início** e **máximo**
- **Dias de Trabalho por Semana** -- número de dias de trabalho semanais, com valores de **início** e **máximo**
- **Nº de Dias com Intervalo** -- número de dias com intervalo, com valores de **início** e **máximo**
- **IHT** -- indicação se o colaborador tem **Isenção de Horário de Trabalho** (Sim/Não)

Cada linha corresponde a um colaborador e ao respetivo contrato ativo ou histórico, conforme os filtros aplicados.

<img width="1860" height="389" alt="image" src="https://github.com/user-attachments/assets/42d38f21-3f79-4245-86ea-7536458a1111" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidades (multi-seleção)
- **i_fk_section** → secções (multi-seleção)
- **i_fk_employee** → colaboradores (multi-seleção)
- **i_fk_contract_labor** → tipo / número de contrato

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secção:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Tipo de contrato:** drop-down
*	**Ordenação:** radio button

<img width="1372" height="654" alt="image" src="https://github.com/user-attachments/assets/e7b4ee45-bb30-4bdf-9fcd-9fd5bca13898" />


**Informação técnica**

- **Nome do relatório:** Contratos dos Colaboradores
- **Key:** Contracts
- **Função:** S_PCK_CORE_REPORTS.GET_EMPLOYEE_LABOR_CONTRACT
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Controlo de Limites de Marcação e Ausências

O relatório **Controlo de Limites de Marcação de Ausências** tem como objetivo apoiar o controlo e a validação de ausências que ultrapassam os limites definidos, nomeadamente ausências injustificadas ou que carecem de justificação adicional.

Para cada registo, o relatório apresenta o colaborador associado, o motivo da ausência, a data em que ocorreu, a justificação introduzida (quando existente), bem como a informação de auditoria relativa à criação do registo. Desta forma, garante-se rastreabilidade e controlo sobre o processo de marcação e validação de ausências.

No cabeçalho, o relatório apresenta a unidade, a secção e o período selecionado, sendo a informação organizada em tabelas separadas por unidade e secção.

Os dados são apresentados em formato tabular e o relatório é composto por 7 colunas:

- **Nº Mecanográfico** -- número identificativo do colaborador
- **Colaborador** -- nome do colaborador
- **Motivo de Ausência** -- motivo associado à ausência
- **Data** -- data em que ocorreu a ausência
- **Justificação** -- justificação associada à ausência
- **Criado por** -- utilizador que registou a informação
- **Criado em** -- data e hora de criação do registo

<img width="1868" height="158" alt="image" src="https://github.com/user-attachments/assets/fbf15c6b-8969-4988-8356-6ca61a0061a4" />

**Parâmetros do relatório (back-end)**

- **i_fk_units** → unidades (multi)
- **i_fk_sections** → secções (multi)
- **i_fk_absence_reason** → motivo de ausência (string)
- **i_begin_date / i_end_date** → período
- **i_employee_filter** → filtro adicional (ativos / inativos / todos)

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Motivo de ausência:** drop-down
*	**Período**
*	**Colaboradores ATIVOS/INATIVOS:** radio-button
*	**Ordenação (nome/número mecanográfico/ data):** radio button

<img width="1358" height="648" alt="image" src="https://github.com/user-attachments/assets/1fec1deb-4f81-4747-bb28-51c27eaeebad" />

**Informação técnica**

- **Nome do relatório:** Controlo de Limites de Marcação de Ausências
- **Key:** EmployeeAbsenceLimitsReport
- **Função:** S_PCK_CORE_REPORTS.EMPLOYEE_ABS_LIMITS
- **Local de impressão:** Módulo "relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Diferença de Cargas

O relatório **Diferença de Cargas** permite analisar se existem discrepâncias entre a **carga semanal média** prevista e a **carga semanal efetivamente executada**, por colaborador e por semana, no período selecionado. Este relatório é essencial para monitorizar desvios de carga horária e apoiar a gestão operacional e contratual.

A informação encontra-se organizada por secções, sendo apresentados os colaboradores associados a cada secção. Para cada colaborador, o relatório mostra a carga média, a carga semanal realizada e a diferença apurada, permitindo identificar facilmente situações de excesso ou défice de carga horária.

No cabeçalho, o relatório apresenta a unidade, o período selecionado e a data de extração.

Os dados são apresentados em formato tabular e incluem:

- **Nº Mecanográfico** -- número identificativo do colaborador
- **Colaborador** -- nome do colaborador
- **Semana(s)** -- colunas correspondentes a cada semana do período, identificadas pela data do primeiro dia da semana
- **Dados agregados**, divididos em:
  - **Média** -- média da carga semanal
  - **Carga semanal** -- carga semanal executada
  - **Diferença** -- diferença entre a média e a carga executada
 
<img width="1855" height="561" alt="image" src="https://github.com/user-attachments/assets/aeecd469-3988-4ba1-80c2-92145193da63" />

**Parâmetros do relatório (back-end)**

- **i_Fk_Unidade** → unidade (single)
- **i_Fk_Secao** → secções (multi)
- **i_Fk_Tipo_Posto** → tipos de posto (multi)
- **i_Data_Ini / i_Data_Fim** → período
- **i_Data** → data de referência
- **i_idioma** → idioma
- **i_dif_carga** → filtro de diferença de carga (T = todos, S = apenas com diferença, N = sem diferença)

**Filtros do relatório**

*	**Unidades:** drop-down (OBRIGATÓRIO)
*	**Secção:** drop-down
*	**Com diferença de carga (todos/sim/não):** radio-button
*	**Período**

<img width="1368" height="655" alt="image" src="https://github.com/user-attachments/assets/2bb0dbfb-8f63-4384-84ed-9e027db6d083" />

**Informação técnica**

- **Nome do relatório:** Diferença de Cargas
- **Key:** WeekDetailSchedule
- **Função:** S_CARGA_SEMANA_COLABORADOR.get
- **Local de impressão:** Módulo "relatórios" e vista "Detalhes das semanas/dias"
- **Formatos disponíveis:** Excel, PDF

---

## Diferença entre planeado e executado

O relatório **Diferença entre Planeado e Executado** permite comparar, de forma detalhada, as horas **planeadas** e as horas **efetivamente executadas** pelos colaboradores, ao nível diário. Este relatório é fundamental para analisar desvios de horários, atrasos, saídas antecipadas ou prolongamentos de jornada.

Para cada colaborador e para cada dia de trabalho, o relatório apresenta as horas de entrada e saída planeadas, as horas executadas e a respetiva diferença, bem como a indicação de isenção de horário de trabalho (IHT), quando aplicável.

No cabeçalho, o relatório apresenta a loja/unidade e o período selecionado. A informação encontra-se organizada por secção, com tabelas separadas por unidade e secção.

Os dados são apresentados em formato tabular e o relatório é composto por 7 colunas principais:

- **Nº Mecanográfico** -- número identificativo do colaborador
- **Colaborador** -- nome do colaborador
- **Data** -- data do dia de trabalho
- **Dia** -- dia da semana correspondente
- **Entrada** (Planeado, Executado, Diferença)
- **Saída** (Planeado, Executado, Diferença)
- **IHT** -- indicação se o colaborador possui isenção de horário de trabalho (S/N)

<img width="1857" height="559" alt="image" src="https://github.com/user-attachments/assets/3bf4e004-d7f2-4d44-8b60-509b5c33ca70" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidade (single)
- **i_fk_section** → secções
- **i_fk_employee** → colaboradores
- **i_begin_date / i_end_date** → período

**Filtros do relatório**

*	**Unidades:** drop-down (OBRIGATÓRIO)
*	**Secção:** drop-down
*	**Colaboradores:** drop-down
*	**Parâmetros legais:** drop-down
*	**Período**
*	**Ordenação (nome/número mecanográfico/ data):** radio button

<img width="1375" height="654" alt="image" src="https://github.com/user-attachments/assets/a58da446-d1d2-419b-811b-26e4f59eaef9" />

**Informação técnica**

- **Nome do relatório:** Diferença entre Planeado e Executado
- **Key:** DiffPlanExec
- **Função:** S_PCK_CORE_EXECUTION_REPORTS. Get_diff_plan_exec
- **Local de impressão:** Módulo "relatórios"

---

## Domingos e Feriados com Horas Complementares

O relatório **Domingos e Feriados com Horas Complementares** é um documento formal de comunicação e registo de trabalho em domingos, feriados e horas complementares, utilizado para informar e validar previamente os dias e horários em que o colaborador irá prestar trabalho adicional, com base num pacto de horas complementares previamente acordado. Serve como comprovativo administrativo e legal do agendamento dessas horas.

O corpo do documento apresenta:

-	Referência explícita ao pacto de horas complementares existente
-	Comunicação formal dos dias de trabalho previstos
-	Para cada registo são indicados:
    - Dia e data
    - Identificação do dia da semana
    - Horário de trabalho

Os dias encontram-se numerados e organizados cronologicamente, garantindo clareza e fácil leitura.

O documento inclui ainda:

-	Assinatura do responsável que emite a comunicação
-	Campo de recebido pelo colaborador, confirmando a tomada de conhecimento

<img width="817" height="484" alt="image" src="https://github.com/user-attachments/assets/0ab3488b-e19b-4842-81c8-8e638a7a0fd1" />

**Parâmetros do relatório (back-end)**

-	**I_fk_unit** → unidade (multi)
-	**I_fk_section** → secções (multi)
-	**I_fk_employee** → colaboradores (multi)
-	**I_year** → ano

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Ano: drop-down**

<img width="1356" height="648" alt="image" src="https://github.com/user-attachments/assets/c9a1b4e9-aeb3-442a-85a9-ea735f916714" />

**Informação técnica**
-	**Nome do relatório:** Domingos e Feriados com Horas Complementares
-	**Key:** AddicionalHours
-	**Função:** S_PCK_CORE_REPORTS.GET_DOM_FER_HC
-	**Local de impressão:** Módulo “relatórios” 

---

## Domingos, Fins de Semana e Feriados

O relatório **Domingos, Fins de Semana e Feriados** permite analisar o cumprimento das regras legais relativas ao usufruto de domingos, fins de semana e feriados por colaborador, num determinado ano. Este relatório é essencial para garantir o cumprimento da legislação laboral e das regras internas de descanso semanal.

Para cada colaborador, o relatório apresenta o número de feriados, domingos e fins de semana já gozados, bem como os que ainda se encontram em falta por usufruir, permitindo identificar situações de incumprimento ou necessidade de planeamento futuro.

No cabeçalho, o relatório apresenta a unidade e o ano selecionados. A informação encontra-se organizada por secção, sendo apresentadas tabelas separadas por secção.

Os dados são apresentados em formato tabular e o relatório é composto por 11 colunas:

- **Colaborador** -- nome do colaborador
- **Nº Mecanográfico** -- número identificativo do colaborador
- **Feriados** -- número de feriados gozados
- **Domingos gozados** -- número de domingos já usufruídos
- **Domingos (em falta)** -- número de domingos ainda por gozar
- **Fins de Semana gozados** -- número de fins de semana já gozados
- **Fins de Semana (em falta)** -- número de fins de semana ainda por gozar
- **Primeira Escala** -- data da primeira escala atribuída
- **Data de Admissão** -- data de admissão do colaborador
- **Data de Demissão** -- data de demissão (quando aplicável)
- **Contrato** -- tipo de contrato associado ao colaborador

<img width="1845" height="600" alt="image" src="https://github.com/user-attachments/assets/df6019cc-259d-4afe-affe-fcea70ba12a3" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidade (single)
- **i_fk_section** → secções
- **i_fk_employee** → colaboradores
- **i_year** → ano (NUMBER)
- **i_cond_status** → filtro (DOM / FDS / vazio)
- **I_COLAB_STATUS** → todos ou apenas ativos (flag)
- **I_CONTRACT_TYPE** → tipo de contrato / nº de dias de trabalho

**Filtros do relatório**

*	**Unidades:** drop-down (OBRIGATÓRIO)
*	**Secções:** drop-down
*	**Colaboradores:** drop-down
*	**Ano:** drop-down
*	**Somente colaboradores ativos:** check-box
*	**Colaboradores que ainda não atingiram os valores (todos / domingos / fins de semana):** radio button
*	**Contratos (Todos / 5 dias de trabalho):** radio button
*	**Ordenação:** radio button
  
<img width="1376" height="655" alt="image" src="https://github.com/user-attachments/assets/d6929db9-9422-45f8-9560-969885785d24" />

**Informação técnica**

- **Nome do relatório:** Domingos, Fins de Semana e Feriados
- **Key:** NonWorkingDays
- **Função:** S_PCK_CORE_REPORTS.GET_NON_WORKING_DAYS
- **Local de impressão:** Módulo Relatórios
- **Formatos disponíveis:** Excel, PDF

---

## Empréstimos

*(conteúdo não completo)*

---

## Entidades Oficiais

O relatório **Entidades Oficiais** apresenta a escala de trabalho semanal e a carga horária realizada por cada colaborador, permitindo uma visão clara dos horários efetivamente executados ao longo de uma semana.

No cabeçalho, o relatório apresenta a empresa, sede, atividade, departamento/secção, local de trabalho, período de abertura e o período selecionado. A informação encontra-se organizada por secção, com tabelas distintas por secção.

Os dados são apresentados em formato tabular e o relatório é composto por 11 colunas:

- **Nome** -- nome do colaborador
- **Matrícula** -- número mecanográfico do colaborador
- **Coluna por cada dia da semana** -- horário realizado pelo colaborador nesse dia
- **Carga semanal** -- carga horária semanal prevista
- **Carga realizada** -- carga horária efetivamente realizada

<img width="1889" height="222" alt="image" src="https://github.com/user-attachments/assets/00417c94-bd32-4dd0-b68c-47f2fd29b538" />

**Parâmetros do relatório (back-end)**

- **i_fk_unidade** → unidade (single)
- **i_fk_secao** → secções (multi)
- **i_fk_colaborador** → colaboradores (multi)
- **i_data_Ini / i_data_Fim** → período
- **i_hora** → hora de saída
- **i_tipo_rel** → tipo de relatório
- **i_tipo_hora** → saem antes/saem depois

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Tipo de relatório:** drop-down
*	**Horário de saída:** drop-down
*	**Período** (obrigatoriedade de uma semana)
*	**Planeamento extra:** check-box
*	**Ordenação:** radio button

<img width="1373" height="656" alt="image" src="https://github.com/user-attachments/assets/7c4612e5-4afe-4062-9bc9-65c7adf4ded3" />

**Informação técnica**

- **Nome do relatório:** Entidades Oficiais
- **Key:** WorkTime
- **Função:** S_RELATORIOS.get_entidade_oficial
- **Local de impressão:** Módulo Relatórios , Vista mensal de horários, Escala
- **Formatos disponíveis:** Excel, PDF

---

## Entidades Oficiais (Avaliação Noturna)

O relatório **Entidades Oficiais (Avaliação Noturna)** é equivalente ao relatório de Entidades Oficiais, mas com aplicação das regras específicas de **redução de horário noturno**, permitindo avaliar corretamente a carga horária quando existem períodos de trabalho noturno.

Este relatório é essencial para garantir o correto cálculo de tempos de trabalho noturnos e o cumprimento da legislação aplicável.

A estrutura do relatório, colunas apresentadas e organização por secção são idênticas ao relatório Entidades Oficiais.

<img width="1904" height="425" alt="image" src="https://github.com/user-attachments/assets/794655fe-efee-4a6c-97ea-15d0c0c14f71" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidade (single)
- **i_fk_section** → secções (multi)
- **i_fk_colaborador** → colaboradores (multi)
- **i_data_Ini / i_data_Fim** → período
- **i_hora** → hora de saída
- **i_tipo_rel** → tipo de relatório
- **i_tipo_hora** → saem antes/saem depois

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Tipo de relatório**: drop-down
*	**Horário de saída:** drop-down
*	**Período** (obrigatoriedade de uma semana)
*	**Planeamento extra:** check-box
*	**Ordenação:** radio button

<img width="1373" height="661" alt="image" src="https://github.com/user-attachments/assets/310b72bb-0bc0-47a9-8c07-97b66e61c9fb" />

**Informação técnica**

- **Nome do relatório:** Entidades Oficiais (Avaliação Noturna)
- **Key:** WorkTimeNightEvaluation
- **Função:** S_RELATORIOS.get_entidade_oficial
- **Local de impressão:** Módulo Relatórios / Vista mensal de horários / Escala
- **Formatos disponíveis:** Excel, PDF

---

## Envio de Gestão de Tempos para SAP

O relatório **Envio de Gestão de Tempos para SAP** permite acompanhar o estado do envio da informação de gestão de tempos dos colaboradores para o sistema SAP. Este relatório é essencial para garantir que os dados de tempos foram corretamente disponibilizados para integração externa e para identificar eventuais pendências ou bloqueios no processo de envio.

Para cada colaborador, o relatório indica se a informação já se encontra disponível no SAP, a data e hora desse estado, bem como o estado correspondente no WFM (Workforce Management). Adicionalmente, apresenta informação relevante como a carga semanal do colaborador e a existência de Isenção de Horário de Trabalho (IHT).

No cabeçalho, o relatório apresenta a empresa, o departamento/secção e o período selecionado, enquadrando temporal e organizacionalmente a informação. Os dados encontram-se organizados por secção, sendo apresentada uma tabela por cada secção.

Os dados são apresentados em formato tabular e o relatório é composto por 8 colunas:

- **Matrícula** -- número mecanográfico do colaborador
- **Nome** -- nome completo do colaborador
- **Status Envio SAP** -- estado do envio da gestão de tempos para o SAP
- **Data Status SAP** -- data e hora associadas ao estado do envio SAP
- **Status WFM** -- estado da gestão de tempos no WFM
- **Data Status WFM** -- data e hora do estado no WFM
- **IHT** -- indicação de isenção de horário de trabalho (S/N)
- **Carga Semanal** -- carga horária semanal do colaborador

<img width="1858" height="264" alt="image" src="https://github.com/user-attachments/assets/91cf2cab-4e21-4b98-8e08-f694717dbd9a" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (single)
- **I_FK_SECTION** → secções
- **I_FK_EMPLOYEE** → colaboradores
- **I_YEAR** → ano
- **I_MONTH** → mês

**Filtros do relatório**

*	**Unidades:** drop-down (OBRIGATÓRIO)
*	**Secções:** drop-down
*	**Colaboradores:** drop-down
*	**Período:** mês (drop-down) e ano (drop-down)
  
<img width="1373" height="657" alt="image" src="https://github.com/user-attachments/assets/26700b9c-409f-456b-8a41-2761d0aaf2a5" />

**Informação técnica**

- **Nome do relatório:** Envio de Gestão de Tempos para SAP
- **Key:** ShippingSAP
- **Função:** S_PCK_CORE_EXECUTION_REPORTS.GET_SHIPPING_SAP
- **Local de impressão:** Módulo Relatórios
- **Formatos disponíveis:** Excel, PDF

---

## Erros da Gestão de Tempos

O relatório **Erros da Gestão de Tempos** apresenta todos os erros registados no sistema de gestão de tempos, permitindo identificar inconsistências, falhas de marcação ou situações que necessitam de correção, por colaborador e por data.

Este relatório é fundamental para o controlo da qualidade da informação de tempos, permitindo uma atuação rápida sobre erros como ausência de marcações, tempos por classificar ou outras situações anómalas.

No cabeçalho, o relatório apresenta a empresa, o departamento/secção e o período selecionado. A informação encontra-se organizada por secção, sendo apresentada uma tabela distinta para cada secção.

Os dados são apresentados em formato tabular e o relatório é composto por 4 colunas:

- **Matrícula** -- número mecanográfico do colaborador
- **Nome** -- nome completo do colaborador
- **Data** -- data em que ocorreu o erro
- **Descrição** -- descrição do tipo de erro registado

<img width="1853" height="661" alt="image" src="https://github.com/user-attachments/assets/80acd666-c65f-44d5-963d-a81d08b59f9a" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade
- **I_FK_SECTION** → secções
- **I_FK_EMPLOYEE** → colaboradores
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

*	**Unidades:** drop-down (OBRIGATÓRIO)
*	**Secções:** drop-down
*	**Colaboradores:** drop-down
*	**Período**

<img width="1375" height="661" alt="image" src="https://github.com/user-attachments/assets/d48906e2-5dcb-4cd2-ba00-947299a56ccf" />

**Informação técnica**

- **Nome do relatório:** Erros da Gestão de Tempos
- **Key:** TmErrors
- **Função:** S_PCK_CORE_EXECUTION_REPORTS. Get_gt_errors
- **Local de impressão:** Módulo Relatórios
- **Formatos disponíveis:** Excel, PDF

---

## Escala de Trabalho

O relatório **Escala de Trabalho** apresenta os horários realizados pelos colaboradores, organizados por dia e por secção. Este relatório permite visualizar em que posto cada colaborador trabalhou, a carga horária associada e eventuais situações de polivalência entre secções.

Para cada dia de escala, o relatório indica o horário efetivamente realizado, a carga no posto, a secção de origem e, quando aplicável, a secção de destino e o novo horário resultante da polivalência. Inclui ainda campos para observações e assinatura do colaborador.

No cabeçalho, o relatório apresenta a data da escala, a unidade e a secção selecionadas. É apresentada uma tabela por dia.

No rodapé de cada tabela são listados os postos disponíveis na secção para o respetivo dia.

Os dados são apresentados em formato tabular e o relatório é composto por 10 colunas:

- **Matrícula** -- número mecanográfico do colaborador
- **Nome** -- nome do colaborador
- **Posto** -- posto onde o colaborador esteve alocado
- **Horário** -- horário realizado
- **Carga no Posto** -- carga horária associada ao posto
- **Secção Origem** -- secção de origem do colaborador
- **Secção Destino** -- secção de destino, caso exista polivalência
- **Horário (polivalência)** -- novo horário em caso de polivalência
- **Observação** -- observações adicionais
- **Assinatura** -- assinatura do colaborador
  
<img width="1863" height="487" alt="image" src="https://github.com/user-attachments/assets/eccf7655-302b-4509-97ea-0f3a23ee6c35" />

**Parâmetros do relatório (back-end)**

- **i_idioma** → idioma
- **i_data_Ini** → data início do período
- **i_data_Fim** → data fim do período
- **i_fk_unidade** → unidades (single)
- **i_fk_secao** → secções (multi)
- **i_fk_colaborador** → colaboradores (multi)
- **i_polivalencia** → polivalência (todos/secção/outra secção)
- **i_fk_tipo_posto** → tipos de posto (multi)
- **i_compensations** → incluir compensações (1=sim / 0=não)

**Filtros do relatório**

*	**Unidades:** drop-down (OBRIGATÓRIO)
*	**Secções:** drop-down
*	**Colaboradores:** drop-down
*	**Tipo de posto:** drop-down
*	**Período**
*	**Planeamento extra:** check-box
*	**Colaboradores (todos/presentes):** radio button
*	**Polivalência (todos/secção/outra secção):** radio button
*	**Ordenação:** radio button
*	**Opções de impressão (por escala / sem quebra / automático):** radio button

<img width="1371" height="658" alt="image" src="https://github.com/user-attachments/assets/48548966-b9bd-4d9d-8f21-c08e4e7d9c13" />

**Informação técnica**

- **Nome do relatório:** Escala de Trabalho
- **Key:** WorkSchedule
- **Função:** S_RELATORIOS.get_relatorio_escala
- **Local de impressão:** Módulo Relatórios, Vista mensal de horários, Escala
- **Formatos disponíveis:** Excel, PD

---

## Estado da Gestão de Tempos

O relatório **Estado da Gestão de Tempos** permite consultar o estado da gestão de tempos de cada colaborador numa data específica, indicando se o colaborador se encontra com a gestão de tempos bloqueada ou desbloqueada, bem como o estado da aplicação externa associada.

Este relatório é particularmente útil para monitorizar processos de fecho mensal, bloqueios automáticos e integração com sistemas externos.

No cabeçalho, o relatório apresenta a unidade, a secção e o período selecionados. A informação é apresentada em tabelas separadas por secção.

Os dados são apresentados em formato tabular e o relatório é composto por 7 colunas:

- **Nº Mecanográfico** -- número mecanográfico do colaborador
- **Nome** -- nome do colaborador
- **Estado WFM** -- estado da gestão de tempos (bloqueado/desbloqueado)
- **Data Estado WFM** -- data do estado no WFM
- **Utilizador** -- utilizador responsável pela alteração
- **Estado Aplicação Externa** -- estado na aplicação externa
- **Data Estado Aplicação Externa** -- data do estado externo

<img width="1857" height="610" alt="image" src="https://github.com/user-attachments/assets/ceb16efd-4d4e-4bf4-9620-aa1b596c69cc" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi)
- **I_FK_SECTION** → secções (multi)
- **I_FK_EMPLOYEE** → colaboradores (multi)
- **I_YEAR** → ano
- **I_MONTH** → mês
- **I_ISACTIVE** → estado do colaborador
- **I_FK_STATE** → estados
- **I_IDIOMA** → idioma

**Filtros do relatório**

*	**Unidades:** multi-seleção (OBRIGATÓRIO)
*	**Secções:** multi-seleção
*	**Colaboradores:** multi-seleção
*	**Estado:** multi-seleção
*	**Período:** mês (drop-down) e ano (drop-down)
*	**Somente colaboradores ativos:** check-box
*	**Ordenação:** radio button

<img width="1376" height="661" alt="image" src="https://github.com/user-attachments/assets/b39a2056-8eb3-474a-bcba-8f43db55c938" />

**Informação técnica**

- **Nome do relatório:** Estado da Gestão de Tempos
- **Key:** TimeManagementState
- **Função:** S_PCK_CORE_EXECUTION_REPORTS.Get_Time_Management_State
- **Local de impressão:** Módulo Relatórios
- **Formatos disponíveis:** Excel, PDF

---

## Estimativas

O relatório **Estimativas** é um mapa de análise que permite comparar previsões de vendas com os resultados efetivamente realizados. Este relatório é utilizado para avaliar a precisão das previsões, analisar o impacto de eventos e acompanhar desvios entre o planeado e o realizado.

Para cada dia do período selecionado, o relatório apresenta previsões baseadas no histórico, valores de forecast, estimativas ajustadas, percentagem de evento, forecast com evento aplicado e os valores reais de vendas, permitindo uma análise detalhada do desempenho.

No cabeçalho, o relatório apresenta a unidade, a secção e o período selecionados.

Os dados são apresentados em formato tabular e o relatório é composto por 10 colunas:

- **Dia da Semana**
- **Data**
- **Previsão segundo o realizado** -- (itens,valor)
- **Forecast** -- valor previsto
- **Estimativas** -- valor estimado
- **% Evento** -- percentagem associada a eventos
- **Vendas Realizadas** -- (itens,valor)
- **Desvio % Realizado / Forecast Evento**

<img width="1856" height="384" alt="image" src="https://github.com/user-attachments/assets/aec19f8e-4f9f-4de6-a9a6-0adeb05d8361" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidade (single)
- **i_fk_section** → secções (multi)
- **i_begin_date / i_end_date** → período

**Filtros do relatório**

*	**Unidades:** drop-down (OBRIGATÓRIO)
*	**Secções:** drop-down
*	**Período**
  
<img width="1374" height="661" alt="image" src="https://github.com/user-attachments/assets/b9b5ce95-e25a-4483-979a-037be6968d92" />

**Informação técnica**

- **Nome do relatório:** Estimativas
- **Key:** Estimates
- **Função:** S_PCK_CORE_REPORTS.GET_ESTIMATES
- **Local de impressão:** Módulo Relatórios
- **Formatos disponíveis:** Excel, PDF

---

## Folgas Compensatórias

O relatório **Folgas Compensatórias** permite acompanhar, por colaborador, o número de folgas compensatórias adquiridas, atribuídas e o respetivo saldo, ao longo de um determinado ano. Este relatório é essencial para o controlo de direitos compensatórios resultantes de trabalho suplementar ou outros mecanismos de compensação.

Para cada colaborador, o relatório apresenta o período de vigência das folgas compensatórias, quantificando as folgas adquiridas, as folgas já atribuídas e o saldo disponível.

No cabeçalho, o relatório apresenta a empresa/unidade, a secção e o período (ano) selecionados. A informação encontra-se organizada por secção.

Os dados são apresentados em formato tabular e o relatório é composto por 7 colunas:

- **Nº Mecanográfico** -- número identificativo do colaborador
- **Nome** -- nome do colaborador
- **Data Início** -- data inicial do período considerado
- **Data Fim** -- data final do período considerado
- **Folgas Adquiridas** -- total de folgas compensatórias adquiridas
- **Folgas Atribuídas** -- total de folgas compensatórias já utilizadas
- **Saldo** -- saldo atual de folgas compensatórias

<img width="1873" height="104" alt="image" src="https://github.com/user-attachments/assets/7a6a06f7-d989-45e7-8c69-57c49b554a6d" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi)
- **I_FK_SECTION** → secções (multi)
- **I_FK_EMPLOYEE** → colaboradores (multi)
- **I_YEAR** → ano

**Filtros do relatório**

* **Unidades:** multi-seleção (OBRIGATÓRIO)
* **Secções:** multi-seleção
* **Colaboradores:** multi-seleção
* **Período (ano):** drop-down

<img width="1372" height="657" alt="image" src="https://github.com/user-attachments/assets/5ae64737-e0b8-453f-8fde-4a6954e7f4bb" />

**Informação técnica**

- **Nome do relatório:** Folgas Compensatórias
- **Key:** CompensatoryDaysOff
- **Função:** S_PCK_CORE_EXECUTION_REPORTS.GET_COMPENSATORY_DAYSOFF
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Folgas e Ausências por Dia

O relatório **Folgas e Ausências por Dia** apresenta, para um dia específico, o número de folgas, feriados, férias, compensações e ausências registadas por colaborador. Este relatório permite uma visão diária consolidada da ocupação e das ausências, sendo útil para análise operacional e controlo diário.

Adicionalmente, o relatório apresenta contadores agregados por secção e por posto, identificados por códigos como FO, FC, FER, DBE, DBT, AR e ANR:

- FO- Folga
- FC- Folga Compensatória
- FER -- Férias
- DBE-
- DBT-
- AR- Ausência Regulamentada
- ANR- Ausência não regulamentada

No cabeçalho, o relatório apresenta a unidade e a data selecionada. A informação é organizada por secção e por posto.

Os dados são apresentados em formato tabular e o relatório é composto por 7 colunas:

- **Operário** -- número identificativo do colaborador
- **Nome** -- nome do colaborador
- **Folgas** -- tipo de folga (folga ou folga compensatória)
- **Feriados** -- número de feriados no dia
- **Férias** -- número de férias no dia
- **Compensações** -- número de compensações no dia
- **Ausências** -- número de ausências no dia

<img width="1847" height="363" alt="image" src="https://github.com/user-attachments/assets/0f5cd98a-277e-408c-89a6-f3436f6cd0f1" />

**Parâmetros do relatório (back-end)**

- **I_fk_unit** → unidades
- **I_fk_secao** → secções (multi)
- **I_fk_grupo** → colaboradores (multi)
- **I_data** → periodo

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções**: multi-seleção
* **Grupos:** multi-seleção
* **Parâmetros legais:** drop-down
* **Data**

<img width="1371" height="661" alt="image" src="https://github.com/user-attachments/assets/b548fa00-986a-4aab-b4bc-a092d1ac1f01" />

**Informação técnica**

- **Nome do relatório:** Folgas e Ausências por Dia
- **Local de impressão:** Módulo "Relatórios"
- **Key:** DaysOffAndAbsencesByDay 
- **Função:** S_PCK_CORE_REPORTS.GET_ABSENCES_TYPES_COLAB
- **Formatos disponíveis:** Excel, PDF

---

## Horários por Colaborador

O relatório **Horários por Colaborador** apresenta, de forma detalhada, os horários realizados por cada colaborador ao longo do período selecionado, organizados por semana. Permite ainda analisar a carga horária diária e semanal, bem como os contadores de ausências associados ao colaborador.

Para cada colaborador, o relatório apresenta uma grelha semanal, onde cada coluna corresponde a um dia da semana, indicando o horário praticado e a carga horária realizada.

No cabeçalho, o relatório apresenta o nome do colaborador, o período selecionado e a carga semanal contratual. A informação encontra-se organizada por colaborador.

Os dados são apresentados em formato tabular e o relatório é composto por 9 colunas:

- **Semana** -- primeiro dia da semana apresentada
- **Dia 1 a Dia 7** -- horário e carga horária realizada em cada dia da semana
- **Carga Semanal** -- total de horas realizadas na semana

<img width="1861" height="368" alt="image" src="https://github.com/user-attachments/assets/21f7a57a-3523-4b9e-86c7-418905e54b87" />

**Parâmetros do relatório (back-end)**

- **i_data_Ini / i_data_Fim** → período
- **i_fk_unidade** → unidades
- **i_fk_secao** → secções
- **i_fk_colaborador** → colaboradores
- **i_idioma** → idioma

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Período**
* **Planeamento Extra:** check-box
* **Opções de impressão (por escala / sem quebra / automático):** radio button

<img width="1373" height="659" alt="image" src="https://github.com/user-attachments/assets/a6833375-7b09-4add-8ac0-50b16aee34ec" />

**Informação técnica**

- **Nome do relatório:** Horários por Colaborador
- **Key:** PersonalSchedule
- **Função:** S_RELATORIOS.get_horario_individual
- **Local de impressão:** Módulo "Relatórios / Vista mensal de horários / Escala"
- **Formatos disponíveis:** Excel, PDF

---

## Horários por Colaborador (Avaliação Noturna)

O relatório **Horários por Colaborador (Avaliação Noturna)** é equivalente ao relatório de Horários por Colaborador, aplicando adicionalmente as regras de redução de horário noturno, quando aplicável. 

As configurações do horário noturno (hora inicio, hora fim e período) podem ser definidas no ecrã “Trabalho noturno” que pode ser acedido através de Parâmetros> Unidades> Colaborador> Gestão de Tempos> Trabalho noturno.

Este relatório é fundamental para a correta análise de cargas horárias sujeitas a regimes noturnos.

A estrutura de apresentação é idêntica ao relatório base, sendo ajustados os cálculos de carga horária conforme as regras de avaliação noturna.

<img width="1853" height="366" alt="image" src="https://github.com/user-attachments/assets/dcfbe4b9-b1e4-4861-8db1-6f198a24cd32" />

**Parâmetros do relatório (back-end)**

- **i_data_Ini / i_data_Fim** → período
- **i_fk_unidade** → unidades
- **i_fk_secao** → secções
- **i_fk_colaborador** → colaboradores
- **i_idioma** → idioma

**Filtros do relatório**

* **Unidades:** drop-down (**OBRIGATÓRIO**)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Período**
* **Planeamento Extra:** check-box
* **Opções de impressão:** radio button

<img width="1373" height="656" alt="image" src="https://github.com/user-attachments/assets/35fc516d-9dee-46cb-87f2-7dc1fa3c348b" />

**Informação técnica**

- **Nome do relatório:** Horários por Colaborador (Avaliação Noturna)
- **Key:** PersonalScheduleNightEvaluation
- **Função:** S_RELATORIOS.get_horario_individual
- **Local de impressão:** Módulo "Relatórios", Vista mensal de horários, Escala
- **Formatos disponíveis:** Excel, PDF

---

## Incumprimentos Legais

O relatório **Incumprimentos Legais** apresenta uma listagem de todos os colaboradores que registam situações de incumprimento face às obrigações legais definidas, no período selecionado.

Este relatório permite identificar quais os parâmetros legais que não foram cumpridos, o valor legal estipulado e a duração do incumprimento.

**Parâmetros legais:** 

- **Dias de trabalho consecutivos** - Refere-se à violação das normas legais que estabelecem o número máximo de dias seguidos que um trabalhador pode laborar sem descanso semanal obrigatório. São vários dias seguidos em que um trabalhador exerce atividade profissional sem interrupção por um dia de descanso. A lei estabelece que o trabalhador deve ter pelo menos um dia de descanso por semana, que pode variar. 

-	**Horas de trabalho consecutivas** - Refere-se à violação das regras legais que limitam o número de horas que um trabalhador pode exercer a sua atividade de forma contínua, sem pausas ou intervalos obrigatórios. São horas trabalhadas seguidas, sem interrupção para descanso ou refeição. A lei define um limite máximo de horas consecutivas que uma pessoa pode trabalhar, e também obriga a pausas (intervalos) após esse limite.
  
-	**Período de descanso entre turnos** - Refere-se à violação das normas legais que estabelecem o intervalo mínimo obrigatório de descanso entre dois turnos de trabalho consecutivos de um trabalhador. É o tempo mínimo de descanso que um trabalhador deve ter entre o fim de uma jornada de trabalho e o início da próxima).
  
-	**Número de dias não trabalhados** - Horário de trabalho planeado/dias com horários e sem picagens, anteriores ou iguais a hoje.

Para cada ocorrência, o relatório indica o período exato do incumprimento, o valor aplicado e se o colaborador possui isenção de horário de trabalho (IHT).

No cabeçalho, o relatório apresenta a loja/unidade, o período e a secção selecionados. A informação encontra-se organizada por secção.

Os dados são apresentados em formato tabular e o relatório é composto por 8 colunas:

- **Nº Mecanográfico** -- número identificativo do colaborador
- **Colaborador** -- nome do colaborador
- **Parâmetro Legal** -- parâmetro legal não cumprido
- **Valor Legal** -- valor estipulado para o parâmetro
- **Data Início** -- início do incumprimento
- **Data Fim** -- fim do incumprimento
- **Valor Aplicado** -- valor efetivamente aplicado
- **IHT** -- indicação de isenção de horário de trabalho (S/N)

<img width="1860" height="504" alt="image" src="https://github.com/user-attachments/assets/07dd665e-90e8-43d7-8e12-b726b8477876" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (single)
- **I_FK_SECTION** → secções
- **I_FK_EMPLOYEE** → colaboradores
- **I_BEGIN_DATE / I_END_DATE** → período
- **i_legal_params** → parâmetros legais

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Parâmetros legais:** drop-down
* **Período**
* **Ordenação:** radio button

<img width="1373" height="657" alt="image" src="https://github.com/user-attachments/assets/76e5c2e3-03cc-448a-a7da-ff0c23ce16b3" />

**Informação técnica**

- **Nome do relatório:** Incumprimentos Legais
- **Key:** LegalDefaults
- **Função:** S_PCK_CORE_EXECUTION_REPORTS.Get_legal_defaults
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Mapa Anual de Férias

O relatório **Mapa Anual de Férias** apresenta, de forma visual e detalhada, o planeamento anual de férias de cada colaborador. Permite analisar, ao longo de todo o ano, os dias de férias marcados, os dias deduzidos ao contingente e a sua distribuição mensal.

O relatório tem um formato de **calendário tabular**, onde cada linha corresponde a um mês e cada coluna representa os dias dos meses do ano. As férias e feriados encontram-se assinalados através de cores, facilitando a leitura e análise global do planeamento.

No cabeçalho, o relatório apresenta a **unidade**, a **secção** e o **ano selecionado**. A informação encontra-se organizada por colaborador, sendo apresentada uma tabela individual por cada um.

Adicionalmente, o relatório inclui:

- Uma coluna com o **total de dias de férias marcados por mês**
- Uma coluna com o **total de dias de férias deduzidos por mês**
- Na última linha, o **total anual** de dias marcados e deduzidos

<img width="1855" height="673" alt="image" src="https://github.com/user-attachments/assets/896b7984-45cd-49d3-b7ce-0903f1834ae2" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidade (single)
- **i_fk_section** → secções (multi)
- **i_fk_employee** → colaboradores (multi)
- **i_year** → ano

**Filtros do relatório**

* **Unidade:** drop-down (OBRIGATÓRIO)
* **Secções:** multi-seleção
* **Colaboradores:** multi-seleção
* **Ano:** drop-down
* **Ordenação:** radio button
  
<img width="1375" height="661" alt="image" src="https://github.com/user-attachments/assets/5edbb3ef-0ef7-4807-8d25-851576cdda78" />

**Informação técnica**

- **Nome do relatório:** Mapa Anual de Férias
- **Key:** AnnualVacationMap
- **Função:** S_PCK_CORE_REPORTS.GET_ANUAL_VACATIONS
- **Local:** Módulo "Relatórios"
- **Formatos:** Excel, PDF

---

## Mapa de Descansos Anual

O relatório **Mapa de Descansos Anual** apresenta, para um determinado ano, o registo diário de descansos e ausências dos colaboradores, permitindo uma visão consolidada dos diferentes motivos de ausência ocorridos nesse período.

No cabeçalho, o relatório apresenta a **unidade**, a **secção**, o **colaborador** e o **ano**. As primeiras linhas da tabela identificam os **dias do mês**, servindo de referência temporal.

Para cada colaborador, o relatório mostra os dias em que ocorreram:

- folgas
- feriados
- férias
- outras ausências, conforme o tipo de informação selecionada.

É apresentado, ainda, o total de ausências, de cada tipo ocorridas, por mês e por colaborador, através de contadores.

A informação é apresentada num formato semelhante a um calendário, facilitando a leitura e análise operacional.

<img width="1852" height="731" alt="image" src="https://github.com/user-attachments/assets/a68236f1-b11e-429f-97cf-9cbb9a36e74c" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidade (single)
- **i_fk_section** → secção (single)
- **i_fk_group** → grupos
- **i_fk_colab** → colaboradores
- **i_month** → mês
- **i_year** → ano
- **i_data_type** → tipo de dados

**Filtros do relatório**

* **Unidade:** drop-down (OBRIGATÓRIO)
* **Secção:** drop-down (OBRIGATÓRIO)
* **Grupos:** drop-down
* **Colaboradores:** drop-down
* **Ano:** drop-down
* **Informação a imprimir:**
  * Mapa completo
  * Domingos e feriados livres

<img width="1374" height="659" alt="image" src="https://github.com/user-attachments/assets/5ab5f277-5b85-4767-bd7c-49c27224fe61" />

**Informação técnica**

- **Nome do relatório:** Mapa de Descansos
- **Key** RestMap
- **Função:** S_PCK_CORE_REPORTS.GET_REST_MAP
- **Local:** Módulo "Relatórios" e vista "Mapa de Descansos"
- **Formatos:** Excel, PDF

---

## Mapa de Descansos (Mensal)

O relatório **Mapa de Descansos Mensal** apresenta, para um determinado mês, o registo diário de descansos e ausências dos colaboradores, permitindo uma visão consolidada dos diferentes motivos de ausência ocorridos nesse período.

No cabeçalho, o relatório apresenta a **unidade**, a **secção** e o **mês selecionado**. As primeiras linhas da tabela identificam os **dias da semana** e os **dias do mês**, servindo de referência temporal.

Para cada colaborador, o relatório mostra os dias em que ocorreram:

- folgas
- feriados
- férias
- outras ausências, conforme o tipo de informação selecionada.

É apresentado, ainda, o total de ausências, de cada tipo ocorridas, por mês e por colaborador, através de contadores.

A informação é apresentada num formato semelhante a um calendário mensal, facilitando a leitura e análise operacional.

<img width="1874" height="217" alt="image" src="https://github.com/user-attachments/assets/35a0d610-3b4d-4fef-9f0d-0748b39730b4" />

**Parâmetros do relatório (back-end)**

- **i_year** → ano
- **i_month** → mês

**Filtros do relatório**

* **Unidade:** drop-down (OBRIGATÓRIO)
* **Secção:** drop-down (OBRIGATÓRIO)
* **Grupos:** drop-down
* **Colaboradores:** drop-down
* **Ano:** drop-down
* **Informação a imprimir:**
  * Mapa completo
  * Domingos e feriados livres

<img width="1140" height="580" alt="image" src="https://github.com/user-attachments/assets/d70e66c4-6771-43c4-84af-a69fbe0012d8" />

**Informação técnica**

- **Nome do relatório:** Mapa de Descansos
- **Key** RestMap
- **Função:** S_PCK_CORE_REPORTS.GET_REST_MAP
- **Local:** Módulo "Relatórios" e vista "Mapa de Descansos"
- **Formatos:** Excel, PDF

---

## Movimentos por Contingente

O relatório **Movimentos por Contingente** apresenta os movimentos de contingentes efetuados no período selecionado, permitindo analisar deduções e compensações realizadas aos colaboradores.

No cabeçalho, o relatório apresenta a **unidade**, a **secção** e o **período selecionado**. A informação encontra-se organizada por secção, sendo apresentada uma tabela distinta para cada uma.

Para cada movimento registado, o relatório identifica:

- o colaborador,
- a data do movimento,
- o contingente movimentado,
- o tipo de movimento (dedução ou compensação),
- o valor movimentado e a respetiva unidade de medida (dias ou horas).

**Colunas do relatório**

**1.** Nº Mecanográfico

**2.** Colaborador

**3.** Data

**4.** Código do contingente

**5.** Contingente

**6.** Tipo (Compensação / Dedução)

**7.** Valor

**8.** Unidade de Medida

<img width="1873" height="573" alt="image" src="https://github.com/user-attachments/assets/a3607926-821d-4824-92bd-55f3ce933eb6" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit, i_fk_section, i_fk_employee**
- **i_is_active** → só ativos (flag)
- **i_contingent** → contingente
- **i_begin_date / i_end_date**
- **i_mov_type** → tipo de movimento
- **i_has_timemanagement **→ flag GT

**Filtros do relatório**

* **Unidades:** multi-seleção (OBRIGATÓRIO)
* **Secção:** multi-seleção
* **Colaboradores:** multi-seleção
* **Parametros legais:** drop-down
* **Período**
* **Contingente:** drop-down
* **Tipo de movimento (todos,compensação,dedução):** drop-down
* **Colaboradores:** radio button

<img width="1379" height="659" alt="image" src="https://github.com/user-attachments/assets/1643ce29-f571-4976-8150-85ea974672f5" />

**Informação técnica**

- **Nome do relatório:** Movimentos por Contingente
- **Key:** ContingentMovements
- **Função:** S_PCK_CORE_REPORTS.GET_CONTINGENT_MOVS
- **Local de impressão:** Módulo "Relatórios"
- **Formatos:** Excel, PDF

---

## Pagamento de Variáveis

O relatório **Pagamento de Variáveis** é um mapa de controlo e cálculo de variáveis salariais, utilizado para apurar pagamentos adicionais relacionados com horas extra, trabalho noturno, trabalho em feriados e domingos, subsídio de alimentação e horas registadas em picagens.

O relatório permite analisar indicadores de assiduidade, presença e carga horária, sendo fundamental para o processamento salarial.

No cabeçalho, o relatório apresenta a **empresa**, a **secção** e o **período analisado**. A informação encontra-se organizada por secção.

Os dados são apresentados em formato tabular e o relatório é composto por 16 colunas:

- **Nº Mecanográfico** -- número interno do colaborador
- **Nome** -- nome completo
- **Categoria** -- função (ex.: Operador Loja, Coordenador Secção)
- **Período de Datas** -- intervalo de dias analisado para esse colaborador
- **Dias de trabalho e assiduidade**
- **Dias Úteis** -- número de dias úteis no período
- **Dias com Picagens** -- dias em que houve registo de ponto
- **Dias s/ Picagem ou Ausência** -- dias sem registo (faltas, férias, ausências)
- **Dias com Ausências** -- ausências justificadas/registadas
- **Trab. Noturnos** -- horas trabalhadas em período noturno
- **Feriados** -- número de feriados no período
- **Trab. Feriados** -- horas trabalhadas em feriados
- **Domingos** -- número de domingos no período
- **Domingos c/ Picagens** -- domingos efetivamente trabalhados
- **Horas de Domingos** -- horas trabalhadas ao domingo
- **Sub. Alimentação** -- total de horas/dias que dão direito ao subsídio de alimentação
- **Horas Picagens** -- total de horas registadas no ponto

<img width="1868" height="226" alt="image" src="https://github.com/user-attachments/assets/cddb29ca-704d-421f-9691-47318fd141b4" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidade
- **i_fk_section** → secções
- **i_fk_employee** → colaboradores
- **i_begin_date / i_end_date** → período
- **i_collaborator_status** → estado do colaborador

**Filtros do relatório**

* **Unidade:** drop-down (OBRIGATÓRIO)
* **Secção:** drop-down
* **Colaboradores:** drop-down
* **Colaboradores (Todos / Ativos / Inativos):** radio button
* **Período**
  
<img width="1373" height="659" alt="image" src="https://github.com/user-attachments/assets/ad010747-b9f7-4c20-8c75-9ca24cf55f2f" />

**Informação técnica**

- **Nome do relatório:** Pagamento de Variáveis
- **Key:** VariablesPayment
- **Função:** S_PCK_CORE_EXECUTION_REPORTS.Get_Variables_Payments
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Pedidos de Alteração de Picagem

O relatório **Pedidos de Alteração de Picagens** apresenta todos os pedidos de alteração de registos de picagem efetuados pelos colaboradores, permitindo controlar as alterações solicitadas, o estado de aprovação e o respetivo histórico de validação.

Para cada pedido, o relatório identifica a picagem original, a nova picagem proposta, bem como a informação associada ao pedido, incluindo o utilizador que o submeteu e o estado do processo.

O relatório apresenta a unidade e a secção selecionadas. A informação encontra-se organizada em formato tabular, sendo cada linha correspondente a um pedido de alteração de picagem.

Os dados são apresentados em formato tabular e o relatório é composto pelas seguintes colunas:

-	**Unidade** – unidade onde o colaborador se encontra afeto
-	**Secção** – secção ou área funcional do colaborador
-	**Nº Mecanográfico** – número interno de identificação do colaborador
-	**Nome** – nome do colaborador
-	**Dia** – data a que corresponde o registo de picagem
-	**Picagem Original** – registo inicial da picagem efetuada
-	**Picagem** – novo registo de picagem solicitado
-	**Data Pedido** – data e hora em que o pedido foi submetido
-	**Utilizador** – utilizador que efetuou o pedido
-	**Estado** – estado do pedido (ex.: Aprovado, Pendente)
-	**Data de Revisão** – data e hora em que o pedido foi analisado
-	**Aprovador** – utilizador responsável pela validação do pedido
-	**Nº Impresso** – número identificativo do pedido ou registo gerado pelo sistema

<img width="1552" height="84" alt="image" src="https://github.com/user-attachments/assets/e46195c0-eaad-40f5-88da-2bab4f1881e6" />

**Parâmetros do relatório (back-end)**

-	**i_fk_unit** → unidade
-	**i_fk_section** → secções
-	**i_fk_employee** → colaboradores
-	**i_begin_date / i_end_date** → período
-	**i_collaborator_status** → estado do colaborador

**Filtros do relatório**

-	**Unidade:** drop-down (OBRIGATÓRIO)
-	**Secção:** drop-down
-	**Colaboradores:** drop-down
-	**Estado:** drop-down
-	**Período**

<img width="1362" height="650" alt="image" src="https://github.com/user-attachments/assets/f3cb6ded-e528-4495-ba91-f6ea30cf99d3" />

**Informação técnica**

-	**Nome do relatório:** Pedidos de Alteração de Picagens
-	**Key:** PunchEdition
-	**Função:** BFF
-	**Local de impressão:** Módulo “Relatórios”
-	**Formatos disponíveis:** Excel

---

## Perfis de Acesso

O relatório **Perfis de Acesso** apresenta os perfis atribuídos a cada utilizador, bem como as unidades e secções onde possuem permissões de acesso. Este relatório permite garantir controlo, auditoria e rastreabilidade dos acessos ao sistema.

No cabeçalho, o relatório apresenta a unidade, secção, colaborador e perfil de acesso selecionados, bem como a data de extração do relatório e a indicação se apenas colaboradores ativos foram considerados.

A informação pode ser apresentada por colaborador ou por unidade, conforme a vista selecionada.

Os dados são apresentados em formato tabular e o relatório é composto por 7 colunas:

- Colaborador
- Utilizador
- Unidade (Colaborador)
- Perfil de acesso
- Unidade (Secção)
- Secção
- Criação de acesso
  
<img width="1853" height="758" alt="image" src="https://github.com/user-attachments/assets/c4bcbdd9-ff1e-4185-920d-a3120884c7c5" />

**Parâmetros do relatório (back-end)**

- **i_view_type** → tipo de vista
- **i_only_active** → só ativos
- **i_fk_unit** → unidades
- **i_fk_section** → secções
- **i_fk_profile** → perfis
- **i_fk_employee** → colaboradores

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Perfis de acesso:** drop-down
* **Somente utilizadores ativos:** check-box
* **Ordenação:** radio button

<img width="1377" height="661" alt="image" src="https://github.com/user-attachments/assets/532540b7-59ca-45a1-a7f9-f71fc9002edc" />

**Informação técnica**

- **Nome do relatório:** Perfis de Acesso
- **Key:** AssignedSections
- **Função:** S_PCK_CORE_REPORTS.GET_SECTION_PERMISSIONS
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Petição de Férias

**Petição de Férias** é um documento de pedido de férias, utilizado para registar, solicitar e autorizar os períodos de férias de um colaborador num determinado ano.

Serve como controlo administrativo entre o colaborador, a chefia direta e os Recursos Humanos, garantindo que as férias são marcadas de acordo com o direito legal e com validação hierárquica.

O cabeçalho do documento identifica o Pedido de Férias, indicando o ano de referência (2024) e a empresa, enquadrando o pedido no tempo e na entidade correta.

De seguida, surge a identificação do colaborador:

-	Nome completo
-	Número mecanográfico
-	Secção onde exerce funções
-	Tipo de contrato/horário

O documento apresenta ainda o direito a férias, indicando o número total de dias a que o colaborador tem direito no ano e, caso existam, as férias adicionais, servindo para controlar o saldo disponível. 

Na área dos períodos de férias são registadas as datas de início e fim de cada período e o respetivo número de dias, sendo apresentado no final o total de dias já marcados, o que permite verificar os dias utilizados e os que ainda disponíveis. 

O pedido só se torna válido após a assinatura do colaborador e do superior hierárquico, com indicação das respetivas datas. 

Existe também uma secção destinada a alterações, onde podem ser registadas mudanças posteriores aos períodos aprovados, com indicação do novo período, número de dias e autorização hierárquica, garantindo o histórico do pedido. 

Por fim, o documento inclui notas finais com orientações sobre a utilização e alteração das férias, a prioridade entre férias do ano e férias adicionais, bem como a data de impressão do documento.

<img width="886" height="974" alt="image" src="https://github.com/user-attachments/assets/81102140-bcc4-4b53-b0ea-4ab6fb3ad6e8" />

**Parâmetros do relatório (back-end)**

-	**I_FK_UNIT** → unidade
-	**I_FK_SECTION** → secções
-	**I_FK_EMPLOYEE** → colaboradores
-	**I_BEGIN_DATE** / I_END_DATE → período

**Filtros do relatório**

-	**Unidades:** drop-down (OBRIGATÓRIO)
-	**Secções:** drop-down
-	**Colaboradores:** drop-down
-	**Período (ano):** drop-down

<img width="1372" height="652" alt="image" src="https://github.com/user-attachments/assets/dbdcba21-3897-4851-922e-cc641851cff5" />

**Informação técnica**

-	**Nome do relatório:** Petição de Férias
-	**Key:** Punch
-	**Função:** S_PCK_CORE_EXECUTION_REPORTS.Get_picagens
-	**Local de impressão:** Módulo “Relatórios”
-	**Formatos disponíveis:** Excel, PDF

---

## Picagens

O relatório **Picagens** apresenta o registo detalhado das picagens (registos de ponto) efetuadas pelos colaboradores no período selecionado. Este relatório é fundamental para o controlo da assiduidade, validação da presença diária, identificação de faltas, registos manuais e alterações efetuadas no sistema, servindo igualmente de base ao cálculo de variáveis salariais e à validação da carga horária contratual.

Para cada colaborador e para cada dia do período analisado, o relatório mostra o estado da picagem, os horários de entrada e saída, o terminal onde a picagem foi efetuada, bem como informação sobre registos manuais, anulações e utilizadores que efetuaram alterações.

No cabeçalho, o relatório apresenta a empresa, o departamento/secção, o período analisado, o nome do colaborador, a matrícula, o número do cartão de picagem, a carga horária semanal contratual, a vigência do cartão e a vigência do contrato.
A informação é apresentada em formato tabular, com detalhe diário por colaborador.

Os dados são apresentados em formato tabular e o relatório é composto pelas seguintes colunas principais:

- **Nome** -- identificação do colaborador
- **Matrícula** -- número interno do colaborador
- **Nº Cartão** -- cartão associado ao sistema de ponto
- **Carga Semanal** -- número de horas semanais contratadas
- **Data** -- dia específico do registo
- **Dia da Semana** -- identificação do dia (ex.: 2ª, 3ª, Sáb., Dom.)
- **Picagem** -- estado do dia (ex.: colaborador trabalhou, colaborador não trabalhou, ausência)
- **Tipo de Picagem** -- Entrada 1, Saída 2, Entrada 3, Saída 4
- **Terminal do Relógio** -- equipamento onde a picagem foi efetuada
- **Picagem Manual** -- indicação se o registo foi inserido manualmente
- **Anulação** -- indica se houve anulação de alguma picagem
- **User** -- utilizador que efetuou alterações
- **Data de Modificação** -- data da última alteração efetuada

<img width="1849" height="568" alt="image" src="https://github.com/user-attachments/assets/3ac14511-59fc-470a-8c17-bb7051aeb98c" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (single)
- **I_FK_SECTION** → secções (multi)
- **I_FK_EMPLOYEE** → colaboradores (multi)
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

* **Unidades**: drop-down (OBRIGATÓRIO)
* **Secções**: drop-down
* **Colaboradores**: drop-down
* **Período**

<img width="1370" height="655" alt="image" src="https://github.com/user-attachments/assets/f8a639a0-fc5d-4218-8e9d-6066b8d5ce14" />

**Informação técnica**

- **Nome do relatório**: Picagens
- **Key**: Punch
- **Função**: S_PCK_CORE_EXECUTION_REPORTS. Get_picagens
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Picagens de Intervalos

O relatório **Picagens de Intervalos** apresenta o controlo detalhado dos períodos de pausa realizados pelos colaboradores, permitindo verificar as horas de entrada e saída dos intervalos, bem como a duração total das pausas efetuadas. Este relatório é utilizado para o controlo da assiduidade, cumprimento dos horários e validação dos intervalos legais de trabalho.

Para cada colaborador e para cada dia do período selecionado, o relatório indica o intervalo realizado, os horários registados e o tempo total de pausa, bem como os terminais onde foram efetuadas as picagens.

No cabeçalho, o relatório apresenta a loja, o período e a secção.
A informação encontra-se organizada por secção, com tabelas separadas.

Os dados são apresentados em formato tabular e o relatório é composto por 10 colunas:

- **Nº Mecanográfico** -- número mecanográfico do colaborador
- **Cartão** -- número do cartão de ponto
- **Colaborador** -- nome do colaborador
- **Data** -- dia em que o intervalo foi registado
- **Dia da Semana** -- dia da semana correspondente
- **Picagem de Entrada** -- hora de início do intervalo
- **Picagem de Saída** -- hora de fim do intervalo
- **Tempo Total (em minutos)** -- duração total do intervalo
- **Terminal 1 / Terminal 2** -- identificação dos terminais utilizados
- **IHT** -- isenção de horário de trabalho (S/N)

<img width="1870" height="133" alt="image" src="https://github.com/user-attachments/assets/549e6401-b059-456b-8ede-28d99bb06d69" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (single)
- **I_FK_SECTION** → secções (multi)
- **I_FK_EMPLOYEE** → colaboradores (multi)
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

* **Unidades**: drop-down (OBRIGATÓRIO)
* **Secções**: drop-down
* **Colaboradores**: drop-down
* **Parâmetros legais**: drop-down
* **Período**
* **Tempo total (minutos)**: menor/igual/maior que (radio-button)
* **Ordenação**: radio button

<img width="1376" height="659" alt="image" src="https://github.com/user-attachments/assets/395c2553-20c8-4672-8483-e8f76605a50c" />

**Informação técnica**

- **Nome do relatório**: Picagens de Intervalos
- **Key**: BreakPunchs
- **Função**: S_PCK_CORE_EXECUTION_REPORTS. Get_f05_breaks
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Picagens Entidade Oficiais

O relatório **Picagens Entidades Oficiais** é um mapa de controlo de picagens utilizado para comprovar a situação diária do colaborador perante entidades externas. Este relatório permite demonstrar, de forma oficial, os dias trabalhados ou não trabalhados num determinado período, com base nos registos do sistema de ponto.

Para cada colaborador, o relatório apresenta uma listagem simples dos dias do período analisado, indicando se houve ou não trabalho nesse dia.

No cabeçalho, o relatório apresenta a empresa, o departamento/secção, o nome e matrícula do colaborador, o número e vigência do cartão, a carga semanal e a vigência do contrato.
A informação é apresentada por colaborador, em tabelas separadas.

Os dados são apresentados em formato tabular e o relatório é composto por 3 colunas:

- **Data** -- data da picagem
- **Dia da Semana** -- dia da semana correspondente
- **Picagem** -- indicação do estado (ex.: "Colab. Não Trab.")

<img width="1856" height="573" alt="image" src="https://github.com/user-attachments/assets/fa883772-816f-44bc-b0ee-c3386ab054f5" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (single)
- **I_FK_SECTION** → secções
- **I_FK_EMPLOYEE** → colaboradores
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

* **Unidades**: drop-down (OBRIGATÓRIO)
* **Secções**: drop-down
* **Colaboradores**: drop-down
* **Período**

<img width="1376" height="663" alt="image" src="https://github.com/user-attachments/assets/507adc65-0816-41f5-a016-6058f3ad8860" />

**Informação técnica**

- **Nome do relatório**: Picagens Entidades Oficiais
- **Key**: OfficialEntityPunch
- **Função**: S_PCK_CORE_EXECUTION_REPORTS. Get_pic_entidade_oficial
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Plano Diário por Posto

O relatório **Plano Diário por Posto** apresenta a afetação diária dos colaboradores por posto de trabalho, permitindo visualizar a distribuição dos recursos humanos ao longo do dia, por secção e por função. Este relatório é essencial para analisar a cobertura operacional e a ocupação dos postos em intervalos horários definidos.

Para cada secção, o relatório mostra os colaboradores escalados e a respetiva ocupação ao longo do dia, normalmente em intervalos de 15 minutos, permitindo identificar períodos de maior ou menor cobertura.

No cabeçalho, o relatório apresenta a data, a unidade, a secção e o período analisado.
A informação encontra-se organizada por secção.

Os dados são apresentados em formato tabular, onde:

- **Nome** -- identifica o colaborador
- **Tipo de Posto** -- posto ou função atribuída
- **Intervalos horários** -- colunas sequenciais ao longo do dia

Em cada célula:

- **1** indica que o colaborador está escalado nesse período
- **0** indica ausência ou não afetação
- **F** indica folga

No final de cada secção existe uma linha de **TOTAL**, que soma o número de colaboradores presentes em cada intervalo horário.

<img width="1854" height="475" alt="image" src="https://github.com/user-attachments/assets/aa679db1-380c-4e7c-b1f7-6e64bd18399e" />


**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (single)
- **I_FK_SECTION** → secções (multi)
- **I_FK_WORKSTATION_TYPE** → tipos de posto (multi)
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

* **Unidades**: drop-down (OBRIGATÓRIO)
* **Secções**: multi-seleção
* **Tipo de posto**: multi-seleção
* **Período**
  
<img width="1376" height="665" alt="image" src="https://github.com/user-attachments/assets/801d042a-0e62-4e55-87be-5c8e2821952a" />

**Informação técnica**

- **Nome do relatório**: Plano Diário por Posto
- **Key**: DailyPlanPerStation
- **Função**: S_PCK_CORE_REPORTS.DAILY_PLAN_PER_STATION
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Polivalências por Colaborador

O relatório **Polivalências por Colaborador** apresenta as diferentes secções e postos onde cada colaborador está habilitado a desempenhar funções, bem como a prioridade atribuída a cada polivalência. Este relatório é utilizado para apoiar o planeamento operacional e a gestão da flexibilidade da equipa.

Para cada secção, o relatório lista os colaboradores associados e as respetivas polivalências, podendo o mesmo colaborador surgir em várias linhas caso esteja habilitado a desempenhar funções em diferentes secções ou postos.

No cabeçalho, o relatório apresenta a unidade e a secção.
A informação encontra-se organizada por secção.

Os dados são apresentados em formato tabular e o relatório é composto por 5 colunas:

- **Nº Matrícula** -- número interno de identificação do colaborador
- **Colaborador** -- nome do colaborador
- **Prioridade** -- nível de prioridade atribuído à função ou posto (quanto menor o número, maior a prioridade)
- **Secção** -- secção onde o colaborador pode exercer funções
- **Posto** -- posto ou função específica associada à secção

<img width="1866" height="865" alt="image" src="https://github.com/user-attachments/assets/41a87b68-dffe-4ea3-877e-b0e9e33ccd22" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi)
- **I_FK_SECTION** → secções (multi)
- **I_FK_EMPLOYEE** → colaboradores (multi)

**Filtros do relatório**

* **Unidades**: multi-seleção (OBRIGATÓRIO)
* **Secções**: multi-seleção
* **Colaboradores**: multi-seleção

<img width="1376" height="663" alt="image" src="https://github.com/user-attachments/assets/4a2651ed-e6e0-4a9a-9b52-2cd6e42c2872" />

**Informação técnica**

- **Nome do relatório**: Polivalências por Colaborador
- **Key**: EmployeePolyvalences
- **Função**: S_PCK_CORE_REPORTS.GET_POLI_PER_COLABORATOR
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Quadro Pessoal

O relatório **Quadro Pessoal** apresenta um mapa do quadro de pessoal da unidade selecionada, permitindo identificar e controlar os colaboradores existentes por secção, bem como as respetivas cargas horárias e datas contratuais.
Este relatório é fundamental para análises de dotação de pessoal, controlo de cargas horárias e acompanhamento da situação contratual dos colaboradores.

No cabeçalho, o relatório indica se estão a ser considerados apenas colaboradores ativos ou todos, bem como a secção a que o mapa se refere. O relatório pode ser emitido para várias secções da mesma unidade, sendo apresentada uma tabela distinta para cada secção.

Os dados são apresentados em formato tabular e o relatório é composto por 6 colunas:

- **Nº Mecan.** -- número mecanográfico do colaborador
- **Colaborador** -- nome completo do colaborador
- **Carga Semanal (SAP)** -- carga horária semanal registada no sistema SAP
- **Carga Semanal (WFM)** -- carga horária semanal definida no WFM
- **Data de Admissão** -- data de entrada do colaborador na empresa
- **Data de Demissão** -- data de saída do colaborador, quando aplicável

No final de cada secção é apresentado um resumo da carga horária semanal, onde constam:

- As diferentes cargas horárias existentes (ex.: 20h, 30h, 35h, 40h)
- O total de colaboradores associados a cada carga horária

<img width="1865" height="902" alt="image" src="https://github.com/user-attachments/assets/6d82f41f-399c-4176-b0e7-ced40298fe90" />

**Parâmetros do relatório (back-end)**

- **i_only_active** → só ativos / todos
- **i_fk_unit** → unidade (single)
- **i_fk_section** → secções (multi)
- **i_fk_employee** → colaboradores (multi)

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Somente colaboradores ativos:** check-box
* **Ordenação:** radio button

<img width="1384" height="672" alt="image" src="https://github.com/user-attachments/assets/b873794b-dd59-46b7-8804-309b8a01d55b" />

**Informação técnica**

- **Nome do relatório:** Quadro Pessoal
- **Key:** StaffingTable
- **Função:** S_PCK_CORE_REPORTS.GET_ALL_WORKERS
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Registo de Eventos

O relatório **Registo de Eventos** é um mapa de registo e controlo de eventos, utilizado para documentar eventos específicos com impacto na gestão operacional, horária ou remuneratória, ocorridos num determinado período. Permite analisar ajustes aplicados, o seu enquadramento e a unidade ou secção abrangida.

No cabeçalho, o relatório apresenta o tipo de registo (Sistema, Unidade ou Secção), o período analisado e a data de extração do relatório.

Os dados são apresentados em formato tabular, sendo cada linha correspondente a um evento registado. O relatório é composto por 11 colunas:

- **Evento** -- código identificativo do evento
- **Data Inicial** -- data de início do evento
- **Data Final** -- data de fim do evento
- **Hora Inicial** -- hora de início do evento
- **Hora Final** -- hora de fim do evento
- **Ajuste** -- valor do ajuste aplicado (ex.: percentagem ou acréscimo)
- **Tipo Alteração** -- natureza do ajuste efetuado (ex.: Percentual)
- **Base Cálculo** -- base utilizada para aplicação do evento (ex.: itens previstos)
- **Tipo Evento** -- nível ou âmbito do evento (ex.: Unidade)
- **Unidade** -- unidade a que o evento se aplica
- **Secção** -- secção específica abrangida

<img width="1871" height="142" alt="image" src="https://github.com/user-attachments/assets/a8aadc09-7568-4cb7-b710-f2c1c731a73b" />

**Parâmetros do relatório (back-end)**

- **i_idioma** → idioma
- **i_fk_unit** → unidade (single)
- **i_fk_section** → secções (multi)
- **i_type** → tipos de evento (multi)
- **i_begin_date / i_end_date** → período

**Filtros do relatório**

* **Tipo:** drop-down (OBRIGATÓRIO)
* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Período**
* **Ordenação:** radio button

<img width="1721" height="627" alt="image" src="https://github.com/user-attachments/assets/83515a5f-c61c-44d3-a737-61d3f5a8aff7" />

**Informação técnica**

- **Nome do relatório:** Registo de Eventos
- **Key:** Events
- **Função:** S_PCK_CORE_REPORTS.GET_EVENT_REG
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Relatório Anual de Férias

O **Relatório Anual de Férias** é um mapa anual utilizado para registar e controlar os períodos de férias gozados por cada colaborador ao longo do ano.
Permite acompanhar a utilização de férias por colaborador e por secção, garantindo controlo e conformidade com o planeamento anual.

No cabeçalho, o relatório apresenta a empresa, o departamento/secção e o ano de referência. O relatório é emitido por secção, sendo apresentada uma tabela distinta para cada uma.

Os dados são apresentados em formato tabular e o relatório é composto por 5 colunas:

- **Matrícula** -- número interno de identificação do colaborador
- **Nome** -- nome completo do colaborador
- **Início** -- data de início do período de férias
- **Fim** -- data de fim do período de férias
- **Dias de Férias** -- número de dias gozados no período

Sempre que um colaborador tem mais do que um período de férias, estes surgem listados em linhas separadas.

No final de cada colaborador é apresentado o total de dias de férias gozados no ano.

<img width="1865" height="390" alt="image" src="https://github.com/user-attachments/assets/7a32b3ef-f7f5-4d7c-8c15-75ca6cdcf805" />

**Parâmetros do relatório (back-end)**

- **i_fk_unit** → unidade (single)
- **i_fk_section** → secções
- **i_fk_employee** → colaboradores
- **i_year** → ano

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Ano:** drop-down
* **Ordenação:** radio button

<img width="1720" height="627" alt="image" src="https://github.com/user-attachments/assets/94b9061c-8607-44af-a79e-760be24978df" />

**Informação técnica**

- **Nome do relatório:** Relatório Anual de Férias
- **Key:** Vacation
- **Função:** S_PCK_CORE_REPORTS.GET_ANUAL_VACATIONS
- **Local de impressão:** Módulo "Relatórios" e vista "Mapa de Ausências"
- **Formatos disponíveis:** Excel, PDF

---

## Relatório de Gerentes por Posto de Trabalho

O **Relatório de Gerentes por Posto de Trabalho** é um mapa de planeamento e controlo da gerência por posto, utilizado para analisar a cobertura de pessoal por secção e posto de trabalho, comparando as horas necessárias com as horas efetivamente planeadas num determinado dia e intervalo horário.

No cabeçalho, o relatório apresenta a unidade, o dia e o horário selecionado, indicando o período exato da análise.

O relatório encontra-se organizado por secções e, dentro de cada secção, por postos de trabalho.
Para cada secção e posto são apresentados:

- **Secção** -- área funcional
- **Posto** -- função ou tipo de posto
- **Horas Necessárias** -- total de horas estimadas como necessárias
- **Horas Planeadas** -- total de horas efetivamente planeadas

De seguida, é apresentada a lista de colaboradores afetos ao posto, com o seguinte detalhe:

- **Operário** -- número mecanográfico do colaborador
- **Nome** -- nome do colaborador
- **Desde** -- hora de início do turno
- **Até** -- hora de fim do turno
- **Horas** -- total de horas planeadas

<img width="1297" height="778" alt="image" src="https://github.com/user-attachments/assets/889c5552-51db-45f7-b8e6-7bb153e3ae9f" />

**Parâmetros do relatório (back-end)**

- I_fk_unit → unidade (single)
- I_fk_secao → secções
- I_data_ini/I_data_fim → período

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Período**
* **Horário:** obrigatório

<img width="1718" height="627" alt="image" src="https://github.com/user-attachments/assets/c86a5ca0-5a58-4ec7-9f5f-1ea6edf9f200" />

**Informação técnica**

- **Nome do relatório:** Relatório de Gerentes por Posto de Trabalho
- **Local de impressão:** Módulo "Relatórios"
- **Key:** WorkstationsManagers
- **Função:** S_PCK_CORE_REPORTS.GET_HOURS_COLAB
- **Formatos disponíveis:** Excel, PDF

---

## Relatório de Horários Escalados

O **Relatório de Horários Escalados** apresenta os horários atribuídos a cada colaborador numa determinada semana, permitindo consultar de forma detalhada os horários planeados por dia.

No cabeçalho, o relatório apresenta o nome do relatório, o período analisado e a identificação da empresa e da secção.

O relatório é apresentado por colaborador, sendo gerado um bloco distinto para cada um.

Para cada colaborador, são apresentados os seguintes dados:

- **Nº Mecanográfico** -- número interno de identificação
- **Nome** -- nome completo do colaborador
- **NIF** -- número de identificação fiscal
- **Dia** -- data específica do horário escalado
- **Horário** -- horário atribuído para esse dia, incluindo períodos de trabalho e pausas

Cada linha corresponde a um dia do período em análise.

<img width="1847" height="504" alt="image" src="https://github.com/user-attachments/assets/44ce0e7e-7867-45ae-99a1-a3af491cf569" />

**Parâmetros do relatório (back-end)**

- **I_DATA_INI / I_DATA_FIM** → período
- **I_FK_UNIDADE** → unidade (single)
- **I_FK_SECAO** → secções (multi)
- **I_FK_COLABORADOR** → colaboradores (multi)
- **I_IDIOMA** → idioma

**Filtros do relatório**

* **Unidades:** multi-seleção (OBRIGATÓRIO)
* **Secções:** multi-seleção
* **Colaboradores:** multi-seleção
* **Período**

<img width="1720" height="624" alt="image" src="https://github.com/user-attachments/assets/59fcd6bb-bc3a-43c2-983d-4e7c0953c9c4" />

**Informação técnica**

- **Nome do relatório:** Relatório de Horários Escalonados
- **Key:** WorkScheduleBi
- **Função:** S_PCK_CORE_REPORTS.GET_WORKSCHEDULEBI
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Relatório de Horas Necessárias vs. Planeadas

O **Relatório de Horas Necessárias vs. Planeadas** apresenta uma análise comparativa entre as horas estimadas como necessárias para a operação e as horas efetivamente planeadas, por secção e por posto de trabalho. Este relatório permite identificar desequilíbrios de planeamento, como défice ou excesso de horas, apoiando a tomada de decisão operacional e o ajuste de escalas.

No cabeçalho, o relatório apresenta a unidade, o dia analisado e o horário selecionado.
A informação é apresentada numa tabela única, organizada por secção e posto de trabalho.

Os dados são apresentados em formato tabular e o relatório é composto por 4 colunas:

- **Secção** -- área funcional da loja
- **Posto** -- tipo de posto ou função
- **Horas Necessárias** -- total de horas estimadas como necessárias para garantir a operação
- **Horas Planeadas** -- total de horas efetivamente escalonadas para o período analisado

Cada linha corresponde a um posto dentro de uma secção, permitindo identificar rapidamente diferenças entre necessidade e planeamento.

<img width="1317" height="396" alt="image" src="https://github.com/user-attachments/assets/8a7371ab-6cf6-4bfa-9277-2dc14942ae86" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades
- **I_FK_SECAO** → secções
- **I_DATA** → data
- **I_DATA_INI / I_DATA_FIM** → intervalo

**Filtros do relatório**

* **Unidades**: drop-down (OBRIGATÓRIO)
* **Secções**: drop-down
* **Período**
* **Horário** (OBRIGATÓRIO)

<img width="1718" height="623" alt="image" src="https://github.com/user-attachments/assets/346b53f7-80cf-44c9-9029-630f73f94019" />

**Informação técnica**

- **Nome do relatório**: Relatório de Horas Necessárias vs. Planeadas
- **Key:** HoursPlannedVsNeeded
- **Função**: S_PCK_CORE_REPORTS.GET_PLAN_NEED_HOURS
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Relatório de Horas Planeadas

O **Relatório de Horas Planeadas** apresenta um mapa consolidado do total de horas de trabalho planeadas, por unidade, região e data.
Este relatório fornece uma visão global do planeamento operacional, sendo especialmente útil para análise comparativa entre unidades, controlo centralizado e acompanhamento do planeamento diário.

A informação é apresentada numa tabela única, organizada hierarquicamente por região e unidade.

Os dados são apresentados em formato tabular e o relatório é composto por 5 colunas:

- **Região** -- região geográfica a que a unidade pertence
- **Cód. Unidade** -- código interno de identificação da unidade
- **Nome da Unidade** -- designação da loja ou unidade operacional
- **Data** -- data a que o planeamento de horas diz respeito
- **Horas Planeadas** -- total de horas planeadas para a unidade nessa data

Cada linha corresponde a uma unidade específica num determinado dia.

<img width="1880" height="718" alt="image" src="https://github.com/user-attachments/assets/30ea7bba-7de6-42c1-8923-52f8b2330dc3" />

**Parâmetros do relatório (back-end)**

- **I_FK_STATE** → estados (multi)
- **I_FK_UNITY** → unidades (multi)
- **I_DATA_INI / I_DATA_FIM** → período

**Filtros do relatório**

* **Países**: multi-seleção (OBRIGATÓRIO)
* **Regiões**: multi-seleção (OBRIGATÓRIO)
* **Unidades**: multi-seleção
* **Período**

<img width="1719" height="627" alt="image" src="https://github.com/user-attachments/assets/4846e9b2-b589-4cc8-a8e6-7a96900d4c17" />

**Informação técnica**

- **Nome do relatório**: Relatório de Horas Planeadas
- **Key:** PlannedHours
- **Função**: S_PCK_CORE_REPORTS.GET_PLANNED_HOURS
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Relatório de Isenção de Horários de Trabalho

O **Relatório de Isenção de Horários de Trabalho** apresenta os colaboradores abrangidos por regime de isenção de horário, permitindo controlar a validade, a origem do registo e a informação associada à sua criação. Este relatório é essencial para efeitos legais, auditoria e controlo de regimes especiais de trabalho.

No cabeçalho, o relatório apresenta o período analisado e a unidade selecionada.
A informação encontra-se organizada por secção.

Os dados são apresentados em formato tabular e o relatório é composto por 7 colunas:

- **Matrícula** -- número interno de identificação do colaborador
- **Nome do Colaborador** -- nome completo
- **Tem IHT** -- indicação se possui Isenção de Horário de Trabalho (Sim/Não)
- **Início** -- data de início da isenção
- **Fim** -- data de fim da isenção
- **Nome do Utilizador** -- utilizador ou sistema que criou o registo
- **Data de Criação** -- data de criação da isenção no sistema

<img width="1898" height="370" alt="image" src="https://github.com/user-attachments/assets/482d89da-9c20-475c-b810-2c69cebe5d44" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (single)
- **I_FK_SECTION** → secção (single)
- **I_FK_EMPLOYEE** → colaborador (single)
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

* **Unidades**: drop-down (OBRIGATÓRIO)
* **Secções**: drop-down
* **Colaboradores**: drop-down
* **Período**

<img width="1715" height="627" alt="image" src="https://github.com/user-attachments/assets/48752c8c-4ae4-4aba-911c-65372b44c469" />

**Informação técnica**

- **Nome do relatório**: Relatório de Isenção de Horários de Trabalho
- **Key**: WorkTimeExemption
- **Função**: S_PCK_CORE_EXECUTION_REPORTS.GET_COLAB_IHT
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Relatório de Transferências e Empréstimos

O **Relatório de Transferências e Empréstimos** apresenta o registo das movimentações internas de colaboradores entre secções, postos ou unidades, permitindo acompanhar mobilidade temporária ou definitiva. Este relatório apoia o controlo administrativo e operacional das transferências.

No cabeçalho, o relatório apresenta a unidade, o período analisado e o tipo de registo (Transferência ou Empréstimo). A informação é apresentada em formato tabular, com uma linha por movimento.

O relatório é composto por 6 colunas:

- **Origem** -- secção, posto ou unidade de origem
- **Destino** -- secção, posto ou unidade de destino
- **Data de Ativação** -- data em que a transferência/empréstimo entrou em vigor
- **Matrícula** -- número interno de identificação do colaborador
- **Nome** -- nome completo do colaborador
- **Estado** -- estado do processo (ex.: Processado)

<img width="1862" height="564" alt="image" src="https://github.com/user-attachments/assets/84caa74e-d634-4d69-993c-1dde5bc5648a" />

**Parâmetros do relatório (back-end)**

- **I_IDIOMA** → idioma
- **I_FK_UNIT** → unidade (1)
- **I_FK_SECTION** → secção (1)
- **I_FK_EMPLOYEE** → colaborador (1)
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

* **Unidades**: drop-down (OBRIGATÓRIO)
* **Secções**: drop-down
* **Colaboradores**: drop-down
* **Período**
* **Tipo**: radio-button (Transferência / Empréstimo)

<img width="1706" height="619" alt="image" src="https://github.com/user-attachments/assets/162d69e9-a7f6-4f79-b12d-9a44d6e30fd5" />

**Informação técnica**

- **Nome do relatório**: Relatório de Transferências e Empréstimos
- **Key**: MoveCollaborator
- **Função**: S_PCK_CORE_REPORTS.GET_MOVE_COLLABORATOR
- **Local de impressão**: Módulo "Relatórios"
- **Formatos disponíveis**: Excel, PDF

---

## Relatório Mensal de Horários

O **Relatório Mensal de Horários** é uma cópia impressa da vista mensal de horários, utilizada para planear, visualizar e controlar os horários de trabalho dos colaboradores ao longo de um mês, por secção. Este relatório é amplamente utilizado para planeamento operacional, comunicação de horários e arquivo.

No cabeçalho, o relatório apresenta a empresa, sede, atividade, unidade, morada, horário de funcionamento, bem como o mês e ano de referência.
A informação encontra-se organizada por secção, sendo apresentada uma grelha mensal para cada uma.

A grelha apresenta:

- **Linhas** -- colaboradores
- **Colunas** -- dias do mês, com dia da semana e data

Em cada célula são registados:

- Horários diários (entrada, saída e pausas)
- **FOLGA** -- dias de descanso
- **FERIADO** -- feriados
- Dias sem horário atribuído, quando aplicável

À esquerda da grelha surgem:

- **Nº Mecanográfico** -- número interno do colaborador
- **Nome do colaborador**

<img width="1885" height="335" alt="image" src="https://github.com/user-attachments/assets/2033dd28-5116-4ad2-bf56-69af972441d9" />

**Parâmetros do relatório (back-end)**

*	**i_fk_unidade** → unidade (single)
*	**i_fk_secao** → secções (multi)
*	**I_FK_GROUP** → grupos (multi)
*	**i_fk_colaborador** → colaboradores (multi)
*	**I_EMPLOYEE_FILTER** → filtro extra (string/num)
*	**i_hora** → hora de saída

**Filtros do relatório**

* **Unidades**: drop-down (OBRIGATÓRIO)
* **Secções**: multi-seleção
* **Grupos**: multi-seleção
* **Colaboradores**: multi-seleção
* **Somente Colaboradores Ativos**: check-box
* **Período**
* **Agregação** (Secção/Grupo): radio-button
* **Ordenação**: radio-button
* **Opções de impressão**: radio-button

<img width="1716" height="618" alt="image" src="https://github.com/user-attachments/assets/ff43a072-1e55-4822-88e9-31c111a31be0" />

**Informação técnica**

- **Nome do relatório**: Relatório Mensal de Horários
- **Local de impressão**: Módulo "Relatórios / Vista mensal de horários / Escala"
- **Key**: MonthlyScheduleReport 
- **Função**: S_RELATORIOS.GET_ENTIDADE_OFICIAL
- **Formatos disponíveis**: Excel, PDF

---

## Resumo de Gerentes Ausentes

O relatório **Resumo de Gerentes Ausentes** apresenta uma síntese das ausências registadas para gerentes na data selecionada, permitindo quantificar rapidamente folgas, férias, feriados, compensações e ausências, agregadas por **secção** e **posto**. Este relatório é útil para análise diária de cobertura de chefias e identificação de impactos operacionais causados por ausências.

No cabeçalho, o relatório apresenta a **unidade** e a **data de referência**. A informação encontra-se organizada em dois blocos: um quadro de **totais globais resumidos** e um quadro **detalhado por secção e posto**.

Os dados são apresentados em formato tabular e o relatório contém os seguintes indicadores:

- **Totais resumidos**: Folgas, Feriados, Férias, Compensações, Ausências
- **Detalhe por secção e posto** com contadores por tipologia:
  - **FO** -- Folgas
  - **FC** -- Folgas compensatórias
  - **FER** -- Feriados
  - **Férias** -- Dias de férias
  - **DBE** -- Débito (ex.: Banco de Horas/Excesso de horas, conforme parametrização)
  - **DBT** -- Débito (ex.: Banco de Tempo, conforme parametrização)
  - **AR** -- Ausência registada
  - **ANR** -- Ausência não registada

<img width="1877" height="267" alt="image" src="https://github.com/user-attachments/assets/79324d28-c342-4f1b-8221-51c063ecddc7" />

**Parâmetros do relatório (back-end)**

-	**I_fk_unit** → unidade (1)
-	**I_fk_secao** → secções (multi)
-	**I_fk_grupo** → grupos (multi)
-	**I_data** → período

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** multi-seleção
* **Grupos:** multi-seleção
* **Período/Data:** data (dia)

<img width="1709" height="619" alt="image" src="https://github.com/user-attachments/assets/fe0d310a-e6e0-42c1-b029-408072eea24d" />

**Informação técnica**

- **Nome do relatório:** Resumo de Gerentes Ausentes
- **Key:** AbsentManagersSummary
- **Função:** S_PCK_CORE_REPORTS.GET_ABSENCES_TYPES
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Tempos Fora do Posto

O relatório **Tempos Fora do Posto** apresenta os registos de períodos em que os colaboradores estiveram ausentes do seu posto de trabalho durante o horário laboral, indicando a duração e o motivo associado. Este relatório é fundamental para monitorização de pausas/ausências operacionais (ex.: aleitação, formação, folga por excesso de horas) e para suporte a auditorias internas de presença no posto.

No cabeçalho, o relatório apresenta a **loja/unidade**, o **período analisado** e a(s) **secção(ões)**. A informação encontra-se organizada por secção, sendo apresentada uma tabela distinta para cada uma.

Os dados são apresentados em formato tabular e cada linha corresponde a um registo individual de tempo fora do posto. O relatório é composto pelas seguintes colunas:

- **Colaborador** -- nome do colaborador
- **Nº Mecanográfico** -- número interno de identificação
- **Período** -- data em que ocorreu o registo
- **Horário de Ausência** -- intervalo horário em que esteve ausente do posto
- **Total** -- duração total do tempo fora do posto
- **Motivo** -- motivo/justificação associada (ex.: Aleitação, Formação, etc.)

<img width="1873" height="129" alt="image" src="https://github.com/user-attachments/assets/558ae2f3-f8bf-407b-bfd0-403268769e30" />

**Parâmetros do relatório (back-end)**

- **i_idioma** → idioma
- **i_fk_unit** → unidade (1)
- **i_fk_section** → secções (multi)
- **i_fk_employee** → colaboradores (multi)
- **i_start_date / i_end_date** → período

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Período**
* **Ordenação:** radio button
  
<img width="1713" height="616" alt="image" src="https://github.com/user-attachments/assets/5494ba54-8b8a-4708-b854-6ca3599ca578" />

**Informação técnica**

- **Nome do relatório:** Tempos Fora do Posto
- **Key:** WorkStationAbsences
- **Função:** S_PCK_CORE_REPORTS.GET_WORKSTATION_ABSENCES
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Tolerâncias

O relatório **Tolerâncias** apresenta os desvios entre a hora planeada e a hora efetivamente executada pelos colaboradores, considerando regras/limites de tolerância definidos. Este relatório é útil para identificar atrasos, saídas antecipadas ou variações de marcação dentro (ou fora) dos limiares aceitáveis, apoiando o controlo de assiduidade e conformidade.

No cabeçalho, o relatório apresenta a **loja/unidade**, o **período** e a **secção**. A informação encontra-se organizada por secção, com tabelas separadas quando aplicável.

Os dados são apresentados em formato tabular e cada linha corresponde a um registo individual de tolerância. O relatório é composto pelas seguintes colunas:

- **Nº Mecanográfico** -- número identificativo do colaborador
- **Colaborador** -- nome do colaborador
- **Carga Horária** -- carga horária contratual
- **Data** -- data do registo
- **Dia da Semana** -- dia da semana correspondente
- **Hora Planeada** -- hora prevista no planeamento
- **Hora Executada** -- hora registada/realizada
- **Tempo (minutos)** -- diferença entre planeado e executado
- **Tipo** -- tipo de tolerância aplicada
- **IHT** -- indicação de isenção de horário (Sim/Não)

<img width="1868" height="147" alt="image" src="https://github.com/user-attachments/assets/7067b48b-2260-477e-a4d3-351ee40e5658" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade (single)
- **I_FK_SECTION** → secções
- **I_FK_EMPLOYEE** → colaboradores
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Período**
* **Ordenação:** radio button

<img width="1712" height="621" alt="image" src="https://github.com/user-attachments/assets/edb24a95-9ab3-4030-af29-a55fd15f444a" />

**Informação técnica**

- **Nome do relatório:** Tolerâncias
- **Key:** Tolerances
- **Função:** S_PCK_CORE_EXECUTION_REPORTS. Get_tolerances
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Trabalho Suplementar

O relatório **Trabalho Suplementar** apresenta os registos de trabalho efetuado fora do horário normal, permitindo acompanhar, validar e justificar trabalho adicional realizado num período. É um relatório de suporte à validação operacional e administrativa, incluindo motivo e fundamento associado.

No cabeçalho, o relatório apresenta o **nome do relatório**, o **período analisado**, a **unidade/loja** e o **departamento/secção**. A informação encontra-se organizada por secção, com tabelas separadas por secção.

Os dados são apresentados em formato tabular. Cada linha corresponde a um registo de trabalho suplementar associado a um colaborador. O relatório é composto pelas seguintes colunas:

- **Matrícula** -- número interno de identificação do colaborador
- **Nome** -- nome completo do colaborador
- **Tipo de Dia** -- classificação do dia (ex.: útil, feriado, etc., conforme regra)
- **Data** -- data do registo
- **Duração** -- tempo total registado como suplementar
- **Hora Início** -- hora de início do trabalho suplementar
- **Hora Fim** -- hora de fim do trabalho suplementar
- **Motivo** -- motivo/justificação
- **Fundamento** -- base administrativa/legal do registo

No final de cada secção pode existir resumo com **totais por colaborador** e **total de colaboradores**.

<img width="1844" height="819" alt="image" src="https://github.com/user-attachments/assets/df2349a6-0dec-41b5-8197-a4de0216866f" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi)
- **I_FK_SECTION** → secções (multi)
- **I_FK_EMPLOYEE** → colaboradores (multi)
- **I_BEGIN_DATE / I_END_DATE** → período
- **I_LIST_DAYS** → lista/tipo de dias (string)

**Filtros do relatório**

* **Unidades:** multi-seleção
* **Secções:** multi-seleção
* **Colaboradores:** multi-seleção
* **Período**
* **Lista dias (Todos os Dias/Só trabalho Suplementar):** radio button

<img width="1715" height="620" alt="image" src="https://github.com/user-attachments/assets/2b126a47-7bbe-4f82-83b0-ab2a27d79140" />

**Informação técnica**

- **Nome do relatório:** Trabalho Suplementar
- **Key:** SupplementaryWork
- **Função:** S_PCK_CORE_EXECUTION_REPORTS. Get_supp_work
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Trabalho Temporário

O relatório **Trabalho Temporário** apresenta os registos associados a trabalho realizado no contexto de trabalho temporário, permitindo acompanhar e validar ocorrências por colaborador, com detalhe diário e totalizações. É particularmente útil para controlo de prestação de trabalho e reconciliação administrativa com entidades de trabalho temporário, quando aplicável.

No cabeçalho, o relatório apresenta o **nome do relatório**, o **período analisado**, a **loja/unidade** e o **departamento/secção**. A informação encontra-se organizada por secção, com tabelas separadas quando aplicável.

Os dados são apresentados em formato tabular e cada linha corresponde a um registo individual (por data) associado ao colaborador. A tabela inclui:

- **Data** -- data do registo
- **Entradas/Saídas** -- registos horários (podendo existir múltiplos blocos por dia)
- **THT** -- total de horas trabalhadas (no dia ou agregado)
- **TS** -- total suplementar (quando aplicável)

<img width="1863" height="666" alt="image" src="https://github.com/user-attachments/assets/127b9e85-ebfc-418d-8a88-08506fd1c4e3" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidades (multi)
- **I_FK_SECTION** → secções (multi)
- **I_FK_EMPLOYEE** → colaboradores (multi)
- **I_FK_TEMPORARY_COMPANY** → empresas de trabalho temporário (multi)
- **I_YEAR** → ano
- **I_MONTH** → mês

**Filtros do relatório**

* **Unidades:** multi-seleção
* **Secções:** multi-seleção
* **Colaboradores:** multi-seleção
* **Empresa trabalho temporário:** multi-seleção
* **Período** (mês/ano)
* **Ordenação:** radio button

<img width="1337" height="602" alt="image" src="https://github.com/user-attachments/assets/947ff26b-d60d-4f59-a541-e88bf9af6e82" />

**Informação técnica**

- **Nome do relatório:** Trabalho Temporário
- **Key:** TemporaryWork
- **Função:** PCK_CORE_EXECUTION_REPORTS.GET_PUNCHES_TEMPORARYWORK_V0
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF

---

## Trocas e Ajustes

O relatório **Trocas e Ajustes** apresenta o registo de alterações efetuadas aos horários ou à carga horária dos colaboradores num período, permitindo comparar claramente o "antes" e o "depois" de cada alteração, bem como o motivo e o utilizador responsável. É útil para auditoria de mudanças, validação de planeamento e controlo de exceções.

No cabeçalho, o relatório apresenta a **unidade** e o **período analisado**. A informação encontra-se organizada por secção, com tabelas separadas por secção e indicação do **total de alterações** em cada secção.

Os dados são apresentados em formato tabular e cada linha corresponde a uma alteração (troca/ajuste). O relatório é composto pelas seguintes colunas:

- **Matrícula** -- número interno de identificação do colaborador
- **Nome Colaborador** -- nome completo do colaborador
- **Data** -- data em que a alteração ocorreu
- **Anterior – Horário/Carga** -- horário e carga antes da alteração
- **Atual – Horário/Carga** -- horário e carga após a alteração
- **Motivo da Alteração** -- justificação da mudança
- **Utilizador** -- utilizador/sistema que efetuou o registo
- **Data da Alteração** -- data em que ficou registada no sistema
- **Nº Troca** -- identificador da troca/ajuste

<img width="1870" height="281" alt="image" src="https://github.com/user-attachments/assets/0edd3a5d-4145-4e7d-866b-8df9196f2ed5" />

**Parâmetros do relatório (back-end)**

- **I_FK_UNIT** → unidade
- **I_FK_SECTION** → secções
- **I_FK_EMPLOYEE** → colaboradores
- **I_BEGIN_DATE / I_END_DATE** → período

**Filtros do relatório**

* **Unidades:** drop-down (OBRIGATÓRIO)
* **Secções:** drop-down
* **Colaboradores:** drop-down
* **Período**
* **Ordenação:** radio button
  
<img width="1712" height="616" alt="image" src="https://github.com/user-attachments/assets/aa237f5f-1fd1-4c48-823a-03061f7a6af6" />

**Informação técnica**

- **Nome do relatório:** Trocas e Ajustes
- **Key:** ExchangesAndAdjustments
- **Função:** S_PCK_CORE_EXECUTION_REPORTS.Get_exchanges_adjustments
- **Local de impressão:** Módulo "Relatórios"
- **Formatos disponíveis:** Excel, PDF
