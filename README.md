<div align="center">

<img width="1650" height="560" alt="capa-fila-certa" src="https://github.com/user-attachments/assets/fac1a91b-8aa0-4380-8006-1e53ef627d2b" />

# Fila Certa


### Seu horário organizado, seu atendimento no tempo certo

Projeto acadêmico da disciplina **Análise de Projeto e Sistemas**

</div>

---

## Sobre o projeto

O **Fila Certa** é a proposta de um sistema web para organizar os agendamentos de salões de beleza e barbearias independentes. O projeto parte de uma situação comum: horários anotados em lugares diferentes, marcações duplicadas, cancelamentos de última hora e dificuldade para preencher vagas que ficaram livres.

A proposta centraliza serviços, profissionais e horários em uma agenda. Quando um atendimento é cancelado, o sistema pode oferecer a vaga a uma pessoa compatível na lista de espera.

> **Importante:** este repositório apresenta o planejamento técnico e acadêmico do sistema. A aplicação ainda não foi implementada; tecnologias, metas e fluxos descritos são decisões e critérios propostos para orientar uma implementação futura.

## A disciplina e o objetivo do trabalho

Na disciplina **Análise de Projeto e Sistemas**, a equipe pratica como transformar um problema em uma especificação que possa orientar o desenvolvimento de software. O trabalho percorre concepção, requisitos, arquitetura, diagramas, banco de dados, planejamento, documentação técnica, qualidade e processo.

O objetivo não é entregar um sistema pronto, mas demonstrar que as decisões se conectam: as necessidades das pessoas orientam as funcionalidades; as funcionalidades orientam a arquitetura e os dados; e o planejamento define como a equipe poderia construir e verificar a solução.

## O que a proposta contempla

- Cadastro de clientes, serviços e profissionais.
- Configuração de expediente semanal, folgas e bloqueios.
- Consulta de horários compatíveis com serviço e profissional.
- Marcação e cancelamento de atendimentos.
- Lista de espera e oferta temporária de horários liberados.
- Registro de atendimentos concluídos ou faltas.
- Consulta de agenda e resumo diário de ocupação.

Pagamento, prontuário, aplicativo nativo, franquias, mensagens automáticas e integrações com redes sociais estão fora do escopo inicial.

## Visão da arquitetura

O piloto foi pensado para um estabelecimento. Uma aplicação web modular atende clientes e equipe; uma API concentra as regras; e o banco relacional mantém agenda, cadastros e histórico.

<img width="2400" height="1500" alt="c4-contexto" src="https://github.com/user-attachments/assets/c0e6a664-64a5-49c8-b32f-94af1128db23" />

### Tecnologias planejadas

| Parte | Tecnologia proposta | Papel no projeto |
|---|---|---|
| Interface web | HTML, CSS e JavaScript | Apresentar agenda e permitir as ações dos usuários |
| API e regras | Java 21 com Spring Boot | Validar acesso, disponibilidade, marcações e lista de espera |
| Banco de dados | PostgreSQL 16 | Guardar os dados e proteger a agenda contra sobreposições |
| Contrato da API | OpenAPI 3.0 | Descrever operações, dados e respostas esperadas |
| Versionamento | Git e GitHub | Registrar mudanças e permitir revisão colaborativa |

Essas tecnologias fazem parte do desenho proposto; a implementação ainda não existe neste repositório.

## Equipe

- Tatyanne Guedes
- Lavynia Monteiro
- Daniel Costa

---

<div align="center">

**Fila Certa** · Projeto acadêmico · 2026

</div>
