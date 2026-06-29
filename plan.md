
scopo de Funcionalidades e Regras de Negócio

Funcionalidades Core Implementadas

1. Auto-completar Assíncrono
* Busca inteligente baseada em caixa baixa (`.toLowerCase()`) e correspondência de texto (`.includes()`).
* Preenchimento automático dos metadados (TDP e Preço médio) para agilizar o cálculo.

2. Limitador de Orçamento Dinâmico (Budget Cap)
* Entrada numérica para definição de teto orçamentário.
* Barra de progresso reativa calculada em tempo real com base no custo acumulado do setup.
* Gatilho de alerta visual que muda a interface para modo crítico se o valor estourar.

3. Alerta de Consumo e Compatibilidade
* Verificação lógica: Se o setup contiver uma GPU de alto desempenho (Série RTX 40/50) e o consumo somado for elevado, o sistema injeta um alerta instruindo o uso de fontes de no mínimo 750W/850W Gold.

4. Portabilidade P2P (Share Build)
* Sistema de importação e exportação via strings Base64 geradas por prompts nativos, eliminando dependência de banco de dados centralizado.

5. Injeção de Presets
* Modelos de entrada, intermediário e entusiasta injetados diretamente no array de estado para testes rápidos de usabilidade.