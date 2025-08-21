# Aula 2 – Ambiente do QGIS, Criação e Organização de Dados Espaciais

## Conteúdo abordado

Nesta segunda aula, exploramos na prática o ambiente do QGIS, aprendendo a navegar pelas principais ferramentas e interfaces do software. Os tópicos principais incluem:

1. **Ambiente do QGIS**
   - Tour pela interface: barras de ferramentas, painel de camadas e navegador
   - Múltiplas formas de realizar as mesmas operações (menus, botões, atalhos)
   - Importância de salvar frequentemente o projeto (`.qgz`)

2. **Criação e manipulação de dados espaciais**
   - Como criar um novo shapefile (vetor): definição de geometria, atributos e sistema de referência
   - Pesquisa, download e abertura de shapefiles de fontes como IBGE, OSM ou portais estaduais
   - Conversão e sugestão de uso do formato Geopackage (`.gpkg`) para maior robustez e organização dos dados

3. **Plugins e recursos adicionais**
   - Instalação e uso do plugin OpenStreetMap (OSM) para importar dados vetoriais diretamente
   - Exploração rápida de outros plugins úteis (ex.: QuickOSM)

4. **Configuração e organização de projetos**
   - Criação de um novo projeto QGIS
   - Configuração do SRC preferencial (por exemplo, SIRGAS 2000 / UTM Zone 23S)
   - Boas práticas para organização de pastas e arquivos de projetos

## Ferramentas e recursos apresentados

### QGIS
Software livre e multiplataforma para manipulação de dados geoespaciais.
- [Download QGIS](https://qgis.org/pt_BR/site/forusers/download.html)
- [Documentação oficial](https://docs.qgis.org/)

### OpenStreetMap (OSM) e Plugins
- [OpenStreetMap](https://www.openstreetmap.org/)
- [QuickOSM Plugin](https://plugins.qgis.org/plugins/QuickOSM/)

### Fontes de dados shapefile
- [IBGE - Download de Malhas](https://www.ibge.gov.br/geociencias/organizacao-do-territorio/malhas-territoriais.html)
- [Geofabrik OSM Downloads](https://download.geofabrik.de/)

## Modelo de organização de pastas

A seguir, um modelo sugerido para organização dos arquivos do projeto QGIS, buscando facilitar a manutenção, backup e compartilhamento dos dados:

```
meu_projeto_SIG/
  projeto/
    projeto_principal.qgz
  dados_brutos/
    ibge/
      municipios_2024.shp
      estados_2024.shp
    osm/
      cidade.osm
  vetores_editados/
    municipios_editado.gpkg
    bairros_editado.gpkg
  rasters/
    satelite_2020.tif
    mde_10m.tif
  mapas/
    mapa_final.pdf
    layout_legenda.qpt
  docs/
    relatorio.docx
    leitura_de_dados.txt
```

- **projeto/**: arquivos do projeto QGIS (`.qgz`)
- **dados_brutos/**: dados originais baixados de fontes externas (nunca editar direto aqui)
- **vetores_editados/**: vetores (preferencialmente em Geopackage) editados durante o projeto
- **rasters/**: imagens, MDEs, ortofotos
- **mapas/**: mapas exportados, layouts e produtos finais
- **docs/**: documentação, relatórios e anotações


# QGIS – Resumo Básico da Interface e Configurações:

## Principais janelas e painéis

- **Área de Mapa**  
  Espaço central onde os dados geográficos são visualizados e manipulados.

- **Barra de Ferramentas**  
  Ícones para acesso rápido a funções como zoom, seleção, adição de camadas, medição, entre outras.

- **Painel de Camadas**  
  Lista todas as camadas vetoriais e raster adicionadas ao projeto, permitindo controlar ordem, visibilidade e estilo.

- **Painel de Navegação**  
  Facilita o acesso a arquivos, bancos de dados e serviços web. Permite arrastar dados diretamente para o mapa.

- **Painel de Propriedades da Camada**  
  Exibe e permite editar propriedades de cada camada, como estilo, rótulos, transparência e SRC.

- **Painel de Atributos**  
  Mostra a tabela de atributos de uma camada (dados tabulares associados aos elementos espaciais).

- **Console Python**  
  Permite executar scripts para automação e personalização do QGIS.

## Abas e menus principais

- **Projeto**  
  Criar, abrir, salvar, exportar e configurar projetos.

- **Editar**  
  Ferramentas para edição de feições vetoriais.

- **Visualizar**  
  Opções de navegação e exibição do mapa.

- **Camada**  
  Adicionar, remover e gerenciar camadas vetoriais, raster, tabelas e serviços.

- **Configurações**  
  Preferências globais do QGIS, atalhos, configurações de interface.

- **Processamento**  
  Acesso ao Toolbox, onde ficam ferramentas de análise, geoprocessamento e scripts.

- **Plugins**  
  Instalação e gerenciamento de plugins que expandem funcionalidades do QGIS.

## Configurações básicas recomendadas

- **SRC do Projeto (Sistema de Referência de Coordenadas)**  
  Defina o SRC do projeto logo no início (exemplo: SIRGAS 2000 / UTM Zone 23S).

- **Salvamento Automático**  
  Ative o salvamento automático para evitar perda de dados.

- **Ajuste da Interface**  
  Personalize barras de ferramentas e painéis conforme sua rotina.

- **Instalação de Plugins Essenciais**  
  QuickOSM, OpenLayers, MMQGIS, entre outros, podem ser úteis dependendo do projeto.

---

Esse resumo cobre os componentes e configurações mais básicos do QGIS para quem está começando. A interface pode ser altamente personalizada, e novas funcionalidades podem ser adicionadas via plugins.
## Próximos passos

Na próxima aula, trabalharemos com operações e análises sobre os dados espaciais carregados, incluindo seleção, filtragem, análise de atributos e exportação de resultados.
