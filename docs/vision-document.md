##  **1. Contexto do Problema**
Ambientes críticos exitgem monitoramento cntínuo, capacidade de identificar situação anormais e acompanhamento adequado de ocorrências que possam comprometer a segurança e a integridade operacional.

Para isso, diferentes fontes de monitoramento, como câmeras, sensores ambientais , dispositivos de controle de acesso e sistemas de inspeção, podem gerar informações relevantes sobre as condições e atividades desses ambientes.

Entretanto, a utilização de múltiplas fontes de informação apresenta desafios relacoonados à fragmentação dos dados, à identificação de anomalias e à correlação de eventos. Informações provenientes de dispositivos distintos podem ser analisadas separadamente, dificultando a contrução de uma visão abrangente e contextualizada de determinadas situações.

Além disso, a identificação deeventos fora dos padrões estabelecidos e a associação entre as ocorrências relacionadas podem exigir reforço significativo dos operadores responsáveis pelo monitoramento, especialemente quando há grande volume de informações a serem analisadas.

Diante desse cenário, identifica-se a necessidade de uma solução capaz de centralizar dados de diferentes fontes, detectar automaticamente eventos que apresentam comportamentos fora dos parâmetros definifos e correlacionar ocorrências com base em critérios como horário, localização, tipo de evento e origem da informação.

O projeto Sentinela surge como uma proposta de plataforma inteligente de monitoramento e detecção de anomalias, com o objetivo de transformar dados dispersos em informações organizadas e alertas contextualizados, apoiando a análise e a tomada de decisão dos operadores humanos. 


## **Stakeholders**

Os stakeholders do projeto Sentinela correspondem aos perfis de pessoas e grupos que possuem interesse, participação ou influência no funcionamento da solução proposta.

| Stakeholder | Descrição | Responsabilidades | Necessidades | Nível de influência |
|---|---|---|---|---|
| Operador de monitoramento | Profissional que acompanha as informações apresentadas pela plataforma. | Monitorar eventos, analisar alertas e registrar decisões. | Alertas contextualizados, evidências visuais, localização e histórico. | Alto |
| Supervisor de segurança | Profissional que supervisiona as atividades de monitoramento. | Acompanhar ocorrências, avaliar prioridades e supervisionar decisões. | Indicadores, relatórios e acompanhamento de alertas. | Alto |
| Administrador do sistema | Responsável pela configuração e manutenção técnica da plataforma. | Gerenciar dispositivos, usuários e regras de detecção. | Acesso administrativo, configuração e estabilidade. | Médio |
| Equipe de manutenção e inspeção | Profissionais que verificam equipamentos e instalações quando necessário. | Verificar ocorrências relevantes e realizar inspeções. | Localização, horário e evidências das ocorrências. | Médio |
| Gestão da organização | Representa os responsáveis pela gestão estratégica e operacional. | Avaliar resultados e acompanhar indicadores. | Rastreabilidade, relatórios e visão consolidada. | Alto |



## **Requisitos Funcionais**

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

## **Requisitos Não Funcionais**

Os requisitos não funcionais estabelecem características de qualidade, desempenho, segurança e utilização esperadas para o sistema.

| ID | Requisito | Descrição |
|---|---|---|
| RNF01 | Usabilidade | A interface deve apresentar informações de maneira clara e organizada. |
| RNF02 | Desempenho | O sistema deve processar os eventos simulados e apresentar os resultados em tempo adequado para a demonstração. |
| RNF03 | Segurança | O acesso às funcionalidades administrativas deve ser controlado. |
| RNF04 | Rastreabilidade | O sistema deve manter registros das ocorrências e das decisões realizadas pelos operadores. |
| RNF05 | Manutenibilidade | A arquitetura deve permitir alterações e inclusão de novas fontes de dados e regras de detecção. |
| RNF06 | Confiabilidade | O sistema deve tratar entradas inválidas e falhas de processamento sem comprometer o funcionamento geral do protótipo. |


## **Escopo do Projeto**

O projeto Sentinela contempla o desenvolvimento de um protótipo acadêmico de uma plataforma web para centralização de dados, detecção de anomalias e correlação de eventos em ambientes críticos. A validação da solução será realizada por meio de dados simulados e arquivos demonstrativos, sem necessidade de equipamentos ou instalações reais.

### **Dentro do Escopo**

- Desenvolvimento de uma aplicação web para monitoramento.
- Criação de um dashboard com indicadores e status dos dispositivos.
- Simulação de dados provenientes de sensores e dispositivos de monitoramento.
- Análise de imagens e vídeos demonstrativos utilizando visão computacional.
- Detecção de anomalias por meio de regras e parâmetros configuráveis.
- Correlação de eventos considerando horário, localização e tipo de ocorrência.
- Geração de alertas contextualizados.
- Visualização de evidências e localização simulada das ocorrências.
- Possibilidade de confirmação ou descarte de alertas pelo operador.
- Registro do histórico de ocorrências e das decisões realizadas.

### **Fora do Escopo**

- Instalação e operação de sensores físicos em ambientes reais.
- Controle de drones físicos ou execução de voos autônomos.
- Integração com sistemas reais da AMAZUL ou da Marinha do Brasil.
- Reconhecimento biométrico ou identificação facial.
- Detecção ou diagnóstico de radiação por equipamentos reais.
- Execução automática de ações físicas em resposta aos alertas.
- Substituição da atuação dos profissionais responsáveis pela segurança.
- Certificação ou homologação para utilização em instalações nucleares reais.

### **Limitações do Protótipo**

Por se tratar de um projeto acadêmico, o Sentinela utilizará dados fictícios e arquivos demonstrativos para simular situações de monitoramento. Dessa forma, os resultados obtidos terão finalidade exclusivamente demonstrativa e não representarão validação operacional em ambientes críticos reais.


## **Benefícios Esperados**

O desenvolvimento do Sentinela busca proporcionar melhorias no monitoramento e na análise de informações provenientes de diferentes fontes, contribuindo para uma identificação mais organizada e contextualizada de possíveis anomalias em ambientes críticos.

Entre os principais benefícios esperados, destacam-se:

- **Centralização das informações:** reunir dados provenientes de diferentes fontes de monitoramento em uma única plataforma, facilitando o acesso e a visualização das informações.

- **Identificação de anomalias:** utilizar regras configuráveis e técnicas de visão computacional para identificar eventos que apresentem comportamentos fora dos padrões estabelecidos.

- **Correlação de eventos:** relacionar ocorrências com base em horário, localização e tipo de evento, permitindo uma análise mais abrangente das situações identificadas.

- **Agilidade na análise:** apresentar alertas contextualizados com informações relevantes e evidências, reduzindo o esforço necessário para compreender determinadas ocorrências.

- **Apoio à tomada de decisão:** disponibilizar informações organizadas para que os operadores possam avaliar os alertas e decidir sobre as ações necessárias.

- **Rastreabilidade das ocorrências:** manter registros históricos dos eventos identificados e das decisões dos operadores, facilitando consultas e análises posteriores.

- **Flexibilidade e expansão:** estabelecer uma estrutura que permita, futuramente, incorporar novas fontes de dados, dispositivos e mecanismos de análise.

Dessa forma, o Sentinela pretende transformar informações dispersas em dados organizados e contextualizados, contribuindo para um monitoramento mais integrado e para o apoio à tomada de decisão humana.
