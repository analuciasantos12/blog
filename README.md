## Alertas

O relatório **Alertas** apresenta todos os parâmetros legais que não foram cumpridos no período selecionado, identificando de forma detalhada os colaboradores em incumprimento e a natureza de cada violação legal.

### Informação apresentada

Para cada ocorrência, o relatório indica:

* Colaborador a que o incumprimento diz respeito
* Parâmetro legal não respeitado
* Valor legal definido
* Valor efetivamente aplicado
* Valor de incumprimento (diferença entre o valor aplicado e o limite legal)

### Informação de auditoria

* Utilizador responsável pela última alteração
* Data da alteração
* Indicação de troca, quando aplicável

### Cabeçalho

* Unidade / Loja
* Período de análise

### Estrutura da tabela

| Coluna                 | Descrição                    |
| ---------------------- | ---------------------------- |
| Nº Mecanográfico       | Identificador do colaborador |
| Colaborador            | Nome do colaborador          |
| Parâmetro Legal        | Parâmetro avaliado           |
| Valor Legal            | Limite legal                 |
| Data Início            | Início do incumprimento      |
| Data Fim               | Fim do incumprimento         |
| Valor Aplicado         | Valor registado              |
| Valor de Incumprimento | Diferença apurada            |
| Utilizador             | Responsável pela alteração   |
| Data                   | Data da alteração            |
| Troca                  | Indicação de troca           |

### Configurações do relatório

* `i_fk_unit` → unidades (multi-seleção)
* `i_fk_section` → secções (multi-seleção)
* `i_fk_employee` → colaboradores (multi-seleção)
* `i_legal_params` → parâmetros legais
* `i_start_date / i_end_date` → período

### Filtros

* Unidades (**obrigatório**)
* Secções
* Colaboradores
* Parâmetros legais
* Período
* Ordenação

### Informação técnica

* **Nome:** Alertas
* **Função:** `S_PCK_CORE_REPORTS.GET_ALERTS`
* **Módulo:** Relatórios
* **Formatos:** Excel, PDF

---

## Alterações à Escala

O relatório **Alterações à Escala** apresenta todas as alterações efetuadas às escalas de trabalho no período selecionado, permitindo acompanhar o histórico de mudanças de horários e cargas horárias.

### Informação apresentada

* Colaborador afetado
* Data da alteração
* Horário e carga **antes** da alteração
* Horário e carga **após** a alteração
* Motivo da alteração
* Utilizadores de criação e alteração
* Datas de criação e alteração
* Número e estado da troca

### Cabeçalho

* Unidade
* Período
* Secção
* Total de alterações encontradas

### Estrutura da tabela

| Coluna                   | Descrição                    |
| ------------------------ | ---------------------------- |
| Matrícula                | Identificador do colaborador |
| Nome do Colaborador      | Nome completo                |
| Data                     | Data da alteração            |
| Anterior – Horário/Carga | Antes da alteração           |
| Atual – Horário/Carga    | Depois da alteração          |
| Motivo da Alteração      | Motivo selecionado           |
| Utilizador de Criação    | Criador                      |
| Data de Criação          | Data de criação              |
| Utilizador de Alteração  | Última alteração             |
| Data de Alteração        | Data da alteração            |
| Nº Troca                 | Número da troca              |
| Estado da Troca          | Estado atual                 |

### Configurações

* `i_fk_unit` → unidades
* `i_fk_section` → secções
* `i_fk_employee` → colaboradores
* `i_begin_date / i_end_date` → período
* `i_status` → estado da troca
* `i_show_history` → mostrar histórico
* `i_only_workflow` → apenas workflow

### Informação técnica

* **Nome:** Alterações à Escala
* **Key:** ScheduleExchanges
* **Função:** `S_PCK_CORE_REPORTS.GET_CHANGE_SCHEDULE`
* **Formatos:** Excel, PDF

---

## Alterações de Carga Horária

O relatório **Alterações de Carga Horária** apresenta todas as modificações efetuadas à carga horária contratual dos colaboradores.

### Estrutura da tabela

| Coluna              | Descrição           |
| ------------------- | ------------------- |
| Matrícula           | Nº do colaborador   |
| Nome do Colaborador | Nome completo       |
| Data Criação CH     | Data de criação     |
| Nova Carga Horária  | Nova carga          |
| Data Início CH      | Início da vigência  |
| Data Fim CH         | Fim da vigência     |
| Estado              | Estado da alteração |

### Informação técnica

* **Nome:** Alterações de Carga Horária
* **Key:** WorkloadChange
* **Função:** `S_PCK_CORE_REPORTS.GET_WORKLOAD_CHANGE`
* **Formatos:** Excel, PDF

