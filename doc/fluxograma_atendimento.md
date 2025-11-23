# Fluxograma do Processo de Atendimento

Este documento descreve o fluxo de ponta a ponta do sistema de triagem hospitalar.

Fluxograma visual:  
`fluxograma.png`

## Etapas

### 1. Cadastro do Paciente
Dados preenchidos:
- nome
- prioridade
- sintomas
- outros atributos

### 2. Inserção na Fila de Prioridade
Organiza os pacientes por:

- prioridade (menor número = mais urgente)
- desempate por hora de chegada

### 3. Chamar Próximo
O sistema sempre remove o elemento de maior prioridade.

### 4. Atendimento
O paciente pode:
- ser finalizado → vai para o histórico (stack LIFO)
- ser retornado ao anterior (volta do histórico)

### 5. Histórico (Stack)
Armazena atendimentos concluídos.
