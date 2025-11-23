# Sistema de Triagem Hospitalar  
Documentação Técnica

Este projeto implementa um sistema de triagem hospitalar que organiza pacientes com base em prioridades e mantém histórico de atendimento.  

## Estrutura Geral

- **CORE** → Classes principais do domínio  
- **DATA** → Persistência e estruturas de dados  
- **SERVICES** → Regras de negócio e integração  
- **GUI** → Interface com o usuário  
- **DOCUMENTAÇÃO** → Descrições, diagramas e fluxos  

## Fluxo Geral

1. Cadastro do paciente  
2. Inserção na fila de prioridades  
3. Chamada do próximo paciente  
4. Atendimento  
5. Registro no histórico (Stack LIFO)  

O fluxograma completo pode ser visto em:  
**fluxograma_atendimento.md**
