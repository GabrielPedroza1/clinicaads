# Sistema de Agendamento Médico

## Objetivo
- Cadastro de usuários
- Controle da disponibilidade dos médicos
- Definição da janela de consultas
- Agenda diária e semanal
- Exibição de mensagens claras e objetivas

## Escopo

### Incluído (In)
- Cadastro de usuários
- Disponibilidade dos médicos
- Definição da janela de consultas
- Agenda diária e semanal
- Exibição de mensagens claras

### Excluído (Out)
- Agendamento em domicílio
- Sistema de notificações
- Prontuário eletrônico
- Relatórios avançados
- Suporte a múltiplas clínicas

## Regras de Negócio (RB)
- **RB-001**: Slots de horário não podem se sobrepor a outros já ocupados
- **RB-002**: Consultas só podem ocorrer dentro da janela de atendimento do profissional
- **RB-003**: Cancelamento deve liberar o slot imediatamente
- **RB-004**: A duração padrão da consulta é de 30 minutos

## Premissas
- Horário comercial: 08:00 às 18:00
- MVP limitado a 10 profissionais
- Banco de dados com até 500 pacientes

## Stakeholders
1. Atendentes
2. Médicos
3. Pacientes
4. Gestor da clínica
