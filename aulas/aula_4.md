# Aula 4 — Topodata no QGIS: Download, manipulação e visualização de dados topográficos

## Conteúdo abordado

1. Utilização prática da plataforma Topodata
   - Apresentação da plataforma Topodata para obtenção de dados topográficos do Brasil
   - Entrega e utilização do KMZ do grid do Topodata (disponível no Drive), contendo links diretos para download das camadas

2. Download e preparação de dados
   - Download da camada de elevação a partir do grid
   - Organização dos arquivos baixados no QGIS: duplicação de camadas, agrupamento e nomenclatura

3. Manipulação de rasters e vetores
   - Corte (clip) de raster usando AOI (Área de Interesse)
   - Corte de shapefile (vector) para delimitar áreas específicas
   - Resolução de problemas de projeção e alinhamento entre camadas

4. Visualização avançada
   - Sobreposição de uma mesma camada raster com diferentes estilos de simbologia para criar visualizações mais chamativas (ex: elevação + relevo sombreado)
   - Ajuste de transparência, paleta de cores e estilos personalizados

5. Extração de informações topográficas
   - Criação de curvas de nível (contornos altimétricos) usando a ferramenta de conversão de raster para linhas
   - Discussão sobre parâmetros de intervalo altimétrico e qualidade do resultado

## Ferramentas e recursos apresentados

- Plataforma Topodata
  - Acesso: http://www.dsr.inpe.br/topodata/
  - Sobre o Topodata: http://www.webmapit.com.br/topodata/
  - Grid KMZ para QGIS (disponível no Drive do curso)

- QGIS — operações utilizadas
  - Ferramenta de recorte raster: https://docs.qgis.org/latest/pt_BR/docs/user_manual/processing_algs/qgis/rasteranalysis.html#clip-raster-by-mask-layer
  - Corte de shapefile: https://docs.qgis.org/latest/pt_BR/docs/user_manual/processing_algs/qgis/vectoroverlay.html#clip
  - Resolução de projeções: https://docs.qgis.org/latest/pt_BR/docs/user_manual/working_with_projections/working_with_projections.html
  - Visualização de rasters: https://docs.qgis.org/latest/pt_BR/docs/user_manual/visualization/raster.html
  - Curvas de nível: https://docs.qgis.org/latest/pt_BR/docs/user_manual/processing_algs/gdal/rasterextraction.html#contour
