# Decisões posteriores à pesquisa

A pesquisa foi escrita antes das decisões de construção. Esta página registra o que o projeto seguiu, onde divergiu e por quê. Atualizada em 29 de setembro de 2026.

## O que foi seguido

| Recomendação da pesquisa | Como entrou no projeto |
|---|---|
| Núcleo inteiro gratuito | Comunicação, edição, fotos, voz, backup, exportação e impressão sem custo |
| Funcionar sem conta e sem internet | O app abre direto na prancha. O projeto não tem servidor |
| Posições e caminhos previsíveis | A posição de cada botão é fixa e guardada por tipo de aparelho. Nada reordena a grade |
| Proteger a autoria da mensagem | Nada é falado sem ação da pessoa. Nenhum recurso reescreve a mensagem |
| Português brasileiro como conteúdo original revisado | Vocabulário próprio, revisado por fonoaudióloga que trabalha com CAA |
| Sem IA generativa no núcleo | O comunicador não usa IA e nunca espera a rede |
| Dados portáveis | Backup próprio com formato publicado, e importação e exportação em Open Board Format |
| Sem alegação terapêutica | Textos do app e deste repositório não prometem fala nem resultado clínico |

## Onde o projeto divergiu

| Recomendação da pesquisa | Decisão do projeto | Motivo |
|---|---|---|
| Validar AsTeRICS AAC e Cboard antes de construir | Construir um app próprio | A lacuna foi documentada. Ver a seção seguinte |
| Flutter como candidato para o app | Capacitor com React e TypeScript | Experiência prévia do mantenedor, HTML semântico como base de acessibilidade e versão web sem custo extra |
| Repositório público de código | Código fechado e conteúdo aberto | Decisão do mantenedor. Em compensação, os formatos de arquivo e a especificação da criptografia são publicados aqui |
| Sincronização futura com contas de apoio | Sem servidor e sem contas | Custo recorrente e guarda de dados de crianças inviabilizariam um app gratuito mantido por uma pessoa. A troca entre família e terapeuta usa pacotes cifrados por QR, link ou arquivo |
| IA opcional só numa fase posterior | Integrações opcionais com a chave do próprio usuário | Permitem voz de melhor qualidade e geração de pictogramas sem custo para o projeto. Ficam desligadas por padrão e fora do caminho da fala |
| Geração de símbolos por IA exige avaliação rigorosa | Adotada, com revisão obrigatória de um adulto | Nenhum pictograma gerado entra numa prancha sem aprovação. A prancha exibe sempre imagem, nunca o desenho vetorial direto |
| Nenhum histórico detalhado por padrão | Registro de uso opcional | Desligado por padrão, guardado só no aparelho, com contagens em vez de frases, indicador visível e pausa pela própria pessoa |

## A lacuna documentada

Verificada nos repositórios e nas páginas oficiais em 29 de setembro de 2026.

| Ferramenta | Lacuna para quem fala português do Brasil |
|---|---|
| Cboard | Tradução para português brasileiro feita por máquina e nunca revisada, segundo o próprio projeto. Exportação em formato aberto e gravação de voz no plano pago |
| AsTeRICS AAC | Cerca de dois terços dos textos da interface em português brasileiro ainda estão em inglês. Não foi encontrado conjunto de vocabulário núcleo em português brasileiro. Funciona só como aplicativo web |
| Todas as bases avaliadas | Nenhuma oferece vocabulário em português brasileiro revisado por fonoaudiólogo, e não foi encontrado nenhum arquivo aberto de pranchas em português brasileiro |

O vocabulário deste projeto será publicado em formato aberto justamente para servir também a quem usa essas ferramentas.

## O que continua em aberto

| Ponto da pesquisa | Situação |
|---|---|
| Participação remunerada de usuários de CAA | Ainda não definida |
| Pesquisa com 8 a 12 unidades de participação | Prevista como piloto acompanhado com um centro terapêutico, ainda a formalizar |
| Plano de manutenção e orçamento anual | Ainda não escrito. O projeto não tem custo recorrente de infraestrutura |
| Acesso por varredura, olhar e controle de cabeça | Fora da primeira versão, como a pesquisa recomenda |

---

[Índice](README.md)
