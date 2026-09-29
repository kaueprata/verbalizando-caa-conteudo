# 9. Arquitetura e decisão sobre a base

## Avaliar antes de escolher

| **Caminho** | **Benefício esperado** | **Custo ou limitação** | **Avaliação estratégica** |
|----|----|----|----|
| Contribuir com uma base aberta existente | Reutilizar maturidade e concentrar esforço em português e implantação | Alinhamento com governança e arquitetura existentes | 9/10 para começar a investigação |
| Manter uma adaptação própria de base aberta | Maior controle da experiência com funções já disponíveis | Manter divergências, atualizações e obrigações da licença | 8/10 se houver lacunas comprovadas |
| Construir app próprio | Controle sobre acesso local, integração e produto | Maior esforço de engenharia, teste e manutenção | 7/10 antes da prova técnica; reavaliar depois |

As notas são julgamentos de estratégia para este projeto. Não comparam eficácia clínica dos aplicativos.

O repositório atual do AsTeRICS AAC informa AGPL 3.0 e documenta múltiplos métodos de entrada, execução offline e sincronização opcional. O Cboard informa GPL 3.0 e uso de síntese de fala do navegador. Ao escolher uma base, verificar o arquivo de licença da versão efetivamente adotada, dependências e conteúdo. Distribuir ou oferecer versões modificadas pode trazer obrigações de disponibilização de código. [\[13–14\]](fontes.md#f13)

## Estrutura proposta para um produto próprio

Separar seis módulos: comunicador, editor, conteúdo linguístico, recursos de acessibilidade, voz e dados locais. O comunicador deve continuar disponível se a sincronização, a atualização de conteúdo ou um serviço opcional falhar.

Para uma implementação móvel nova, Flutter é um candidato, a ser comparado com React Native ou desenvolvimento nativo conforme a equipe. Proponho armazenamento local transacional, mídia em arquivos locais e adaptadores para voz e tecnologias assistivas de cada sistema. Um editor web pode vir depois, reutilizando o formato de conteúdo.

Uma PWA é útil para distribuição e avaliação inicial. Sua voz, persistência de armazenamento e comportamento offline dependem de navegador e sistema. A documentação do AsTeRICS confirma essa variação e recomenda vozes offline pela confiabilidade. Logo, a decisão entre web e aplicativo instalado deve sair de uma prova em aparelhos representativos. [\[15–16\]](fontes.md#f15)

**Prova técnica proposta:** abrir offline depois de reiniciar o aparelho; falar português; recuperar a prancha; tolerar interrupção de áudio; editar uma foto; restaurar backup; operar com foco e acionamento acessíveis. Comparar pelo menos um Android de entrada, um intermediário e um iPad utilizado pelo público.

---

[← 8](08-portugues-brasileiro-e-biblioteca-visual.md) · [Índice](README.md) · [Fontes](fontes.md) · [10 →](10-voz-e-confiabilidade.md)
