# Desafio oficina

Projeto Conceitual - Sistema de Gestão de Ordem de Serviço para Oficina Mecânica
1. Visão Geral
Este projeto visa modelar um Sistema de Controle e Gerenciamento de Ordens de Serviço (OS) para uma oficina mecânica. O sistema permitirá o acompanhamento de veículos, mecânicos, serviços e peças utilizadas em cada OS, garantindo uma gestão eficiente e organizada do fluxo de trabalho.

2. Objetivo
Criar um banco de dados estruturado para gerenciar o fluxo de trabalho da oficina mecânica, incluindo:
✅ Cadastro de clientes e veículos.
✅ Registro de ordens de serviço (OS), incluindo status e histórico de alterações.
✅ Atribuição de mecânicos responsáveis por cada OS.
✅ Controle de peças e mão de obra utilizadas nos serviços.
✅ Registro de serviços realizados e valores correspondentes.

3. Estrutura do Banco de Dados
A modelagem do banco de dados foi baseada na narrativa fornecida e estruturada da seguinte forma:

3.1. Principais Entidades
Clientes: Representa os clientes da oficina. Cada cliente pode possuir múltiplas ordens de serviço.
Ordem de Serviço (OS): Representa os serviços solicitados pelo cliente para um veículo. Possui um número único, data de emissão, status atual e um valor total.
Mecânicos: Armazena os dados dos mecânicos responsáveis pela execução dos serviços.
Serviços: Contém os diferentes tipos de serviços oferecidos, como revisão e conserto.
Peças: Representa as peças utilizadas na execução dos serviços.
Mão de Obra: Contabiliza os custos de trabalho realizados pelos mecânicos.
Status: Define o estágio da OS, como "Aguardando Aprovação", "Em Execução", "Finalizada" etc.
3.2. Relacionamentos
Cada cliente pode possuir múltiplas ordens de serviço (OS).
Cada OS está vinculada a um status, indicando sua fase no processo.
Uma OS pode incluir vários serviços, que podem ser executados por um ou mais mecânicos.
Para cada OS, há um controle sobre as peças e mão de obra utilizadas.
Cada mecânico pode estar envolvido em várias OS, e cada OS pode ter múltiplos mecânicos.
