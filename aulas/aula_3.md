# Aula 3 — Operações práticas no QGIS e imagens Sentinel-2

## Conteúdo abordado

1. Importação e preparação da Área de Interesse (AOI)
   - Importar AOI em SHP e converter para KML/KMZ para uso web
   - Importância de definir o SRC/CRS correto (especialmente para medidas confiáveis)

2. Sentinel Hub e composições de bandas
   - Uso do EO Browser para buscar e baixar imagens Sentinel‑2
   - Diferenças entre cor verdadeira, falsa cor e índices de vegetação (ex.: NDVI)
   - Baixamos uma imagem Sentinel‑2 nas três configurações: cor verdadeira, falsa cor e índice de vegetação

3. QGIS — plugins e organização
   - Plugin de basemaps para contexto cartográfico (basemaps)
   - Plugin Layout Loader
   - Navegador e organização da Caixa de Camadas (grupos, duplicar camadas, nomenclatura)

4. Edição vetorial e atributos
   - Ferramentas de Vetorização Avançada (snapping, restrições, precisão)
   - Tabela de atributos: edição básica, criação/ configuração de campos
   - Observação: mostramos a ferramenta de cálculo de áreas, mas não realizamos cálculo em m² nesta aula

5. Raster: bandas e visualizações
   - Conceitos de renderização de bandas no QGIS
   - Cor verdadeira (B4‑B3‑B2), falsa cor (B8‑B4‑B3) e NDVI (B8, B4)

## Ferramentas e recursos apresentados

- Sentinel Hub (EO Browser)
  - https://apps.sentinel-hub.com/eo-browser/
  - Documentação Sentinel‑2 L2A: https://docs.sentinel-hub.com/api/latest/data/sentinel-2-l2a/

- QGIS — Basemaps
  - QuickMapServices (plugin): https://plugins.qgis.org/plugins/quick_map_services/

- QGIS — Layout Loader
  - Página de busca do plugin: https://plugins.qgis.org/search/?q=layout%20loader

- QGIS — Documentação (recursos usados)
  - Projeções/SRC: https://docs.qgis.org/latest/en/docs/user_manual/working_with_projections/working_with_projections.html
  - Vetorização e Digitalização: https://docs.qgis.org/latest/en/docs/user_manual/digitizing/digitizing_tools.html
  - Tabela de Atributos: https://docs.qgis.org/latest/en/docs/user_manual/working_with_vector/attribute_table.html
  - Simbologia/Estilos: https://docs.qgis.org/latest/en/docs/user_manual/visualization/symbology.html
  - Painel Navegador: https://docs.qgis.org/latest/en/docs/user_manual/introduction/qgis_gui.html#the-browser-panel

## Próximos passos

- Reforçar a escolha de SRC projetado adequado antes de quaisquer cálculos de área/perímetro.
- Praticar cálculos de área (ex.: hectares) e análise de atributos no QGIS.
- Aplicar Layout Loader para padronizar mapas e exportar produtos (PDF/PNG).
- Explorar séries temporais no Sentinel Hub (NDVI/EVI) e máscaras de nuvens.
