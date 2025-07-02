# 📊 Projeto Power BI - Formação Power BI Analyst (DIO)

Este projeto faz parte do desafio da **Formação Power BI Analyst** promovida pela [DIO](https://www.dio.me/). O objetivo foi trabalhar com dados de colaboradores, departamentos e salários, realizando o tratamento e modelagem dos dados, além da criação de um dashboard interativo com indicadores estratégicos.

## 🛠️ Etapas Realizadas

1. **Verificação dos Cabeçalhos e Tipos de Dados:**  
   Conferência dos nomes das colunas e dos tipos atribuídos automaticamente pelo Power BI, com ajustes manuais quando necessário.

2. **Conversão de Valores Monetários:**  
   Padronização dos campos salariais para o tipo `double` com precisão adequada.

3. **Tratamento de Valores Nulos:**  
   Análise da presença de valores nulos. Os campos `Super_ssn` foram avaliados e interpretados como possíveis indicações de gerência.

4. **Verificação de Colaboradores sem Gerente:**  
   Identificação de registros onde `Super_ssn` está nulo, validando se representam cargos de chefia.

5. **Análise de Departamentos sem Gerente:**  
   Verificação de integridade das relações entre `departamentos` e seus respectivos `gerentes`.

6. **Preenchimento de Dados Faltantes:**  
   Em casos de departamentos sem gerente, foi assumido que os dados estavam disponíveis e as lacunas foram preenchidas com valores fictícios consistentes.

7. **Validação de Número de Horas por Projeto:**  
   Análise para garantir que os valores de horas estavam coerentes e não nulos.

8. **Separação de Colunas Complexas:**  
   Divisão de colunas compostas em múltiplas colunas simples para melhor manipulação.

9. **Mesclagem de Tabelas `Employee` e `Department`:**  
   Utilizada a tabela `Employee` como base para a junção via Power BI, garantindo que cada colaborador tivesse o nome do seu departamento associado corretamente.

10. **Eliminação de Colunas Desnecessárias:**  
    Durante o processo de transformação de dados, colunas sem uso no relatório final foram removidas.

11. **Associação entre Colaboradores e Gerentes:**  
    Utilizado Power BI para mesclar dados de `employees` com os respectivos nomes de seus `gerentes` a partir do `Super_ssn`.

12. **Criação de Nome Completo dos Colaboradores:**  
    Junção das colunas `first_name` e `last_name` em uma única coluna `full_name`.

13. **Criação de Combinação Departamento + Localização:**  
    As colunas `department_name` e `location` foram unidas para formar uma chave única, facilitando a criação de dimensões no modelo estrela.

14. **Agrupamento por Gerente:**  
    Agrupamento dos dados para identificar o número de colaboradores sob responsabilidade de cada gerente.

## 📈 Visualizações Criadas

O relatório apresenta os seguintes elementos:

- Indicadores com contagem de:
  - Departamentos
  - Funcionários
  - Chefes
  - Total em salários
- Gráficos de:
  - Funcionários por departamento
  - Funcionários por gerente
  - Distribuição por cidade

![image](https://github.com/user-attachments/assets/0c88144b-06a4-4bf2-9895-2f2cce78db53)


---

✅ Projeto finalizado com sucesso, aplicando boas práticas de ETL no Power BI, modelagem relacional e construção de dashboard com KPIs relevantes para análise de pessoas e gestão.

