Ideathon INOVA SAÚDE 2026 — Requisitos
Foram escolhidas duas soluções entre as apresentações finalistas: Dose Certa e VozVital. A escolha considera que ambas apresentam problemas claros e propõem funcionalidades que podem ser representadas em casos de uso.
1. Dose Certa
Descrição da solução: organizador de medicamentos conectado a um aplicativo. O sistema avisa o horário da dose, acende a luz do compartimento correto e alerta um familiar quando o paciente não confirma que tomou o medicamento.
Diagrama de casos de uso (UML)
![Diagrama UML de casos de uso — Dose Certa](dose-certa-casos-de-uso.svg)
Caso de uso 1 — Cadastrar medicamento e horários
História de usuário: Como paciente, quero cadastrar meus medicamentos e os horários de cada dose, para receber lembretes nos momentos corretos.
Critérios de aceitação:
Dado que o paciente está na área de cadastro, quando informa o nome do medicamento e os horários, então o sistema salva essas informações.
Dado que existem campos obrigatórios sem preenchimento, quando o paciente tenta salvar o cadastro, então o sistema informa quais dados faltam.
Dado que o medicamento foi cadastrado, quando o paciente consulta sua lista, então o medicamento e seus horários aparecem corretamente.
Caso de uso 2 — Confirmar dose tomada
História de usuário: Como paciente, quero confirmar que tomei a dose, para manter meu histórico atualizado e evitar alertas desnecessários para meu familiar.
Critérios de aceitação:
Dado que existe uma dose programada, quando o paciente confirma que tomou o medicamento, então o sistema registra a confirmação com data e horário.
Dado que a dose está aguardando confirmação, quando o paciente não confirma dentro do período configurado, então o sistema envia um alerta ao familiar cadastrado.
Dado que a dose já foi confirmada, quando o paciente tenta confirmar novamente a mesma dose, então o sistema mantém apenas um registro de confirmação para aquela dose.
---
2. VozVital
Descrição da solução: aplicativo em que a técnica de enfermagem identifica o paciente pela pulseira e dita os sinais vitais. O aplicativo transcreve os valores, avisa quando algo está fora do normal e envia os dados ao prontuário.
Diagrama de casos de uso (UML)
![Diagrama UML de casos de uso — VozVital](vozvital-casos-de-uso.svg)
Caso de uso 1 — Identificar paciente pela pulseira
História de usuário: Como técnica de enfermagem, quero identificar o paciente pela leitura da pulseira, para registrar os sinais vitais no prontuário correto.
Critérios de aceitação:
Dado que a técnica está na tela de identificação, quando lê a pulseira do paciente, então o sistema apresenta os dados de identificação encontrados.
Dado que a leitura não reconhece uma pulseira válida, quando a técnica tenta identificar o paciente, então o sistema informa que não foi possível localizar o cadastro.
Dado que o paciente foi identificado, quando a técnica inicia o registro dos sinais vitais, então o sistema associa os próximos dados ao paciente selecionado.
Caso de uso 2 — Registrar sinais vitais por voz
História de usuário: Como técnica de enfermagem, quero ditar os sinais vitais do paciente, para registrar as informações mais rapidamente e reduzir a digitação manual.
Critérios de aceitação:
Dado que o paciente está identificado, quando a técnica dita os valores dos sinais vitais, então o aplicativo transcreve os dados para conferência.
Dado que a transcrição foi realizada, quando um valor está fora da faixa esperada configurada, então o aplicativo destaca esse valor para chamar a atenção da profissional.
Dado que a técnica conferiu e confirmou os valores transcritos, quando finaliza o registro, então o sistema envia os dados ao prontuário do paciente.
---
Observação
Os casos de uso e critérios de aceitação foram elaborados a partir das descrições das soluções no material INOVA SAÚDE 2026: as 15 soluções. Detalhes operacionais que não aparecem no material, como o período para disparo de alerta ou as faixas de referência dos sinais vitais, precisam ser definidos com os responsáveis pelo produto e pela área de saúde.
