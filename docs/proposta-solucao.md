# **Proposta de Solução — SENTINELA**

## **1. Visão Geral**

O SENTINELA propõe o desenvolvimento de uma plataforma web inteligente para centralização de informações, detecção de anomalias e correlação de eventos provenientes de diferentes fontes de monitoramento.

A plataforma permitirá reunir dados de dispositivos como câmeras, sensores ambientais e sistemas de controle de acesso em um ambiente único, proporcionando uma visão integrada das informações monitoradas.

A solução utilizará mecanismos de análise específicos para cada tipo de informação recebida, combinando regras configuráveis, processamento de dados e técnicas de visão computacional para identificar possíveis eventos fora dos padrões estabelecidos.

## **2. Funcionamento da Solução**

O funcionamento do SENTINELA será dividido em etapas:

### **2.1 Recebimento e centralização de dados**

A plataforma receberá informações provenientes de diferentes fontes de monitoramento. No protótipo acadêmico, esses dados serão gerados por simuladores e arquivos demonstrativos.

### **2.2 Análise das informações**

Os dados recebidos serão encaminhados para mecanismos de análise conforme sua natureza:

- **Sensores:** utilização de regras, limites e parâmetros configuráveis para identificar valores ou comportamentos fora do padrão.
- **Imagens e vídeos:** utilização de técnicas de visão computacional para identificar objetos e situações relevantes nas mídias demonstrativas.

### **2.3 Detecção e correlação de eventos**

Após a análise, o sistema identificará possíveis anomalias e verificará a existência de outros eventos relacionados.

A correlação considerará critérios como horário, localização, tipo de ocorrência e dispositivo de origem. Dessa forma, diferentes eventos poderão ser analisados em conjunto, permitindo identificar situações que poderiam passar despercebidas quando avaliadas isoladamente.

### **2.4 Geração e gerenciamento de alertas**

Com base nas análises realizadas, o SENTINELA gerará alertas contextualizados, reunindo informações sobre a ocorrência, sua origem, localização, horário, evidências disponíveis e eventos relacionados.

Os operadores poderão visualizar, analisar, classificar, confirmar ou descartar os alertas, registrando suas decisões na plataforma.

### **2.5 Histórico e rastreabilidade**

As ocorrências identificadas e as decisões realizadas pelos operadores serão armazenadas para permitir consultas posteriores, acompanhamento de incidentes e rastreabilidade das ações.

## **3. Participação do Operador**

O SENTINELA terá caráter de apoio à tomada de decisão. Os mecanismos automatizados serão responsáveis por identificar possíveis anomalias e apresentar informações relevantes, mas a avaliação final das ocorrências permanecerá sob responsabilidade dos operadores humanos.

Essa abordagem busca evitar que uma detecção automatizada seja interpretada automaticamente como uma ameaça confirmada.

## **4. Tecnologias e Abordagem de Desenvolvimento**

A proposta considera a utilização de tecnologias para desenvolvimento web, processamento de dados e visão computacional.

Entre as tecnologias inicialmente consideradas estão React, Python, FastAPI, OpenCV, YOLO e PostgreSQL. A seleção definitiva dependerá das necessidades de implementação e das condições do protótipo.

## **5. Limitações da Proposta**

Para o desenvolvimento do protótipo acadêmico, serão utilizados dados simulados e arquivos demonstrativos, permitindo validar o fluxo de centralização, análise, detecção, correlação e apresentação de alertas sem depender de equipamentos ou instalações reais.

A solução não contempla integração com sistemas operacionais da AMAZUL ou da Marinha, controle físico de drones, detecção de radiação ou certificação para utilização em instalações nucleares.

Portanto, o SENTINELA será apresentado como uma demonstração acadêmica de monitoramento inteligente e apoio à tomada de decisão, não como uma solução pronta para operação em ambientes críticos reais.
