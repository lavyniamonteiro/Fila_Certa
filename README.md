<div align="center">

![Capa do Fila Certa](docs/diagramas/capa-fila-certa.png)

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

![Diagrama de contexto do Fila Certa](docs/diagramas/c4-contexto.png)

### Tecnologias planejadas

| Parte | Tecnologia proposta | Papel no projeto |
|---|---|---|
| Interface web | HTML, CSS e JavaScript | Apresentar agenda e permitir as ações dos usuários |
| API e regras | Java 21 com Spring Boot | Validar acesso, disponibilidade, marcações e lista de espera |
| Banco de dados | PostgreSQL 16 | Guardar os dados e proteger a agenda contra sobreposições |
| Contrato da API | OpenAPI 3.0 | Descrever operações, dados e respostas esperadas |
| Versionamento | Git e GitHub | Registrar mudanças e permitir revisão colaborativa |

Essas tecnologias fazem parte do desenho proposto; a implementação ainda não existe neste repositório.

## Como o trabalho está organizado

| Caminho | Conteúdo |
|---|---|
| [`docs/Fila-Certa-final.docx`](docs/Fila-Certa-final.docx) | Documento editável com os blocos do trabalho e diagramas |
| [`docs/projeto-final.md`](docs/projeto-final.md) | Fonte Markdown do documento técnico |
| [`docs/guia-simples-do-projeto-fila-certa.md`](docs/guia-simples-do-projeto-fila-certa.md) | Explicação do projeto em linguagem simples |
| [`docs/guia-simples-do-enunciado.md`](docs/guia-simples-do-enunciado.md) | Explicação dos blocos e termos pedidos pelo professor |
| [`docs/diagramas/`](docs/diagramas/) | Diagramas C4, UML e modelo entidade-relacionamento |
| [`docs/openapi.yaml`](docs/openapi.yaml) | Especificação formal proposta para a API |
| [`database/V1__core.sql`](database/V1__core.sql) | Estrutura inicial proposta para o banco de dados |
| [`docs/dicionario-de-dados.md`](docs/dicionario-de-dados.md) | Significado e características dos campos do banco |

## Como conferir os artefatos

Para validar a estrutura do contrato da API, com Python e as dependências do projeto disponíveis, execute:

```bash
python scripts/validate_openapi.py
```

O esquema SQL pode ser aplicado somente em um banco PostgreSQL de teste vazio. A aplicação web, o Compose de desenvolvimento e os testes da aplicação serão criados em uma etapa futura.

## Equipe

- Tatyanne Guedes
- Lavynia Monteiro
- Daniel Costa

---

<div align="center">

**Fila Certa** · Projeto acadêmico · 2026

</div>
