#  Análise Bibliográfica e Fluxograma PRISMA em Python

Este projeto automatiza a **busca, triagem e visualização de artigos científicos** seguindo uma Revisão Sistemática de Literatura, usando Python. Ele inclui a geração de métricas de avaliação (precision, recall, F1) e a criação de um **fluxograma PRISMA**.

---

##   Funcionalidades

1. **Definição da estratégia de busca**  
   - Termos relacionados a violência juvenil, centros comunitários, políticas públicas, prevenção e engajamento de jovens.
   - Filtro por idioma (`English` e `Portuguese`) e tipo de artigo (`Journal Article`, `Review`, `Working Paper`).
   - Delimitação de período de publicação (ex.: 2010-01-01 a 2025-09-30).

2. **Busca de artigos**  
   - Realiza consulta em bases de dados (ex.: PubMed).
   - Retorna lista de artigos com título, resumo e metadata.

3. **Deduplicação e padronização**  
   - Identificação de duplicatas
   - Criação de `gold standard` baseado em termos-chave

4. **Métricas de avaliação**  
   - **Precision** → proporção de artigos identificados que são realmente relevantes  
   - **Recall** → proporção de artigos relevantes que foram identificados  
   - **F1 Score** → média harmônica entre precision e recall  

5. **Fluxograma PRISMA**  
   - Visualização do processo de triagem:
     - Registros identificados
     - Registros após deduplicação
     - Registros triados
     - Registros excluídos
     - Artigos avaliados em texto completo
     - Estudos incluídos na análise final
   - Fluxograma criado com `matplotlib` (sem necessidade do Graphviz)

6. **Exportação de resultados**  
   - Artigos incluídos salvos em Excel (`.xlsx`)
