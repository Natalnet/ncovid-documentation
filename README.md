# ncovid-documentation

Documentar o desenvolvimento do sistema ncovid

# Definições do sistema

## DAVI

--------
I. O que é o sistema?

O propósito principal do sistema é fornecer um ambiente (site) para auxiliar gestores e autoridades a melhor alocar recursos no combate às epidemias virais. De início, o sistema será usado para a pandemia do covid. Para isto, o sistema fornece predições das curvas da pandemia (principalmente a de mortes) e também permite a geração de resultados esperados de certas ações. Por exemplo, caso aumente o investimento em máscaras, quais são os efeitos esperados na curva? (com embasamento científico). Quais os efeitos de lockdown (se fizermos lockdown por tal período qual é o efeito esperado na curva?). Informações deste tipo devem ser disponibilizadas pelo site. O site deve ser amigável o suficiente para facilitar o uso por pessoas leigas.

A princípio o site fará estes processos para um estado brasileiro. Na sua forma final, o sistema deve ser capaz de coletar, agregar e tratar dados, treinar modelos e realizar predições e sugestões de ações para qualquer região do mundo.


--------
II.  Stakeholders:

Cidadão Comum

Gestores

Desenvolvedores

--------
III.  Casos de Uso por Stakeholder:

Cidadão Comum:
Visualizar predições das curvas
Mostrar taxa de acerto de previsões passadas (grau de confiança)

Gestores:
Visualizar predições das curvas
Visualizar resultados de possíveis ações

Desenvolvedor:
Carregar curvas
Processar curvas
Treinar modelos
Avaliar modelos


## DUNFREY

## JULIO

--------
I. O que é o sistema?

Uma plataforma para gestores e afins consultarem-se a respeito de dados de uma pandemia particular. Essa consulta deve informá-los a respeito de: o estado de um recente passado, o estado atual e, a partir desse um conjunto de dados passados e atuais, prever o estado futuro da pandemia. Esse estado deve ser entregue como curvas de contágio e óbitos, em termos de séries temporais, por exemplo. Tais séries temporais, usadas na entrada ou oferecidas na sáida, estão limitadas a uma certa quantidade de dias na entrada e na saída do processo de prediação.


--------
II. Stakeholders:
Um stakeholder é um perfil de usuário que compõe a lista de pessoas/profissionais e/ou empresas que operam na construção e uso do sistema diretamente.

Desenvolvedores: entre os desenvolvedores temos as especializações: Cientistas de Dados, Engenheiros e Arquitetos de Software.

Usuários: entre os usuários temos as especializações: Gestores (Públicos, ONGs, Empresas) e Pesquisadores/Cientistas


--------
III. Casos de Uso por Stakeholder:
  Casos de uso são uma lista de senteças transitivas ou intransitivas. cada sentença implica um sujeito, um verbo de ligação e um predicado.

  a. Usuários:Gestores 
  a.1. solicita a visualização da curva de: 
  a.1.1. contágio ou óbito para:
  a.1.1.1. uma localidade, em um período de tempo e de um repositório de dados:
  a.1.1.1.1. curva já consolidada, ou
  a.1.1.1.2. curva para predição
  
  (essa forma acima é mais trabalhosa. fica mais a título de exemplo. vcs podem simplificar e escrever como abaixo, e depois refinamos. também não se ocupem com o stackholder de tipo "Desenvolvedores". vamos nos ocupar por hora com as funcionalidades vistas pelos papeis de tipo "Usuários")
  
  b. Usuários:Pesquisadores 
  b.1. Importa I.1
  b.2. Solicita listagem de modelos do repositório da plataforma
  b.3. Solicita listagem de hiperparâmetros de modelos do repositório da plataforma
  b.4. Cadastrar perfil de pesquisador e associar modelos e hiperparâmetros usados por esse a sua conta  
  b.5. Cadastrar repositório de dados do próprio pesquisador
  b.6. Treinar modelo a partir de repositório de dados indicado pelo cientista

## FRANCINALDO

## EMERSON
