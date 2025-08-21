
## 1) Configurar estilos (simbologia)

A) Camadas vetoriais
1. Clique direito na camada > Propriedades > Simbologia.
2. Escolha o modo:
   - Cor única: um estilo para todas as feições.
   - Categorizado: selecione um Campo (ex.: classe) > Classificar.
   - Graduado: selecione um Campo numérico (ex.: índice) > Modo (Quantis/Natural Breaks) > Número de classes > Classificar.
3. Ajustes rápidos:
   - Cores e espessuras (linhas), preenchimento (polígonos), tamanho (pontos).
   - Transparência (Global): Propriedades > Transparência.
4. Rotulação (opcional): Propriedades > Rótulos > Único rótulo > escolha o campo > ajuste fonte, buffer.
5. Salvar/Reutilizar estilo:
   - Botão Estilo (canto inferior esquerdo) > Salvar Estilo… (.qml) ou Salvar no Projeto.
   - Copiar/Colar estilo: clique direito na camada > Estilo > Copiar Estilo; na outra camada > Estilo > Colar Estilo.

B) Camadas raster
1. Clique direito na camada > Propriedades > Simbologia.
2. Renderização:
   - RGB (três bandas): defina as bandas para R, G, B (ex.: B4/B3/B2).
   - Banda única pseudocor: escolha paleta (ex.: RdYlGn) e defina Min/Max.
3. Contraste/Stretch:
   - Estatísticas: Min/Max ou Percent Clip (ex.: 2–98%).
   - Reamostragem de exibição (Melhor visualização ao dar zoom).
4. Transparência global conforme necessário.
5. Salvar estilo (.qml) via botão Estilo.

Dicas rápidas:
- Para comparar simbologias, duplique a camada (Ctrl+C/Ctrl+V) e aplique estilos diferentes.
- Use grupos no Painel de Camadas para organização.

---

## 2) Tabela de atributos — editar e configurar colunas

A) Acessar e editar
1. Clique direito na camada > Abrir Tabela de Atributos.
2. Ativar edição (ícone lápis).
3. Adicionar campo (ícone “+”):
   - Defina Nome, Tipo (Inteiro, Decimal, Texto, Data), Comprimento/Precisão se aplicável.
4. Configurar campo (opcional):
   - Propriedades da Camada > Campos: defina Valor padrão (expressão), Restrição (ex.: "valor" > 0) e Comentários.

B) Calculadora de Campo
1. Ícone Calculadora de Campo.
2. Crie um novo campo ou atualize um existente.
3. Exemplos de expressões:
   - Texto maiúsculo: upper("nome")
   - Concatenar: "classe" || ' - ' || "subclasse"
   - Número formatado: to_real("indice")
   - Data atual: now()
   - Área (opcional): $area  (use SRC projetado em metros; para hectares: $area/10000)
4. Aplicar > Salvar Edições > Desativar edição.

C) Selecionar por atributos (rápido)
1. Na Tabela de Atributos: ícone “Selecionar por Expressão”.
2. Exemplos:
   - "nome" ILIKE '%parque%'
   - "valor" >= 100
   - "classe" IN ('APP','Reserva')
3. Aplicar e fechar.

Dicas rápidas:
- Evite cálculos métricos em EPSG:4326 (graus). Prefira SIRGAS 2000 / UTM da sua zona.
- Use “Refatorar campos” (Processamento) para renomear/remover/reordenar colunas em lote.

---

## 3) Selecionar por localização

Opção 1 — Menu Selecionar
1. Menu superior: Selecionar > Selecionar por Localização…
2. Defina:
   - Camada de destino (onde a seleção será feita).
   - Predicado espacial (ex.: intersecta, contém, dentro, toca, distancia até).
   - Camada de comparação (a que será usada para a relação espacial).
   - Comportamento da seleção: substituir/ somar/ remover da seleção atual.
   - Distância (quando usar “está a uma distância de”).
3. Executar. As feições da camada de destino serão selecionadas.

Opção 2 — Caixa de Ferramentas (Processamento)
1. Processamento > Caixa de Ferramentas > Vector Selection > Select by location.
2. Preencha os mesmos parâmetros e Execute.
3. Para salvar o resultado como nova camada: use “Extrair feições selecionadas” ou “Extrair por localização”.

Dicas rápidas:
- Projeção: para predicados com distância/tolerância, use camadas em SRC projetado (metros).
- “contém” vs “intersecta”: “contém” exige inclusão total; “intersecta” basta tocar/cruzar.
- Se a seleção falhar, valide geometrias: Vetor > Geometria > Corrigir Geometrias.

---

Checklist de boas práticas
- Definir SRC do projeto e da camada antes de medir/selecionar por distância.
- Salvar estilos (.qml) e criar um repositório de estilos do projeto.
- Documentar novos campos (descrição/unidade) em Propriedades > Campos.
