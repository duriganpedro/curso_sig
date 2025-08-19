# Aula 1 - Introdução aos Sistemas de Informação Geográfica (SIG)

## Conteúdo abordado

Nesta primeira aula, foram introduzidos conceitos fundamentais para o entendimento e utilização de Sistemas de Informação Geográfica (SIG):

1. **Conceitos básicos de SIG**
   - Definição e aplicações
   - Importância na análise espacial e tomada de decisões

2. **Projeções Cartográficas**
   - Conceitos de projeções e sistemas de coordenadas
   - Principais projeções utilizadas no Brasil
   - Impacto da escolha da projeção na análise de dados geográficos

3. **Tipos de dados geográficos**
   - **Dados vetoriais**: pontos, linhas e polígonos
   - **Dados matriciais (raster)**: imagens de satélite, modelos digitais de elevação
   - Diferenças e aplicações específicas de cada tipo

4. **Organização de pastas e arquivos em projetos SIG**
   - Boas práticas de nomenclatura
   - Estruturação lógica de projetos

## Ferramentas e recursos apresentados

### SATVEG - Sistema de Análise Temporal da Vegetação
O SATVEG é uma ferramenta da Embrapa para monitoramento da cobertura vegetal através de séries temporais de índices vegetativos.
- [SATVEG - Embrapa](https://www.satveg.cnptia.embrapa.br/)

### ForestGIS
Plataforma com diversos recursos para análises florestais e ambientais.
- [Site ForestGIS](https://www.forestgis.com/)
- [Plugin ForestGIS para QGIS](https://plugins.qgis.org/plugins/forestgis_plugin/)

### OpenStreetMap (OSM)
Mapa colaborativo mundial com dados geoespaciais livres.
- [OpenStreetMap](https://www.openstreetmap.org/)
- [Página de downloads do OSM](https://download.geofabrik.de/)

### MapBiomas
Projeto de mapeamento anual da cobertura e uso do solo no Brasil.
- [Site MapBiomas](https://mapbiomas.org/)
- [Plugin MapBiomas para QGIS](https://mapbiomas.org/pages/plugins)

## Estrutura de arquivos utilizada

Durante a aula, utilizamos alguns arquivos de exemplo organizados na seguinte estrutura:

```
input/
  ForestGIS_BaseLayers/
    ForestGIS_BaseLayers.gpkg
  vetores/
    BR_Municipios_2024/
      BR_Municipios_2024.shp
      area.shp
      curso.shp
      inter.shp
      ITURAMA.shp
    cidade.osm
```

## Próximos passos

Na próxima aula, iremos aprofundar os conhecimentos práticos com exercícios de manipulação dos dados geográficos apresentados, utilizando o QGIS como principal ferramenta de trabalho.
