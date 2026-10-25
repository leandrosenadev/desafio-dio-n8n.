# Desafio DIO — Planejando Automações com n8n Usando Apenas Bons Prompts

## Prompt final

Atue como um especialista em n8n e explique a solução de forma clara, organizada e adequada para uma pessoa iniciante.

Crie uma automação no n8n para receber, validar e registrar automaticamente contatos enviados por meio de um formulário, além de notificar a pessoa responsável pelo atendimento.

**Público:**
Pequenas empresas e equipes comerciais que precisam organizar contatos de potenciais clientes e acompanhar novos pedidos de contato.

**Ferramentas envolvidas:**
- n8n, para coordenar o workflow;
- Google Forms, para receber os dados dos contatos;
- Google Sheets, para armazenar os contatos válidos;
- Gmail, para enviar notificações por e-mail.

**Fluxo desejado:**
1. Detectar ou receber uma nova resposta enviada pelo Google Forms, explicando qual gatilho ou método de integração pode ser usado no n8n.
2. Obter os dados da resposta e verificar se os campos obrigatórios foram preenchidos.
3. Validar se o endereço de e-mail informado possui um formato válido.
4. Se os dados forem válidos, registrar o contato em uma planilha do Google Sheets.
5. Somente depois de confirmar o registro bem-sucedido, enviar uma notificação por Gmail à pessoa responsável pelo atendimento, informando que um novo contato foi registrado.
6. Se os dados forem inválidos, não registrar o contato e enviar uma notificação de erro para a pessoa responsável pela análise.
7. Se ocorrer uma falha ao registrar os dados ou ao enviar uma notificação, permitir identificar o ponto da falha e obter informações úteis para corrigir o problema.

**Regras e restrições:**
- Nome e e-mail são campos obrigatórios.
- Não registrar contatos com e-mail em formato inválido.
- Manter os dados organizados na planilha.
- Enviar a notificação de novo contato somente após o registro bem-sucedido no Google Sheets.
- Não tratar uma operação como bem-sucedida se ela retornar erro.
- Explicar como identificar e tratar falhas, sem ocultar mensagens de erro.
- Não presumir que as integrações e credenciais já estejam configuradas. Indicar quais credenciais e permissões precisam ser preparadas.
- Se o recebimento direto de respostas do Google Forms não estiver disponível na configuração proposta, apresentar uma alternativa viável e explicar suas limitações.

**O que preciso na resposta:**
1. Liste os nós do n8n necessários e a função de cada um.
2. Explique a sequência do workflow e como conectar os nós.
3. Mostre como separar o caminho dos dados válidos do caminho dos dados inválidos.
4. Explique como configurar as integrações com Google Forms, Google Sheets e Gmail, incluindo as credenciais necessárias.
5. Explique como identificar falhas no registro e no envio de e-mails.
6. Apresente um roteiro simples para testar o workflow com um contato válido, um e-mail inválido e uma falha simulada.
7. Use linguagem simples, passo a passo, sem presumir experiência prévia com n8n.
