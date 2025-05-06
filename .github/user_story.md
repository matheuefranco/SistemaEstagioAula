name: 📘 História de Usuário
description: Descreva uma funcionalidade do ponto de vista do usuário seguindo o modelo ágil (Scrum)
title: "[USXX] "
labels: [user-story]
assignees: ''

body:
  - type: markdown
    attributes:
      value: |
        Obrigado por contribuir com o projeto! Preencha os campos abaixo para descrever esta história de usuário.

  - type: input
    id: user-story-id
    attributes:
      label: ID da História
      description: Defina um identificador único para esta história (ex: US01, US02...)
      placeholder: "US01"
    validations:
      required: true

  - type: textarea
    id: descricao
    attributes:
      label: 📌 Descrição
      description: Use a estrutura "Como [tipo de usuário], quero [ação] para [benefício]"
      placeholder: |
        Exemplo:
        Como analista de dados,
        Quero consultar as informações meteorológicas das estações cadastradas,
        Para que eu possa analisar as tendências climáticas da região.
    validations:
      required: true

  - type: textarea
    id: criterios
    attributes:
      label: ✅ Critérios de Aceitação
      description: Liste os critérios que validam que a história foi implementada com sucesso
      placeholder: |
        - A API deve retornar os dados dos últimos 3 dias
        - Os dados devem ser armazenados em arquivos .txt
        - A resposta deve incluir temperatura, umidade, chuva, etc.
    validations:
      required: true

  - type: textarea
    id: tarefas
    attributes:
      label: 🛠️ Tarefas
      description: Liste as tarefas técnicas necessárias para implementar esta história
      placeholder: |
        - [ ] Criar endpoint `/stations`
        - [ ] Consumir API externa Plugfield
        - [ ] Salvar arquivos por estação
    validations:
      required: true

  - type: textarea
    id: requisitos
    attributes:
      label: 📎 Requisitos Não-Funcionais
      description: Inclua aspectos como desempenho, segurança, compatibilidade, etc. (opcional)
      placeholder: |
        - O tempo de resposta da API deve ser inferior a 3 segundos
        - O arquivo deve ser salvo localmente em UTF-8
      required: false

  - type: textarea
    id: dependencias
    attributes:
      label: 🔗 Dependências
      description: Indique se esta história depende de outras histórias, tarefas ou componentes
      placeholder: |
        - Depende da [US00] Configuração da conexão com a API
      required: false