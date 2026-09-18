# Ficha de análise · Português Studio IA

Arquivo entregue: `individual/Portugues_Studio_IA.html` (149 KB, 10 scripts, 0 erros de sintaxe, 0 onclick inline).

## O que estava errado no lote

Mesma família da Paleontologia (mesma estrutura, mesmo motor): 8 eixos de trabalho em chips, sugestões de conteúdo por eixo com o dado de sortear, 15 tipos de material, resumo "Seu material terá". No lote a fase dos tipos passava de 890 px (15 cartões em duas colunas) e a acessibilidade da suíte nascia em Gerar, que chegava a 834 px.

Ajustes, os mesmos da Paleontologia e só de apresentação: cartões em três colunas (chave `css` dos ajustes individuais), acessibilidade para "Formato e estilo" (regra R3), títulos e subtítulos. Nada no script mudou.

## Fluxo

| | Original | Premium |
|---|---|---|
| Etapas | 6: O tema · Tipo de material · A turma · Como fica · Identificação · Gerar | 5: O tema · O que você vai criar · A turma · Formato e estilo · Gerar |
| Cliques até o comando | 6 | 5 |
| Fase mais alta em 1366 px | 891 px no lote (tipos) | 708 px (tipos, em três colunas) |
| Acessibilidade | em Gerar | em Formato e estilo (669 px); Gerar ficou em 614 px |

Sem fusão nova: O tema (553 px) mais os tipos (708 px) e A turma (584 px) mais Formato e estilo (669 px) passam de 880.

## Controles

- O tema: 8 eixos (Leitura e interpretação, Gramática em uso, Ortografia, Gêneros textuais, Produção textual, Literatura, Oralidade, Variação linguística), conteúdo com sortear e sugestões do eixo, assunto do texto.
- O que você vai criar: 15 tipos em três colunas (Interpretação de Texto, Gramática em Uso, Ortografia, Gênero Textual, Produção Textual, Correção e Reescrita, Vocabulário e Sentido, Literatura, Oralidade, Variação Linguística, Jogo de Português, Flashcards, Avaliação, Questões estilo ENEM, Sequência Didática).
- A turma: ano, finalidade, foco, gênero, questões e os extras (Proposta de escrita, Momento de oralidade, Descritor do SAEB, Habilidade da BNCC). Formato e estilo: "Vai ser usado", cartões Imprimir/Projetar, estilo, modo econômico, chips de acessibilidade.
- Gerar: identificação, "Onde você vai gerar", resumo "Seu material terá", botão principal; tela de resultado padrão.

## Comunicação (texto de tela, nunca do comando)

- Trilha: "Tipo de material" → "O que você vai criar"; "Como fica" → "Formato e estilo". Subtítulos: "Onde o material será usado, o estilo e as adaptações da turma."; Gerar: "Identificação e o comando pronto para colar na IA."
- Botões: "Próximo →" / "← Voltar" → "Continuar" / "Voltar"; "📕 Gerar Ficha Visual Inteligente" e "🎲 Gerar uma variação com texto novo" → sem emoji; "ver conteúdo" → "Ver o comando"; o dado de sortear ganhou o ícone da folha. Estados de cópia na voz única. As sugestões com lâmpada são escritas pelo motor.

## Prova

1. **Comando byte a byte igual**, pelo caminho real, na original e na premium (robô `prova_padrao.js`): padrão (16.333 c); segunda opção em todos os campos, dois chips de inclusão, projetar e variação (18.523 c); última opção em todos os campos, TEA e identificação (17.604 c). 3 de 3 idênticos, 0 erros.
2. **12 dispositivos** (5 fases e resultado com comando aberto): 0 vazamentos, 0 alvos abaixo de 44 px, 0 texto miúdo, trilha sem rolagem.
3. **Sem lampejo** com CPU 12× mais lenta.
