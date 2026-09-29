# 10. Voz e confiabilidade

No Android, a API de voz permite verificar se determinada voz exige rede. A implementação deve selecionar uma voz local compatível, conferir disponibilidade e orientar a instalação quando necessário. Um aparelho pode ter síntese de fala e ainda não ter o pacote de português adequado instalado. [\[30\]](fontes.md#f30)

No ecossistema Apple, a síntese de fala utiliza APIs como AVSpeechSynthesizer e AVSpeechSynthesisVoice. A lista real de vozes e o comportamento precisam ser testados nos aparelhos e versões de sistema apoiados. O produto não deve presumir que toda voz apresentada será utilizável offline em qualquer dispositivo. [\[31\]](fontes.md#f31)

**Comportamento proposto:** verificar voz e volume no início, com uma frase de teste curta. Guardar configurações por perfil. Manter áudio pré-gravado opcional para mensagens pessoais. Exibir claramente a falha e oferecer texto visível ou gravação disponível se a síntese não puder funcionar.

Evitar sobreposição e filas inesperadas de fala. O usuário precisa conseguir interromper imediatamente, repetir deliberadamente e ouvir a frase escolhida. Filtros de toque acidental não podem eliminar repetições intencionais de palavras. A resposta a um toque longo ou a vários toques deve ser configurável e documentada.

| **Indicador técnico** | **Meta inicial proposta** | **Condição de medição** |
|----|----|----|
| Abrir até a prancha utilizável | Percentil 95 de até 2 segundos | Aparelhos definidos, abertura a frio, conteúdo instalado |
| Confirmação visual da seleção | Percentil 95 de até 100 ms | Sem bloquear a fila de entrada |
| Seleção até início da fala local | Percentil 95 de até 500 ms | Motor aquecido; medir também a primeira fala separadamente |
| Operação sem rede | Todos os fluxos essenciais aprovados | Modo avião, reinício e uso prolongado |
| Integridade dos dados | Nenhuma perda nos testes de falha definidos | Interrupção de escrita, atualização e restauração |

Esses números são metas de engenharia propostas, não limiares clínicos nem desempenho já demonstrado. Se a voz do sistema não atingir uma meta, investigar o impacto real e a viabilidade técnica antes de anunciar o requisito como cumprido.

Testar também armazenamento quase cheio, bateria baixa, chamadas, saída Bluetooth, mudança de orientação e retorno após o sistema encerrar o aplicativo. Preservar a frase em composição conforme a preferência de privacidade. Oferecer uma prancha impressa de reserva e um procedimento simples de recuperação.

---

[← 9](09-arquitetura-e-decisao-sobre-a-base.md) · [Índice](README.md) · [Fontes](fontes.md) · [11 →](11-dados-portaveis-e-protecao.md)
