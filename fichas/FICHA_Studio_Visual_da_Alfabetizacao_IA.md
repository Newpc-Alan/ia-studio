# Ficha de análise · Studio Visual da Alfabetização IA · 16/09/2026

## 1. Fluxo
- Original: 4 fases (Atividade · Aparência · Identidade · Gerar).
- Agora: 3 (Atividade e turma · Estilo e formato · Gerar). "Identidade" entrou no topo de Gerar; escola em cima, professor, município, destino e turma numa grade 2x2, depois título e instrução.

## 2. Controles
- Esta ferramenta ficou fora do retrofit de julho: os campos de identificação tinham ids próprios (i-prof, i-escola, i-municipio), e por isso três camadas da suíte nunca montavam aqui: identificação compartilhada entre ferramentas (localStorage), seletor "Onde você vai gerar" e o bloco de acessibilidade. Só o id dos três campos mudou (o motor lê o mesmo valor); com isso as três camadas passaram a funcionar. Os chips de acessibilidade foram para a fase de estilo, ao lado do select de adaptação inclusiva que a ferramenta já tinha.
- Formato: os cartões Imprimir na folha / Projetar na lousa (camada de orientação, sobre o select #i-orient) já existiam; ganharam a cor e ficaram na fase de estilo.

## 3. Saída
- Bloco padrão reordenado pela grade (Copiar primeiro). Mensagem de estado sem "prompt".

## 4. Comunicação
- "Atividade" → "Atividade e turma" (a etapa escolar está nela); "Aparência" → "Estilo e formato"; subtítulo de Gerar sem "prompt".

## 5. Prova, e a única diferença deliberada no comando
- Com os mesmos valores nos dois lados, o comando tem 138 linhas e difere em 2: a DECLARAÇÃO DE USO DE IA, que agora nomeia a IA escolhida e o professor ("material produzido com ChatGPT ... responsabilidade: Prof. Alan Ramos") em vez do genérico "ferramenta de IA generativa ... do professor que aplica o material". É o padrão das outras 40; aqui só não acontecia porque a camada não montava. Todo o resto é byte a byte igual.
- 12 de 12 dispositivos, zero erro.

## 6. Defeito herdado, não corrigido (aguarda decisão)
- No rodapé do comando, a instrução "Logo abaixo ... escreva a DECLARAÇÃO DE USO ..." sai TRÊS vezes seguidas, igual ao caso já relatado no Criador de Cartazes: camadas de retrofit empilhadas. Corrigir muda o motor (remove a repetição). Não mexi sem o seu aval.
