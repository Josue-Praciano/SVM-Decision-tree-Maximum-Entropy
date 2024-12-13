# SVM-Decision-tree-Maximum-Entropy
Treinando esses modelos em dados anotados do corpus, buscando determinar qual algoritmo tem melhor desempenho no reconhecimento dos papéis temáticos em sentenças que contêm verbos psicológicos.

O corpus: Tycho Brahe - www.tycho.iel.unicamp.br

Preprocessamento do Corpus:

- Tokenização: divisão das frases em tokens 
- Part-of-Speech (POS) Tagging: anotação das categorias gramaticais.
- Mapeamento das relações sintáticas associadas aos verbos, como sujeito, objeto direto e complementos.
- Parsing de dependências: identificação de relações gramaticais entre os tokens (Stanford Parser)

Conjunto de Treinamento e Teste:
Divisão estratificada do corpus em dados de treinamento (70%) e teste (30%).

Extração de Características
Representação das relações gramaticais das sentenças contendo os verbos psicológicos.
Tipo de dependência entre o verbo e seus argumentos (ex.: nsubj, obj, obl).
Presença de Ligação Anafórica 
Ergatividade
Causatividade
Passivização sintática ou adjetiva
pro arbitrário como sujeito
causativas encabeçadas com - fazer -
Uso de ferramentas de Semantic Role Labeling (SRL) para anotar papéis como Experienciador e Tema.

Representação dos Dados:
Vetores de características combinando as informações sintático-semânticas e linguísticas personalizadas.
Técnicas com One-Hot Encoding ou representações densas para atributos categóricos.
Treinamento:
Treinamento individual dos três algoritmos nos dados preparados.
Predição e Avaliação:
Cada modelo realiza a predição dos papéis temáticos com base nas características extraídas.
