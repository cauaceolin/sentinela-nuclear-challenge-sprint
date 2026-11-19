Plano de Testes — SENTINELA
Projeto: SENTINELA — AMAZUL Sprint 1
Disciplina: Software Engineering
Instituição: FIAP
Versão: 1.0
Data: 20 de Novembro de 2026

## **1. Objetivo**
Este documento define o planejamento dos testes do SENTINELA, uma aplicação web demonstrativa destinada à centralização de dados simulados de monitoramento, identificação de eventos fora dos padrões configurados e correlação de ocorrências para gerar alertas contextualizados que apoiem a análise humana.

Os testes têm como finalidade verificar se as funcionalidades previstas atendem aos requisitos definidos no Documento de Visão.

## **2. Escopo dos testes**
O planejamento contempla as seguintes funcionalidades:
- Centralização de dados simulados provenientes de diferentes fontes.
- Simulação de eventos gerados por sensores e dispositivos.
- Análise de imagens e vídeos demonstrativos para identificação de objetos de interesse.
- Detecção de anomalias com base em regras e parâmetros configurados.
- Correlação de eventos por horário, localização e tipo.
- Geração de alertas com informações contextuais.
- Análise, confirmação ou descarte de alertas pelo operador.
- Armazenamento de ocorrências e decisões.
- Exibição de indicadores e informações consolidadas em um painel.
Os testes serão realizados em ambiente acadêmico e demonstrativo, utilizando dados simulados e arquivos de demonstração. Não haverá integração com equipamentos ou instalações reais.

## **3. Estratégia de testes**
Os testes serão planejados com base nos requisitos funcionais (RF01 a RF09) e não funcionais (RNF01 a RNF06) do Documento de Visão.

Serão considerados:
- Testes funcionais: verificam se cada funcionalidade apresenta o comportamento esperado.
- Testes não funcionais: verificam aspectos de usabilidade, desempenho, autenticação, rastreabilidade, extensibilidade e tratamento de falhas.
- Testes de integração: verificam a troca e o relacionamento de informações entre os módulos da aplicação.
Os casos abaixo representam cenários planejados. Sua inclusão neste documento não significa que já tenham sido executados.

## **4. Casos de testes funcionais**
ID	Requisito	Cenário planejado	Resultado esperado
CT01	RF01	Enviar dados simulados provenientes de diferentes fontes.	Os dados são recebidos e apresentados de forma centralizada.
CT02	RF02	Gerar um evento por meio do simulador de dispositivos.	O evento simulado é recebido e registrado corretamente.
CT03	RF03	Submeter uma imagem ou vídeo demonstrativo para análise.	O sistema processa o arquivo e identifica objetos de interesse, conforme a capacidade implementada.
CT04	RF04	Enviar um valor ou evento que ultrapasse uma regra ou parâmetro configurado.	O sistema identifica o desvio e o classifica como possível anomalia.
CT05	RF05	Enviar eventos relacionados por horário, localização ou tipo.	O sistema relaciona os eventos conforme os critérios de correlação implementados.
CT06	RF06	Gerar uma ocorrência identificada como potencialmente anômala.	O sistema apresenta um alerta com as informações contextuais disponíveis, como origem, horário e localização.
CT07	RF07	O operador analisar um alerta e confirmar ou descartar a ocorrência.	A decisão selecionada pelo operador é registrada e refletida no estado do alerta.
CT08	RF08	Consultar uma ocorrência após o registro de uma decisão.	O histórico apresenta a ocorrência e a decisão correspondente.
CT09	RF09	Acessar o dashboard após a geração de eventos e alertas.	O painel apresenta indicadores e informações consolidadas disponíveis.


## **5. Casos de testes não funcionais**
ID	Requisito	Cenário planejado	Resultado esperado
TNF01	RNF01	Avaliar a navegação e a compreensão das telas por um usuário.	A interface apresenta informações de forma clara e facilita a utilização.
TNF02	RNF02	Medir o intervalo entre o recebimento de um evento simulado e a geração do alerta correspondente.	O alerta é gerado em até 5 segundos, desconsiderando o processamento de arquivos de vídeo.
TNF03	RNF03	Tentar acessar funcionalidades administrativas sem autenticação.	O acesso às funcionalidades administrativas é bloqueado para usuários não autenticados.
TNF04	RNF04	Registrar uma ocorrência e uma decisão do operador e consultar os registros.	As informações permanecem disponíveis para consulta e rastreabilidade.
TNF05	RNF05	Avaliar a inclusão de uma nova fonte de dados ou regra de detecção.	A estrutura permite a extensão sem exigir alterações extensas.
TNF06	RNF06	Enviar uma entrada inválida ou provocar uma falha pontual durante o recebimento de eventos.	A entrada inválida ou falha é tratada sem interromper o processamento dos demais eventos.


## **6. Critérios de aprovação**
Um caso de teste será considerado aprovado quando o comportamento observado corresponder ao resultado esperado definido para aquele cenário.

A avaliação deverá considerar:
- Funcionamento da funcionalidade conforme o requisito relacionado.
- Recebimento e apresentação corretos dos dados simulados.
- Geração de alertas com as informações contextuais disponíveis.
- Registro das decisões realizadas pelo operador.
- Preservação da rastreabilidade das ocorrências.
- Tratamento adequado de entradas inválidas e falhas pontuais.
Caso o resultado observado seja diferente do esperado, o caso deverá ser registrado como reprovado ou bloqueado, acompanhado de uma descrição da divergência. Os resultados só deverão ser preenchidos após a execução dos testes.

## **7. Ambiente e recursos de teste**
O ambiente de testes será acadêmico e demonstrativo, utilizando os recursos disponíveis no desenvolvimento do SENTINELA, tais como:
- Aplicação web demonstrativa.
- Dados e eventos simulados.
- Simulador de sensores e dispositivos.
- Imagens e vídeos demonstrativos.
- Regras e parâmetros configurados para detecção.
- Interface de dashboard, mapa de monitoramento, central de alertas e histórico de ocorrências.
Não serão utilizados sensores, câmeras ou sistemas operacionais reais da AMAZUL ou da Marinha.

## **8. Limitações dos testes**
Os testes estarão restritos ao ambiente demonstrativo do projeto. Os resultados não representam validação operacional, certificação ou autorização para utilização em instalações nucleares ou outros ambientes críticos reais.

A análise automatizada identifica indícios e padrões, mas não determina autonomamente a ocorrência de uma ameaça. A avaliação final dos alertas permanece sob responsabilidade do operador humano.

## **9. Registro dos resultados**
Após a execução de cada caso, recomenda-se registrar as seguintes informações:
Campo	Descrição
ID do teste	Identificador do caso executado.
Data da execução	Data em que o teste foi realizado.
Responsável	Integrante que executou o teste.
Resultado	Aprovado, reprovado ou bloqueado.
Evidência	Captura de tela, log ou outro registro pertinente.
Observações	Falhas encontradas ou detalhes relevantes.


Status inicial: os casos de teste deste documento estão planejados. Nenhum resultado de execução é declarado nesta versão.
