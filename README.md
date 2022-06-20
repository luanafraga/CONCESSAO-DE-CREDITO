# PONTUACAO-DE-CREDITO

**Projeto Concessão de Crédito**

O projeto foi desenvolvido utilizando linguagem **Python** no Jupyter Notebook. O python possui um série de bibliotecas que nos auxiliam na construção das análises e modelagem dos dados. Neste projeto, foram utilizadas as seguintes:

   - Pandas
   - Numpy
   - Seaborn
   - Matplotlib
   - Plotly
   - Scikit-learn

**Objetivo**

O objetivo deste projeto é criar um **modelo de decisão de crédito** para que o Bytebank, um banco digital, use na concessão deste. O evento que nós estamos buscando é **classificar os nossos solicitantes em adimplentes ou inadimplentes**, de acordo com as informações cadastrais e financeiras fornecidas pelo cliente.

**Dados**

A base de dados possui informações sobre:

  - **default:** se o cliente foi adimplente (1) ou inadimplente (0)
  - **conta_corrente:** valor em conta corrente
  - **prazo_emprestimo_meses:** prazo do empréstimo em meses
  - **historico_credito:** histórico de crédito do cliente
  - **proposito_emprestimo:** propósito do empréstimo
  - **valor_emprestimo:** valor do empréstimo
  - **reserva_cc:** reserva em conta corrente
  - **tempo_emprego_atual:** tempo do emprego atual do cliente
  - **taxa_comp_salario:** taxa de comprometimento do salário
  - **sexo_est_civil:** sexo e estado civil do cliente
  - **outros_fiadores:** se o cliente possui outros fiadores
  - **anos_residencia_atual:** quantidade de anos da residencia atual do cliente
  - **propriedade:** se o cliente possui propriedade
  - **idade:** idade do cliente
  - **outros_planos_financiamento:** se o cliente possui outros planos de financiamento
  - **tipo_residencia:** tipo de residência
  - **n_creditos_banco:** quantidade de créditos no banco
  - **status_emprego:** se o cliente está empregado
  - **n_dependentes:** número de dependentes do cliente
  - **telefone:** se o cliente possui telefone
  - **trabalhador_estrangeiro:** se o cliente é estrangeiro


**Conclusões**


Após o pré-processamento dos dados, foi criado um modelo de **Regressão Logística** com a biblioteca Scikit Learn. Este modelo foi selecionado para o desenvolvimento do projeto porque pode ser replicado com facilidade e também conseguimos entender bem como as variáveis do problema estão afetando os resultados. Além de que, não exige grande poder computacional e isso a torna atrativa já que podemos ter grandes bases de dados de clientes. O modelo foi treinado e avaliado utilizando métricas de avaliação matemáticas e gráficas.

Por fim, Conseguimos concluir após nosso estudo que o banco precisa ficar atento a alguns padrões da maioria dos clientes com **crédito negado**:
    
    Não possui conta-corrente;
    Possui conta crítica/outros créditos existentes;
    Valor do empréstimo entre 1000 e 1500 euros;
    Possui alta taxa de comprometimento do salário;
    São homens solteiros;
    Sem fiador;
    Não há telefone registrado;
    Possui 20 a 40 anos de idade;
    É trabalhador estrangeiro.
