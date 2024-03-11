# Pontos de Função: Detalhamento dos fatores técnicos

A técnica de pontos de função sugere 14 fatores de ajuste técnico (General Systems Characteristics - GSC). 
Atribuímos uma nota de 0 até 5 pare eles, sendo que zeero significa que o fator não possui influência e 5 para um fator que possui influência determinante no projeto.

Nos parágrafos a seguir, são detalhados os fatores técnicos, de acordo com Wazlawick:

## Comunicação de dados

**Comunicação de dados:** Avaliamos o grau em que necessidades especiais de comunicação afetam o sistema. Sistemas isolados estariam no extremo inferior da avaliação; já os sistemas que fazem uso intensivo de dados obtidos em outros lugares e que enviam informação para muitos lugares diferentes, através de diferentes protocolos de comunicação, estariam no extremo oposto. 
* 0: aplicações que são somente processamento em batch ou que executam isoladas em um computador
* 1: aplicações em batch, mas como entrada de dados remota ou saída demota
* 2: aplicações em batch com entrada de dados remota e saída remota
* 3: aplicações que incluem coleta de dados online ou front-end de teleprocessamento para um sistema em batch ou sistema de consultas
* 4: aplicações que são mais do que um front-end, mas suportam um único tipo de protocolo de comunicação
* 5: aplicações que são mais de um front-end e suportam vários tipos de protocolos de comunicação

