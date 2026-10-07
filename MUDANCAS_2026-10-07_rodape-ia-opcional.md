# Rodapé · aviso de IA opcional (07/10/2026)

## Regra
- A barra do Portal do Educador (site, YouTube, Instagram) sai SEMPRE no material.
- O aviso de uso de IA (quadro IA RESPONSÁVEL, declaração de uso e linha de conformidade com o ID) é OPCIONAL.
- Começa DESLIGADO em toda abertura da ferramenta. O professor decide na última fase, no interruptor "Incluir aviso de uso de IA no material".
- Com o aviso ligado, o campo "Onde você vai gerar este material" aparece dentro do quadro do interruptor.

## Onde vale
- 45 ferramentas com rodapé (blocos/ e docs/), incluindo Comando de Aula, Planejador Pedagógico e Biblioteca Visual.
- Fora: hub 00_IA_Studio_Botoes e Caixa de Ferramentas da Aula (não geram material com rodapé).

## Como funciona (camada PDE-RODAPE-IA-OPCIONAL-V1, no fim de cada arquivo)
- O filtro age nas duas saídas: o texto mostrado na tela e tudo o que vai para a área de transferência (Copiar, Copiar e abrir ChatGPT/Gemini/Claude). Por isso funciona também onde a tela e a cópia vinham de fontes diferentes (Planejador, Banco, Comando de Aula).
- Desligado: some o quadro IA RESPONSÁVEL, a declaração, a linha de conformidade, as regras do ID e os itens da checagem final que cobravam esses elementos; o contrato do topo passa a exigir só a barra final.
- Ligado: a declaração sai UMA vez no rodapé e nenhum marcador [[PDE_...]] chega à IA.
- O resumo "Seu painel terá" esconde "Selo IA Responsável com ID" enquanto o aviso estiver desligado.

## Correções de motor feitas junto
- Declaração triplicada escrita no código: corrigida na fonte em 40 ferramentas (44 trechos), nos blocos e nas páginas do GitHub Pages.
- A camada antiga que acrescentava a declaração no fim do comando só age com o aviso ligado.
- Tecnologia Sem Medo: o rodapé de reserva, que vazava código JavaScript e placeholders [professor]/[data] para dentro do comando, só entra quando o motor não trouxe rodapé nenhum.

## Provas
- Robô em 43 ferramentas (blocos) e 43 páginas (docs), nas duas posições do interruptor: barra presente, zero aviso de IA na tela e na cópia com o aviso desligado, aviso completo e sem marcador com ele ligado, zero erro de script.
- Equivalência: com o aviso desligado, o comando novo é idêntico ao antigo passado pelo filtro (nada além do rodapé mudou), exceto Tecnologia Sem Medo, que mudou de propósito.
- Comando de Aula, Planejador e Biblioteca: testados no Chromium real, tela = cópia nas duas posições.
- Interface: 1366 px e 390 px sem rolagem lateral.
