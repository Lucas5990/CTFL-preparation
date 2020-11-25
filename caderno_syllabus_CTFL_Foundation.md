# ISTQB - CTFL Foundation

## Capítulo 0 - Introdução

| Níveis Cognitivos | - |
|-|-|
| K1 | Lembrar |
| K2 | Entender |
| K3 | Aplicar |

O Exame: 40 questões de múltipla escolha, para ser aprovado 65% (26 acertos).

| Capítulo | Título | Tempo (min) |
| - | - |- |
|1|Fundamentos do teste|175|
|2|Teste durante o ciclo de vida de desenvolvimento de software|100|
|3|Testes estáticos|135|
|4|Técnicas de teste|330|
|5|Gerenciamento de teste|225|
|6|Ferramentas de apoio ao teste|40|


## Capítulo 1 - Fundamentos de teste

#### 1.1 O que é teste ?

Envolve não apenas execução de teste, existem outras fases como: planejamento, análise de requisitos, modelagem, etc.

Testes dinâmicos: São testes que envolvem a execução do componente a ser testado
Testes estáticos: São testes que NÃO envolvem a execução do componente a ser testado

Teste também inclui a revisão de produtos de trabalho, como requisitos, histórias de usuários e código-fonte.

Nem todos os testes que precisam ser executados se encontram nos documentos de histórias de usuário ou requisitos.

##### (K1) Identificar os objetivos típicos de teste

1.1.1 Objetivos típicos do teste

- Evitar defeitos, avaliar os produtos de trabalho, como requisitos, histórias de usuários, modelagem e código;
- Verificar se todos os requisitos especificados foram cumpridos;
- Verificar se o objeto de teste está completo e validar se funciona como os usuários e stakeholders esperam;
- Criar confiança no nível de qualidade do objeto de teste;
- Encontrar defeitos e falhas reduz o nível de risco de qualidade inadequada de software;
- Fornecer informações suficientes aos stakeholders para que tomem decisões especialmente em relação ao nível de qualidade do objeto de teste;
- Cumprir os requisitos ou normas contratuais, legais ou regulamentares, ou verificar a conformidade do objeto de teste com esses requisitos ou normas.

Os objetivos podem variar dependendo do contexto do componente ou sistema que está sendo testado, do nível de teste e do modelo de ciclo de vida de desenvolvimento de software. Exemplos de diferenças:

- Durante o teste do componente, um objetivo pode ser encontrar tantas falhas quanto possível, de modo que os defeitos sejam identificados e corrigidos antecipadamente. Outro objetivo pode ser aumentar a cobertura de código dos testes de componentes;
- Durante o teste de aceite, um objetivo pode ser confirmar que o sistema funciona como esperado e satisfaz os requisitos. Outro objetivo deste teste pode ser fornecer informações aos stakeholders sobre o risco de liberar o sistema em um determinado momento.

##### (K2) Diferenciar o teste da depuração

1.1.2 Teste e depuração de código

A execução dos testes pode mostrar falhas causadas por defeitos no software. Já a depuração é a atividade de desenvolvimento que localiza, analisa e corrige esses defeitos. Normalmente o testador é responsável pelo teste inicial e pelo teste de confirmação final, enquanto os desenvolvedores fazem a depuração e os testes de componentes. 

No entanto, em metodologias ágeis, os testadores podem estar envolvidos na depuração do código e nos teste de componentes.

#### 1.2 Por que o teste é necessário ?

##### (K2) Dar exemplos de porque o teste é necessário

1.2.1 - Contribuições do teste para o sucesso

Com o uso de técnicas de teste nos pontos certos do ciclo de vida de desenvolvimento é possível reduzir a frequência de entregas problemáticas que devido a presença de defeitos causam falhas ou não atendem às necessidades dos stakeholders. Exemplos incluem:

- Ter testadores envolvidos nas revisões de requisitos ou no refinamento da história do usuário poderia detectar defeitos nesses produtos de trabalho. A identificação e remoção de defeitos de requisitos reduz o risco de desenvolvimento de funcionalidade incorreta ou não testável;

- Ter testadores trabalhando em conjunto com os projetistas do sistema pode aumentar o entendimento de cada parte sobre o projeto e como testá-lo;

- Ter testadores trabalhando em estreita colaboração com os desenvolvedores enquanto o código está em desenvolvimento pode aumentar o entendimento de como testar o código, reduzindo o risco de defeitos no código e nos testes;

- Ter testadores para verificar e validar o software antes de liberar pode detectar falhas que poderiam ter sido perdidas e ajudar o processo de remoção dos defeitos que causaram as falhas., aumentando a probabilidade do software atender aos requisitos.


##### (K2) Descrever a relação entre testes e garantia de qualidade e dar exemplos de como os testes contribuem para melhorar a qualidade

1.2.2 Garantia de qualidade e teste

Garantia de qualidade e testes não são sinônimos, um conceito maior os une: "Gerenciamento/Gestão da qualidade"

Garantia de qualidade é o processo tipicamente focado na adesão de processos adequados, a fim de fornecer confiança de que os níveis apropriados de qualidade serão alcançados.

Controle de qualidade é o processo que envolve várias atividades, incluindo testes, que apoiam a obtenção de níveis adequados de qualidade. As atividades de teste são parte do processo geral de desenvolvimento ou manutenção de software.

##### (K2) Distinguir erro, defeito e falha

1.2.3 Erros, defeitos e falhas

Erros: Geralmente refere-se ao ato humano de errar ao fazer algo, como escrever um caso de teste com passo a passo errado por exemplo

Defeito: Defeitos são gerados no produto por conta da ocorrência de erros, por exemplo um bug no código

Falhas: Normalmente refere-se ao teste ou resultado de uma funcionalidade que não funcionou como esperado, um defeito pode desencadear uma falha para determinadas entradas por exemplo. 

Falsos positivos são detecções de defeitos de forma incorreta
Falsos negativos são testes que não detectam um defeito que deveria ter sido detectado


##### (K2) Distinguir causa-raiz de um defeito e seus efeitos

Causa-raiz: São as primeiras ações/condições que contribuiram para que um defeito fosse desencadeado

Exemplo: Um código com um defeito que gera pagamento de juros incorretos (falhas), onde o motivo do defeito foi uma falta de conhecimento por parte do proprietário do produto durante a escrita do documento de histórias. Neste exemplo, a causa raiz foi a falta de conhecimento por parte do proprietário do produto, que resultou no erro ao escrever a história do usuário.


#### 1.3 Os sete princípios de testes

##### (K2) Explicar os sete principios de teste

| Lista | Os 7 princípios de teste |
| - | - |
| 1 | O teste mostra a presença de defeitos e não a sua ausência|
| 2 | Testes exaustivos são impossíveis |
| 3 | O teste inicial economiza tempo e dinheiro |
| 4 | Defeitos se agrupam |
| 5 | Cuidado com o paradoxo do pesticida |
| 6 | O teste depende do contexto |
| 7 | A ausência de erros é uma ilusão |   

1. O teste mostra a presença de defeitos e não a sua ausência

O teste reduz a propabilidade de defeitos, mas não garante que não existe defeito algum.

2. Testes exaustivos são impossíveis

Testar todas as combinações de entradas e pré-condições não é viável a não ser em casos muito triviais. Devem ser levados em conta prioridades e análise de risco.

3. O teste inicial economiza tempo e dinheiro

É mais barato corrigir um defeito de software durante uma etapa inicial do ciclo de vida do desenvolvimento de software.

4. Defeitos se agrupam

Um pequeno número de módulos geralmente contém a maioria dos defeitos durante a fase de pré-lançamento. Esta análise de qual funcionalidade apresenta mais defeitos num estágio inicial é importante para análise de risco citada no principio anterior.

5. Cuidado com o paradoxo do pesticida

Assim como um pesticida deixa de ser eficaz contra insetos após um tempo, os testes podem deixar de encontrar erros e precisarem ser atualizados. Em alguns casos não encontrar mais falhas é benéfico como nos testes automatizados de regressão.

6. O teste depende do contexto

O teste é feito de forma diferente em diferentes contextos, como em projetos ágeis ou sequenciais, ou softwares industriais e aplicativos móveis.

7. Ausência de erros é uma ilusão

Como já descrito nos itens 1 e 2, os testes não garantem que não existem defeitos, e testar todas as possibilidades é impossível.

#### 1.4 Processo de teste

##### (K2) Explicar o impacto do contexto no processo de teste

1.4.1 Processo de teste no contexto

Alguns fatores contextuais que influenciam o processo de teste de uma organização:

- Modelo de ciclo de vida de desenvolvimento de software e metodologias de projeto utilizados;
- Níveis de testes e tipos de teste considerados;
- Risco de produto e projeto;
- Domínio do negócio;
- Restrições operacionais como: orçamento e recursos, escalas de tempo, complexidade, requisitos contratuais e regulamentares
- Políticas e práticas organizacionais
- Normas internas e externas necessárias

As seções a seguir descrevem aspectos gerais dos processos de teste organizacionais:

- Atividades e tarefas de teste;
- Produtos de trabalho de teste;
- Rastreabilidade estre a base de teste e os produtos de trabalho de teste.

É útil se a base de testes tiver definida os critérios de cobertura mensuráveis, pois eles podem atuar como KPIs (indicadores chave de qualidade)


##### (K2) Descrever as atividades de teste e respectivas tarefas dentro do processo de teste

1.4.2 Atividades e tarefas de teste

Um processo de teste consiste nos seguintes grupos principais de atividades:
- Planejamento do teste

Envolve as atividades que definem os propósitos e a abordagem do teste para atender aos objetivos do teste dentro das restrições impostas pelo contexto, por exemplo, especificar técnicas e tarefas de teste adequadas e formular um cronograma de teste para cumprir um prazo. Os planos de teste podem ser revisitados com base no feedback das atividades de monitoramento e controle.

- Monitoramento e controle do teste;

O monitoramento do teste envolve a comparação contínua do progresso real com o plano de teste usando qualquer métrica de monitoramento definida no plano de teste. Engloba a tomada de decisão de ações necessárisa para atender aos objetivos do plano de teste (que pode ser atualizado ao longo do tempo). O monitoramento e controle são apoiados pelos critérios de avaliação das saídas, que são referidos como "feito" em alguns ciclos de vida.
 
 Exemplo de avaliação dos critérios de saída para a execução dos testes: Verificar os resultados do teste e os registros em relação aos critérios específicados de cobertura; Avaliar o nível de qualidade do componente ou sistema com base nos resultados e registros de testes; Determinar se são necessários mais testes.

- Análise do teste;

Durante a análise, a base de teste é analisada para identificar recursos testáveis e definir as condições de teste associadas. A análise determina "o que testar" em termos dos critérios de cobertura mensuráveis.

Inclui as seguintes atividades principais: Analisar a base de teste apropriada ao nivel de teste que está sendo utilizado, por exemplo, as especificações de requisitos como RFs e histórias de usuário, épicos, casos de uso; A modelagem e a implementação de informações, como diagramas ou documentos de arquitetura de sistema ou software como diagramas UML; Implementação dos componentes de sistema em si, incluindo o código, metadados e consultas ao banco de dados e interfaces; Relatórios de análise de risco que podem considerar os aspectos funcionais, não funcionais e estruturais do componente ou sistema; Avaliar a base de teste e os itens de teste para identificar vários tipos de defeitos como Ambiguidades, Omissões, Inconsistências, Imprecisões, Contradições, Declarações supérfluas; Identificar os recursos e os conjuntos de recursos a serem testados; Definir e priorizar as condições de teste para cada recurso com base na análise da base de teste e considerando outros fatores como níveis de riscos; Capturar a rastreabilidade bidirecional entre cada elemento da base de teste e as condições de teste associadas.

A aplicação de técnicas de teste caixa-preta, caixa-branca e experiência pode ser útil no processo de análise do teste para reduzir a probabilidade de omitir as condições importantes de teste e difinir as condições de teste mais corretas e precisas.

Em alguns casos a análise produz condições de teste que devem ser usadas como objetivos de teste em cartas de teste. As cartas de teste são típicos produtos de trabalho em alguns tipos de teste baseados na experiência. Quando esses objetivos são rastreáveis até a base de teste, a cobertura obtida durante esses testes baseados na experiência pode ser medida.

A identificação dos defeitos durante a análise do teste é um benefício potencial importante, especialmente quando nenhum outro processo de revisão está sendo usado e/ou o processo de teste está intimamente ligado ao processo de revisão.  A Análise não apenas verifica que os requisitos são consistentes, expressos adequadamente e completos, mas também validam se os requisitos capturam adequadamente as necessidades do cliente, do usuário e stakeholders. 


- Modelagem do teste;

Durante a modelagem de teste, as condições de teste são elaboradas em casos de teste de alto nível, em conjuntos de casos de teste de alto nível e outros testwares. Assim, a análise do teste responde à pergunta "o que testar", enquanto a modelagem de teste responde à pergunta "como testar?".

A modelagem de teste inclui as seguintes atividades principais:

| Lista | Principais atividades da Modelagem de Teste |
| - | - |
| 1 | Projetar e priorizar casos de teste e conjuntos de casos de teste |
| 2 | Identificar os dados de teste necessários para comportar as condições de teste e os casos de teste |
| 3 | Projetar o ambiente de teste e identificar qualquer infraestrutura e ferramenta necessária |
| 4 | Capturar a rastreabilidade bidirecional entre a base de testes, as condições de testes, os casos de teste e os procedimentos de teste |

A elaboração das condições de teste em casos de teste e conjuntos de casos de teste durante a modalagem muitas vezes envolve muitas vezes o uso de técnicas de teste.

Assim como na análise do teste, a modelagem do teste também pode resultar na identificação de tipos semelhantes de defeitos na base de teste. A identificação dos defeitos durante a modelagem do teste é um benefício potencial importante.

- Implementação do teste

Durante a implementação, o testware necessário para a execução do teste é criado ou concluído, incluindo o sequenciamento dos casos de teste nos procedimentos de teste.

A implementação do teste responde a pergunta "agora temos tudo para executar os testes?"

| Lista | Principais atividades da Implementação do Teste |
|-|-|
| 1 | Desenvolver e priorizar procedimentos de teste, e se possível criar scripts de automação |
| 2| Criar as suítes de teste a partir dos procedimentos de teste e os testes automatizados|
|3|Organizar os conjuntos de teste em um cronograma buscando eficiência na execução|
|4|Construir o ambiente de teste (equipamentos, virtualização, simuladores, entre outros itens de infra) e verificar se foi configurado adequadamente|
|5|Preparar os dados de teste e garantir que são carregados corretamente no ambiente de teste|
|6||Verificar a rastreabilidade bidirecional entre a base de teste, as condições de teste, os casos de teste, procedimentos de teste e suítes de teste|

As tarefas do projeto de teste e a implementação de teste são frequentemente combinadas

Nos testes exploratórios e outros tipos de teste baseados na experiência, a modelagem e a implementação podem ocorrer e serem documentadas como parte da execução. Os testes exploratórios podem ser baseados em cartas de teste (produzidas como parte da análise dos testes)

- Execução do teste;

Durante a execução, os conjuntos de testes são executados de acordo com a programação de execução do teste

| Lista | Principais atividades da Execução do Teste |
| - | - |
|1|Gravar os identificadores e versões dos itens de teste ou do objeto de teste, da ferramementa de teste e testware|
|2|Executar os testes manualmente ou usando ferramentas de execução de teste|
|3|Analisar anomalias para estabelecer suas prováveis causas|
|4|Comunicar os defeitos com base nas falhas observadas|
|5|Registrar o resultado da execução do teste (passar, falhar, bloquear)|
|6|Repetir as atividades de teste onde foram identificadas anomalias para verificar correções|
|7|Verificar a rastreabilidade bidirecional entre a base de teste, as condições de teste, os casos de teste, os procedimentos de teste e os resultados de teste|

- Conclusão do teste.

As atividades de conclusão consistem em coletar os dados das atividades de teste já concluidas para consolidar a experiência, o testware e qualquer outra informação relevante. As atividades de conclusão do teste ocorrem nos marcos do projeto, como quando um sistema de software é lançado, um projeto de teste é concluído (ou cancelado), uma iteração do projeto ágil é concluída (como parte de uma reunião retrospectiva por exemplo), um nível de teste ou uma liberação de manutenção é concluída

| Lista | Principais atividades da Conclusão do Teste |
| - | - |
|1|Verificar se todos os relatórios de defeitos estão fechados, inserindo solicitações de mudança ou itens de lista não processada do produto para quaisquer defeitos que não foram resolvidos no final da execução do teste|
|2|Criar um relatório de resumo de teste para ser comunicado aos stakeholders|
|3|Finalizar e arquivar o ambiente de teste, os dados de teste, a infraestrutura de teste e outros testwares para posterior reutilização|
|4|Entragar o testware para as equipes de manutenção ou para alguém que possa se beneficiar do seu uso|
|5|Analisar as lições aprendidas das atividades de teste concluídas para determinar alterações necessárias para futuras iterações, releases e projetos|
|6|Usar as informações coletadas para melhorar a maturidade do processo de teste|

##### (K2) Diferenciar os produtos de trabalho que suportam o processo de teste

1.4.3 Produtos de trabalho do teste

Os produtos de teste podem variar de organização para organização

- Produtos de trabalho do planejamento do teste

Geralmente inclui um ou mais planos de teste. Planos de teste incluem informações sobre a base de teste com as quais os outros produtos de teste serão relacionados através das informações de rastreabilidade, bem como os critérios de saída.

- Produtos de trabalho de monitoramento e controle do teste

Relatórios de progresso do teste, abordando também preocupações de geranciamento de projetos, como conclusão das tarefas, alicação e uso de recursos e o esforço.

- Produtos de trabalho da análise do teste

Condições de teste definidas e priorizadas, preferencialmente onde cada uma das quais é bidirecionalmente rastreável para a base de teste. Para testes exploratórios, a análise do teste pode envolver a criação de cartas de teste. A análise do teste também pode resultar na descoberta e no relato de defeitos na base de teste

- Produtos de trabalho da implementação do teste

| Lista | Produtos de trabalho da implementação do teste |
| - | - |
| 1 | Procedimentos de teste e seu sequenciamento |
| 2 | As suítes de teste |
| 3 | Um cronograma de execução do teste |

A rastreabilidade bidirecional ajuda a demonstrar a obtenção dos critérios de cobertura estabelecidos

Em alguns casos envolve a criação de produtos de trabalho como virtualização de serviços e scripts de teste automatizado

Também pode resultar na criação e verificação dos dados de teste e do ambiente de teste

Os dados de teste servem para atribuirem valores concretos às entradas e aos resultados esperados da execução dos casos de teste. Valore concretos em conjunto com instruções explicitas sobre o uso transformam casos de teste de alto nível em casos de teste executáveis de baixo nível

- Produtos de trabalho da execução do teste

| Lista | Produtos de trabalho da execução do teste |
| - | - |
| 1 | Documentação de status dos casos de teste (Ex: Passed, Failed, Blocked) |
| 2 | Relatórios de defeitos |
| 3 | Documentação sobre quais itens, objetos e ferramentas estavam envolvidas no teste |

Com os produtos do teste e a rastreabilidade bidirecional é possível saber quais itens dos requisitos passaram nos testes e quais falharam, gerando um relato mais compreensível para os stakeholders

- Produto de trabalho de conclusão do teste

Relatórios de resumo de teste, itens de ação para melhoria de projetos subsequentes ou iterações, solicitações de mudança ou itens finalizados de backlog de produto e testware

##### (K2) Explicar o valor de manter a rastreabilidade entre a base de teste e os produtos de trabalho de teste

1.4.4 Rastreabilidade entre a base de teste e os produtos de trabalho de teste

| Lista | A boa rastreabilidade suporta |
| - | - |
| 1 | Avaliação da cobertura de teste |
| 2 | Analisar o impacto das mudanças |
| 3 | Tornar o teste auditável |
| 4 | Atender aos critérios de governança de TI |
| 5 | Melhorar a compreensibilidade dos relatórios de progresso do teste e dos relatórios de resumo do teste pra incluir o status dos elementos da base de teste (Ex: Requisitos que passaram em seus testes, que falharam e que tem testes pendentes) |
| 6 | Relacionar os aspectos técnicos do teste com os stakeholders em termos que eles possam entender |
| 7 | Fornecer informações para avaliar a qualidade do produto, a capacidade do processo e o progresso do projeto em relação às metas de negócios |

Alguns ferramentas de gerenciamento de testes fornecem modelos de produtos de trabalho de teste que correspondem a parte ou a totalidade dos produtos de trabalho de testes descritos no capítulo. Algumas organizações criam os seus próprios sistemas de gerenciamento para organizar os produtos de trabalho


#### 1.5 A psicologia do teste

##### (K1) Identificar os fatores psicológicos que influenciam o sucesso do teste

1.5.1 Psicologia humana e os testes

Um elemento da psicologia humana chamado "viés de confirmação" pode dificultar o aceite das informações que não concordam com as crenças atualmente mantidas. Por exemplo, desenvolvedores esperam que o código esteja correto, eles tem um viés de confirmação que dificulta o aceite do código incorreto. Além disso outros vieses cognitivos podem dificultar que as pessoas entendam ou aceitem informações produzidas por testes, é um traço humano culpar o portador de más notícias.

Devido a esses fatores, algumas pessoas podem perceber o teste como uma atividade destrutiva, embora contribua grandemente para o progresso do projeto e a qualidade do produto. Para reduzir esses efeitos deve-se comunicar defeitos e falhas de maneira construtiva. Dessa forma as tensões entre testadores, analistas e proprietários de produtos, designers e desenvolvedores podem ser reduzidas (isso aplica a testes estáticos e dinâmicos).

Os testadores e gerentes de teste precisam ter boas habilidades interpessoais para se comunicarem de forma eficaz sobre defeitos, falhas, resultados de teste, progresso de testes e riscos, e para construir relacionamentos positivos com os colegas.

| Lista | Maneiras de se comunicar bem |
| - | - |
| 1 | Comece com colaboração em vez de batalhas. Lembre a todos o objetivo comum de sistemas de melhor qualidade |
| 2 | Enfatize os beneficios do teste. Informações sobre defeitos podem ajudar a melhorar os produtos de trabalho dos autores, para a organização reduz tempo e dinheiro gasto e o risco geral à qualidade do produto |
| 3 | Comunique os resultados dos testes de maneira neutra, focada no fato e sem criticar a pessoa que criou o item com defeito. Escreva relatórios de defeitos objetivos e factuais e revise os resultados |
| 4 | Tente entender como a outra pessoa se sente e as razões pelas quais ela pode reagir negativamente à informação |
| 5 | Confirme se a outra pessoa entendeu o que foi dito e vice-versa |


##### (K2) Explicar a diferença entre a mentalidade necessária para as atividades de teste e a mentalidade necessária para atividades de desenvolvimento

1.5.2 A mentalidade do testador e do desenvolvedor

A mentalidade de um testador e de um desenvolvedor é diferente, reunir as duas ajuda a alcançar um nível mais alto de qualidade do produto

A mentalidade de testador inclui curiosidade, pessimismo profissional, olho crítico, atenção aos detalhes e motivação para comunicações e relacionamentos bons e positivos. A mentalidade de um testador tende a crescer e amadurecer a medida que o testador ganha experiência

A mentalidade de um desenvolvedor inclui alguns dos elementos da mentalidade de um testador, mas geralmente estão mais interessados em projetar e criar soluções do que em contemplar o que pode estar errado nessas soluções. Além disso, o viés de confirmação torna dificil encontrar erros em seu próprio trabalho

Com a mentalidade certa, os devs podem testar seu próprio código. Diferentes modelos de ciclo de vida de desenvolvimento de software geralmente têm maneiras diferentes de organizar os testadores e as atividades de teste. Ter algumas atividades do teste feitas por testadores independentes aumenta a eficácia da detecção de defeitos, o que é particularmente para sistemas grandes, complexos ou de segurança crítica. Testadores independentes trazem uma perspectiva diferente, uma vez que possuem vieses cognitivos diferentes dos autores

----

## Capítulo 2 - Teste durante o ciclo de vida de desenvolvimento de software

#### 2.1 Modelos de ciclo de vida de desenvolvimento de software

##### (K2) Explicar as relações entre as atividades de desenvolvimento de software e as atividades de teste no ciclo de vida de desenvolvimento de software

##### (K1) Identificar os motivos pelos quais os modelos de ciclo de vida de desenvolvimento de software devem ser adaptados ao contexto das características do projeto e do produto


#### 2.2 Níveis de teste

##### (K2) Comparar os diferentes níveis de teste na perspectiva de seus objetivos, na base de teste nos artefatos de teste, nas falhas e defeitos típicos e nas abordagens e responsabilidades

#### 2.3 Tipos de teste

##### (K2) Comparar os testes funcionais dos não-funcionais e caixa-branca

##### (K1) Reconhecer que os testes funcionais, não funcionais e caixa-branca ocorrem em qualquer nível de teste

#### 2.4 Teste de manutenção

##### (K2) Resumir os gatilhos para o teste de manutenção

##### (K2) Descrever o papel da análise de impacto no teste de manutenção