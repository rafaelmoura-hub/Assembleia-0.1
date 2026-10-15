# Assembleia Digital

Protótipo responsivo de assembleias e votações online, feito em HTML, CSS e JavaScript sem dependências de build.

## Acessar

- Administração: `adm/adm.html`
- Participante: `cliente/cliente.html`
- Acesso inicial do administrador: usuário `111111`, senha `1111`

Abra as páginas pelo mesmo servidor de arquivos e pela mesma origem (por exemplo, hospede a pasta inteira em um servidor web). O painel administrativo gera links de convite com código para compartilhar com os participantes.

## O que está incluído

- Criação de assembleias com data, horário, prazo de votação, pautas, regra de aprovação, visibilidade de resultados e quórum mínimo.
- Cadastro autônomo de participantes por CPF, e-mail e senha ao abrir um link válido de assembleia; o painel administrativo consulta a lista de cadastros.
- Link público por código de convite, identificação, voto Sim/Não/Abstenção, consulta de apuração e download de comprovante.
- O painel pode preparar mensagens de convite e resultado no aplicativo de e-mail padrão; o participante também pode preparar um e-mail com o comprovante ou a apuração.
- Painel com indicadores, quórum, lista de reuniões, relatórios e exportação CSV.
- Layout adaptável para celular e computador.

## Limites desta versão

Esta entrega é um protótipo de front-end: os dados ficam no `localStorage` do navegador e as senhas são armazenadas localmente sem proteção. O cadastro feito por um link público só fica disponível no mesmo navegador/origem neste protótipo; visitantes em outros dispositivos não compartilham os mesmos cadastros ou votos sem um backend. Os botões de e-mail apenas abrem uma mensagem preenchida no programa de e-mail do usuário; não enviam notificações automaticamente. Para uso real, será necessário conectar um backend com banco de dados, proteção de credenciais e dados pessoais, controle de acesso, trilha de auditoria, serviço de e-mail e serviço de assinatura. Não use esta versão para assembleias oficiais nem para armazenar CPFs reais.
