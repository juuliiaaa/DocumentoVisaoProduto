# Rastreador de Fitness (FitTrack)

## 1. Visão Geral do Produto

###### 1.1 Declaração do Problema e Oportunidade de Negócio
Atualmente, muitas pessoas buscam melhorar sua saúde e qualidade de vida através da prática regular de atividades físicas. Entretanto, acompanhar o progresso dessas atividades pode ser difícil, pois o registro manual de exercícios costuma ser trabalhoso e pouco motivador.

Muitos praticantes de exercícios acabam abandonando o acompanhamento de suas atividades por falta de ferramentas simples que permitam registrar treinos, visualizar evolução e manter a motivação ao longo do tempo.

Além disso, academias e grupos esportivos frequentemente não possuem ferramentas digitais simples para acompanhar o desempenho coletivo de seus membros.

Nesse contexto, surge a oportunidade de desenvolver uma plataforma digital que facilite o registro de atividades físicas, o acompanhamento do progresso e a criação de desafios entre usuários.

O FitTrack busca atender essa necessidade oferecendo um sistema que permite registrar atividades físicas, definir metas pessoais e visualizar estatísticas de desempenho. Dessa forma, o sistema contribui para incentivar hábitos saudáveis e aumentar o engajamento dos usuários com a prática de exercícios.

Além dos benefícios individuais para os usuários, a solução também pode trazer vantagens para academias e grupos esportivos, que poderão acompanhar o progresso de seus alunos e promover desafios motivacionais.

###### 1.2 Perspectiva do Produto
O FitTrack é um aplicativo de rastreamento de atividades físicas voltado para pessoas que desejam acompanhar sua evolução em exercícios como caminhada, corrida, ciclismo e musculação.

O sistema se insere no contexto de aplicativos de saúde e bem-estar, semelhantes a outras plataformas de monitoramento de atividades físicas disponíveis no mercado. No entanto, o FitTrack se diferencia ao permitir a criação de grupos e academias, possibilitando desafios coletivos e acompanhamento de desempenho entre membros.

O público-alvo do sistema inclui:

Pessoas que praticam atividades físicas regularmente

Usuários iniciantes que desejam melhorar sua saúde

Academias e grupos de treino

Comunidades esportivas

A proposta de valor do FitTrack está em oferecer uma plataforma simples e acessível para registrar atividades físicas, acompanhar progresso e incentivar a prática de exercícios por meio de estatísticas e desafios entre usuários.

###### 1.3 Capacidades do Produto
O sistema FitTrack oferecerá um conjunto de funcionalidades voltadas ao monitoramento e incentivo à prática de atividades físicas.

Funcionalidades:
* Registro de atividades físicas como caminhada, corrida, ciclismo e musculação
* Definição de metas pessoais de distância, tempo ou calorias
* Visualização de estatísticas e gráficos de progresso
* Participação em desafios e competições entre usuários
* Compartilhamento de resultados com amigos
* Registro de histórico completo de atividades
* Notificações e lembretes para incentivar a prática de exercícios

###### Fluxograma - Cadastro
![Cadastro](./cadastro.svg)


###### Fluxograma - Visualizar Estatística
![Visualizar Estatísticas](./visualizarEstatistica.svg)


Características de qualidade

O sistema deve garantir uma boa experiência para os usuários. A interface precisa ser simples e fácil de usar, permitindo o registro rápido das atividades. Também é importante garantir a segurança dos dados, de forma que cada usuário tenha acesso apenas às suas próprias informações. Além disso, os dados registrados devem ser armazenados de forma confiável, e o sistema deve ser desenvolvido de maneira organizada para facilitar futuras melhorias e atualizações.

## 2. Definição de usuários
| Atributo              | Descrição                                                                                                                                                         |
| --------------------- |:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| Usuário ID            | USER-001                                                                                                                                                                                    |
| Nome do Perfil        | Atleta                                                                                                                                                            |
| Descrição             | O usuário utiliza o sistema para registrar exercícios, acompanhar seu progresso e participar de desafios. treinos e metas.                                        |
| Experiência Técnica   | Baixa a média; acostumado ao uso de aplicativos móveis para saúde e redes sociais.                                                                                |
| Frequência de Uso     | Alta                                                                                                                                                              |
| Principais Objetivos  | Registrar atividades físicas, acompanhar evolução e atingir metas                                                                                                 |
| Desafios              | Registrar dados de forma rápida e manter a motivação.                                                                                                             |
| Restrições            | Acessa apenas seus próprios dados e os desafios nos quais está participando.                                                                                      |
| Requisitos Principais | Registro de atividades, metas pessoais, visualização de gráficos                                                                                                  |

| Atributo              | Descrição                                                                                                                                                         |
| --------------------- |:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| Usuário ID            | USER-002                                                                                                                                                          |
| Nome do Perfil        | Administrador da Academia                                                                                                                                         |
| Descrição             | Responsável pela gestão dos membros e criação de desafios.                                                                                                        |
| Experiência Técnica   | Média; Capaz de operar dashboards de gestão.                                                                                                                      |
| Frequência de Uso     | Regularmente, para monitorar relatórios e criar eventos.                                                                                                          |
| Principais Objetivos  | Gerenciar membros, criar desafios e acompanhar progresso coletivo                                                                                                 |
| Desafios              | Garantir que os alunos estejam ativos na plataforma.                                                                                                              |
| Restrições            | Gerencia apenas sua própria academia e seus membros.                                                                                                              |
| Requisitos Principais | Painel de gestão de membros, criação de desafios, relatórios de atividades do grupo, envio de mensagens de motivação.                                             |


## 3. Restrições do Projeto e do Produto

| Campo                                | Descrição                                                                                                                                          |
| ------------------------------------ |:--------------------------------------------------------------------------------------------------------------------------------------------------:|
| Restrição ID                         | NF-CONST-001                                                                                                                                       |
| Título                               | Restrições Tecnológicas                                                                                                                            |
| Descrição                            | O sistema deve integrar-se com serviços de mapas e dispositivos fitness.                                                                           |
| Origem                               | Equipe de arquitetura                                                                                                                              |
| Critérios de verificação e validação | Testes de API com dispositivos e serviços de GPS.                                                                                                  |
| Relacionamento com outros requisitos | RF03 (registro de atividades), RF06 (gráficos), RF10 (notificações)                                                                                |

| Campo                                | Descrição                                                                                                                                          |
| ------------------------------------ |:--------------------------------------------------------------------------------------------------------------------------------------------------:|
| Restrição ID                         | NF-CONST-002                                                                                                                                       |
| Título                               | Restrições de Prazo e Recursos                                                                                                                     |
| Descrição                            | O projeto é desenvolvido no contexto acadêmico com equipe reduzida e prazo semestral.                                                              |
| Origem                               | Disciplina acadêmica                                                                                                                               |
| Critérios de verificação e validação | Entrega das etapas do projeto conforme os prazos estabelecidos                                                                                     |
| Relacionamento com outros requisitos | Todos os RFs                                                                                                                                       |

| Campo                                | Descrição                                                                                                                                          |
| ------------------------------------ |:--------------------------------------------------------------------------------------------------------------------------------------------------:|
| Restrição ID                         | NF-CONST-003                                                                                                                                       |
| Título                               | Restrições de Segurança e Privacidade                                                                                                              |
| Descrição                            | O sistema deve implementar autenticação por usuário e senha com políticas mínimas de segurança. O acesso aos dados deve ser isolado por usuário e por academia. O tratamento de dados pessoais deve estar em conformidade com a LGPD                                                                                                              |
| Origem                               | Legislação de Privacidade / LGPD                                                                                                                   |
| Critérios de verificação e validação | Testes de penetração básicos; revisão de conformidade com LGPD antes do lançamento; isolamento de dados validado por testes de autorização.        |
| Relacionamento com outros requisitos | RF01, RF02 (cadastros), RF09 (histórico de atividades)                                                                                             |


## 4. Análise de Riscos e Mitigação

| Campo                  | Descrição                                                                                                                                                        |
| ---------------------- |:----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| ID do Risco            | RISCO-001                                                                                                                                                        |
| Descrição              | Usuários abandonarem o app por falta de engajamento a longo prazo.                                                                                               |
| Categoria              | Externo                                                                                                                                                          |
| Probabilidade          | Alta                                                                                                                                                             |
| Impacto                | Alto                                                                                                                                                             |
| Ação de Mitigação      | Implementar desafios, metas e notificações motivacionais                                                                                                         |
| Plano de Contingência  | Criar novos recursos de engajamento, como recompensas.                                                                                                           |

| Campo                  | Descrição                                                                                                                                                        |
| ---------------------- |:----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| ID do Risco            | RISCO-002                                                                                                                                                        |
| Descrição              | Usuários podem inserir dados incorretos ou exagerados nas atividades                                                                                             |
| Categoria              | Técnico                                                                                                                                                          |
| Probabilidade          | Média                                                                                                                                                            |
| Impacto                | Médio                                                                                                                                                            |
| Ação de Mitigação      | Implementar validações básicas e limites plausíveis de atividade                                                                                                 |
| Plano de Contingência  | Permitir edição ou revisão manual dos dados registrados                                                                                                          |

| Campo                  | Descrição                                                                                                                                                        |
| ---------------------- |:----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| ID do Risco            | RISCO-003                                                                                                                                                        |
| Descrição              | Cada fabricante de smartwatch e pulseira fitness utiliza formatos de dados proprietários, tornando a padronização da importação tecnicamente complexa e custosa. |
| Categoria              | Técnico                                                                                                                                                          |
| Probabilidade          | Alta                                                                                                                                                             |
| Impacto                | Médio                                                                                                                                                            |
| Ação de Mitigação      | Criar uma camada de padronização para importar dados                                                                                                             |
| Plano de Contingência  | Permitir inserção manual de atividades                                                                                                                           |