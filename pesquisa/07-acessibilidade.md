# 7. Acessibilidade como requisito de funcionamento

Cada configuração deve responder a uma necessidade observada. Uma estética infantil, muitos efeitos, um tema escuro ou um número pequeno de botões não são, por si, recursos universalmente adequados.

| **Área** | **Requisito proposto** | **Como verificar** |
|----|----|----|
| Toque | Alvos amplos, distância útil e ajuste de tempo de ativação | Uso no tablet e telefone por pessoas com diferentes precisões motoras |
| Acesso alternativo | Ordem de foco lógica, teclado e acionamento por tecnologias do sistema | Executar o fluxo inteiro sem toque direto |
| Visão | Contraste, rótulos legíveis, ampliação e imagens substituíveis | Testar tema, tamanho e contraste com o usuário |
| Cognição e atenção | Navegação curta e consistente, sem pop-ups na comunicação | Observar erros, retornos e busca de palavras |
| Audição e fala | Texto visível, controle de volume, velocidade e voz | Conferir compreensão com interlocutores reais |
| Controle | Desfazer, interromper fala e recuperar a frase | Simular seleção errada e limpeza acidental |
| Sensibilidade | Animação e vibração opcionais; nenhuma música obrigatória | Verificar preferências, conforto e distrações |

Na web, a WCAG 2.2 define 24 por 24 pixels CSS como mínimo do critério AA de tamanho de alvo, com exceções; o critério aprimorado utiliza 44 por 44. Isso é referência de acessibilidade, não medida clínica suficiente para uma prancha de CAA. Para dispositivos móveis, definir medidas apropriadas à plataforma e testar dimensões maiores conforme o acesso. [\[33\]](fontes.md#f33)

Usar como referência WCAG 2.2 AA para a interface web, incluindo contraste, foco, operação por teclado e identificação dos controles. Conformidade exige avaliação do conjunto; cumprir apenas tamanho de botão não é suficiente. [\[34\]](fontes.md#f34)

Se Flutter for escolhido, seus recursos de semântica e testes de acessibilidade ajudam, mas os componentes personalizados precisam de implementação explícita e avaliação com tecnologias assistivas. A escolha do framework não certifica acessibilidade. [\[32\]](fontes.md#f32)

Acesso por olhar, controle de cabeça e varredura especializada devem entrar em uma etapa com profissionais e usuários desses métodos. A primeira versão não deve anunciar suporte pleno apenas porque um ponteiro conseguiu clicar em uma demonstração.

---

[← 6](06-experiencia-de-uso.md) · [Índice](README.md) · [Fontes](fontes.md) · [8 →](08-portugues-brasileiro-e-biblioteca-visual.md)
