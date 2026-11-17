## **1. Introdução**
O SENTINELA é uma proposta de plataforma inteligente de monitoramento, centralização de dados e detecção de anomalias em ambientes críticos.

A solução tem como finalidade integrar informações provenientes de diferentes fontes de monitoramento, como câmeras, sensores e sistemas de controle de acesso, permitindo identificar eventos fora dos padrões estabelecidos e apresentar alertas contextualizados aos operadores.

O projeto propõe a utilização de tecnologias como Internet das Coisas (IoT), visão computacional, processamento de dados e mecanismos de correlação de eventos para apoiar o acompanhamento de ocorrências e a tomada de decisão humana.

Nesta primeira etapa, será desenvolvido um protótipo acadêmico utilizando dados simulados e arquivos demonstrativos, sem conexão com equipamentos ou instalações reais.

## **2. Contexto do Problema/**
Ambientes críticos exigem monitoramento contínuo e análise de informações provenientes de diferentes fontes. Entretanto, quando esses dados são apresentados de maneira isolada, torna-se mais difícil identificar relações entre eventos, reconhecer comportamentos fora do padrão e acompanhar ocorrências de forma centralizada.

Por exemplo, uma abertura inesperada de acesso pode parecer um evento isolado. Porém, quando relacionada a uma detecção de movimento em uma área restrita e a informações de sensores próximos, pode representar uma situação que merece investigação.

A ausência de centralização e correlação dessas informações pode dificultar a identificação de situações anormais, aumentar o tempo de análise e prejudicar a rastreabilidade das ocorrências.

Diante desse cenário, o SENTINELA propõe uma plataforma capaz de reunir dados de diferentes fontes, analisar eventos e apresentar alertas com informações relevantes para avaliação dos operadores.

## **3. Objetivos da Solução**
## **3.1 Objetivo geral**
Desenvolver uma plataforma de monitoramento inteligente capaz de centralizar dados simulados de diferentes fontes, identificar anomalias e correlacionar eventos para gerar alertas contextualizados e apoiar a tomada de decisão humana em ambientes críticos.

## **3.2 Objetivos específicos**
- Centralizar informações provenientes de diferentes dispositivos e fontes de monitoramento.
- Simular o recebimento de dados de sensores e equipamentos.
- Analisar imagens e vídeos demonstrativos por meio de visão computacional.
- Identificar eventos que estejam fora de padrões previamente definidos.
- Correlacionar ocorrências considerando horário, localização e tipo de evento.
- Gerar alertas com informações sobre origem, horário, localização e evidências.
- Permitir que operadores analisem, confirmem ou descartem alertas.
- Registrar ocorrências e decisões para consulta e auditoria.


## **4. Stakeholders**

Os stakeholders do projeto Sentinela correspondem aos perfis de pessoas e grupos que possuem interesse, participação ou influência no funcionamento da solução proposta.

| Stakeholder | Descrição | Responsabilidades | Necessidades | Nível de influência |
|---|---|---|---|---|
| Operador de monitoramento | Profissional que acompanha as informações apresentadas pela plataforma. | Monitorar eventos, analisar alertas e registrar decisões. | Alertas contextualizados, evidências visuais, localização e histórico. | Alto |
| Supervisor de segurança | Profissional que supervisiona as atividades de monitoramento. | Acompanhar ocorrências, avaliar prioridades e supervisionar decisões. | Indicadores, relatórios e acompanhamento de alertas. | Alto |
| Administrador do sistema | Responsável pela configuração e manutenção técnica da plataforma. | Gerenciar dispositivos, usuários e regras de detecção. | Acesso administrativo, configuração e estabilidade. | Médio |
| Equipe de manutenção e inspeção | Profissionais que verificam equipamentos e instalações quando necessário. | Verificar ocorrências relevantes e realizar inspeções. | Localização, horário e evidências das ocorrências. | Médio |
| Gestão da organização | Representa os responsáveis pela gestão estratégica e operacional. | Avaliar resultados e acompanhar indicadores. | Rastreabilidade, relatórios e visão consolidada. | Alto |



## **5. Requisitos do Sistema**
## **5.1 Requisitos funcionais**

Os requisitos funcionais descrevem as funcionalidades que o sistema deverá disponibilizar aos seus usuários.

| ID | Requisito | Descrição |
|---|---|---|
| RF01 | Centralização de dados | O sistema deve centralizar informações provenientes de diferentes fontes simuladas de monitoramento. |
| RF02 | Simulação de dispositivos | O sistema deve permitir a geração de eventos fictícios de sensores e dispositivos. |
| RF03 | Análise visual | O sistema deve analisar imagens e vídeos demonstrativos para identificar objetos de interesse. |
| RF04 | Detecção de anomalias | O sistema deve identificar eventos que estejam fora dos parâmetros e regras configurados. |
| RF05 | Correlação de eventos | O sistema deve relacionar ocorrências com base em horário, localização e tipo de evento. |
| RF06 | Geração de alertas | O sistema deve gerar alertas contextualizados para eventos identificados como anômalos. |
| RF07 | Gerenciamento de alertas | O sistema deve permitir que o operador analise, confirme ou descarte alertas. |
| RF08 | Histórico de ocorrências | O sistema deve armazenar as ocorrências identificadas e as decisões dos operadores. |
| RF09 | Visualização de monitoramento | O sistema deve apresentar indicadores e informações consolidadas em um dashboard. |

## **5.2 Requisitos Não Funcionais**

Os requisitos não funcionais estabelecem características de qualidade, desempenho, segurança e utilização esperadas para o sistema.

| ID | Requisito | Descrição |
|---|---|---|
| RNF01 | Usabilidade | A interface deve apresentar informações de maneira clara e organizada, facilitando a compreensão e a utilização pelos operadores. |
| RNF02 | Desempenho | O sistema deve processar eventos simulados e apresentar os alertas correspondentes em até 5 segundos após o recebimento do evento, considerando as condições do ambiente de demonstração. |
| RNF03 | Segurança | O acesso às funcionalidades administrativas deve exigir autenticação, restringindo sua utilização a usuários autorizados. |
| RNF04 | Rastreabilidade | O sistema deve manter registros das ocorrências e das decisões realizadas pelos operadores, permitindo consultas posteriores. |
| RNF05 | Manutenibilidade | A arquitetura deve permitir alterações e inclusão de novas fontes de dados e regras de detecção sem exigir modificações significativas em toda a aplicação. |
| RNF06 | Confiabilidade | O sistema deve identificar e tratar entradas inválidas e falhas de processamento sem interromper o processamento dos demais eventos recebidos. |

## **6. Proposta de Solução**
O SENTINELA propõe uma aplicação web que centraliza informações de diferentes fontes de monitoramento e utiliza mecanismos de análise para identificar possíveis anomalias.

A solução será organizada em módulos:
- Dashboard: apresenta indicadores gerais, dispositivos monitorados e eventos recentes.
- Simulador de dispositivos: gera dados fictícios de sensores, câmeras e outros equipamentos.
- Análise visual: utiliza visão computacional para analisar imagens e vídeos demonstrativos.
- Detecção de anomalias: aplica regras e parâmetros para identificar eventos fora do padrão.
- Correlação de eventos: relaciona ocorrências por horário, localização e contexto.
- Central de alertas: apresenta ocorrências identificadas para análise dos operadores.
- Histórico e auditoria: armazena eventos, classificações e decisões realizadas.
A detecção será realizada de acordo com a natureza dos dados. Valores de sensores poderão ser analisados por regras e limites configurados, enquanto imagens e vídeos poderão ser processados por técnicas de visão computacional.

A correlação permitirá relacionar eventos que, individualmente, poderiam parecer comuns, mas que, quando analisados em conjunto, podem indicar uma situação que merece atenção.

A plataforma funcionará como ferramenta de apoio à decisão. A confirmação ou o descarte de uma ocorrência permanecerá sob responsabilidade do operador.

## **7. Arquitetura Conceitual e Funcionamento**
A arquitetura proposta segue um fluxo de recebimento, análise, correlação e apresentação de eventos.
Fluxo conceitual:
1. Dispositivos simulados geram eventos e informações.
2. A plataforma recebe e centraliza os dados.
3. Os dados são encaminhados para os mecanismos de análise correspondentes.
4. Eventos fora dos padrões definidos são identificados.
5. O sistema verifica a existência de eventos relacionados.
6. Os eventos são correlacionados por horário, localização e contexto.
7. A plataforma gera um alerta contextualizado.
8. O operador analisa a ocorrência e confirma ou descarta o alerta.
9. O resultado é registrado no histórico para consulta e auditoria.
A arquitetura poderá utilizar tecnologias como React, Python, FastAPI, OpenCV, YOLO e PostgreSQL. Essas tecnologias representam opções iniciais e poderão ser ajustadas durante o desenvolvimento.


##  **8. Escopo do Projeto**
## ** 8.1 Dentro do escopo**
- Desenvolvimento de uma aplicação web.
- Dashboard para visualização de indicadores.
- Simulação de sensores e dispositivos.
- Análise de imagens e vídeos demonstrativos.
- Detecção de objetos por visão computacional.
- Identificação de anomalias por regras configuráveis.
- Correlação básica de eventos.
- Geração e classificação de alertas.
- Visualização de localização simulada dos dispositivos e ocorrências.
- Registro de histórico e decisões dos operadores.


## **8.2 Fora do escopo**
- Controle físico de drones ou voos autônomos.
- Instalação de sensores em ambientes reais.
- Integração com sistemas operacionais da AMAZUL ou da Marinha.
- Reconhecimento facial ou identificação biométrica.
- Detecção ou diagnóstico de radiação.
- Execução automática de respostas físicas a incidentes.
- Substituição dos profissionais responsáveis pela segurança.
- Certificação para utilização em instalações nucleares.

##** 8.3 Limitações**
O SENTINELA será desenvolvido como um projeto acadêmico demonstrativo. Portanto, utilizará dados simulados e arquivos de demonstração, sem representar uma solução validada ou certificada para operação em ambientes nucleares reais.


## **9. Benefícios Esperados**
A implementação do SENTINELA poderá proporcionar os seguintes benefícios conceituais:
- Centralização: reunir informações de diferentes fontes em uma única plataforma.
- Identificação de anomalias: facilitar a identificação de eventos fora dos padrões definidos.
- Correlação de eventos: permitir a análise conjunta de ocorrências relacionadas.
- Agilidade operacional: apresentar alertas com informações relevantes para análise.
- Apoio à decisão: fornecer contexto e evidências para os operadores.
- Rastreabilidade: manter registros de eventos e decisões.
- Expansibilidade: permitir a inclusão futura de novas fontes de dados e mecanismos de análise.

## **10. Protótipo Conceitual**
O protótipo de baixa fidelidade foi desenvolvido no Figma com o objetivo de representar a organização das principais funcionalidades e a experiência de utilização da plataforma.

Ele é composto por quatro telas principais:

## **10.1 Dashboard**
Apresenta indicadores gerais, estado dos dispositivos monitorados e eventos recentes.
<img width="940" height="605" alt="Dashboard" src="https://github.com/user-attachments/assets/4d98074a-46af-47c9-8d9c-3d222577b941" />

## **10.2 Mapa de Monitoramento**
Representa a instalação fictícia, suas zonas e a localização simulada dos dispositivos.
<img width="932" height="608" alt="Mapa" src="https://github.com/user-attachments/assets/3ad3d31f-86da-478e-925f-cef5a3c18e44" /> 

## **10.3 Central de Alertas**
Apresenta ocorrências identificadas, prioridade, evidências e ações de confirmação ou descarte.
<img width="933" height="620" alt="Alertas" src="https://github.com/user-attachments/assets/8adae0fd-29eb-4c1a-94eb-d9bc7c8702f7" />

## **10.4 Histórico e Auditoria**
Permite consultar ocorrências anteriores, decisões dos operadores e informações registradas.
<img width="893" height="566" alt="Histórico" src="https://github.com/user-attachments/assets/6009a9c4-a474-47ad-8840-8c5018521a0c" />

As imagens definitivas desta seção devem ser capturas das quatro telas que você construiu no Figma, não imagens ilustrativas. Inclua também uma breve legenda para cada captura.

## **11. Conclusão**
O projeto SENTINELA apresenta uma proposta de solução tecnológica voltada à centralização de informações, detecção de anomalias e correlação de eventos em ambientes críticos.

A partir da identificação dos desafios relacionados à fragmentação de dados e à análise isolada de diferentes fontes de monitoramento, foi definida uma plataforma capaz de organizar informações, identificar possíveis situações anormais e apresentar alertas contextualizados para apoiar a atuação dos operadores.

A definição dos stakeholders, requisitos funcionais e não funcionais, escopo e arquitetura conceitual estabelece uma base para o desenvolvimento das próximas etapas do projeto.

O protótipo conceitual demonstra como as principais funcionalidades poderão ser organizadas em uma interface web, contemplando o acompanhamento de dispositivos, a visualização de alertas e a consulta ao histórico de ocorrências.

Por se tratar de um projeto acadêmico, a validação inicial será realizada com dados simulados e arquivos demonstrativos, não representando uma solução certificada ou pronta para utilização em instalações reais.

Assim, o SENTINELA busca demonstrar como a integração de diferentes fontes de informação, associada a mecanismos de análise e correlação de eventos, pode contribuir para um monitoramento mais organizado e para o apoio à tomada de decisão humana.
