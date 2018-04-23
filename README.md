# Changelog
Todas as alteraçṍes notáveis deste projeto serão documentadas aqui.

Changelog baseado no formato criado por [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
este projeto usa [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [1.6] - 2018-03-14
### Adicionado

- Quadro - Adiciona Visao de Kanban
- Funcao e Nivel
- Nova tela de Permissoes
- Nova Visao na Tela de Permissao
- UsuarioController/Service/Repository - ranking em grupo favorito, M - UsuarioController/Service refatoracao busca de ranking
- inicio visao filtros, inicio refatoracao ranking para adicionar grupo favorito
- modificando fluxo de adicioanar usuario no projeto
- Adicao de Feedback ao adicionar um grupo como favorito na tela de Resultados Ulitizando o componente SnackBar
- Padronização de Icones Tela de Perfil e Remoção de Atalho no Page Header
- Inicia criacao de constantes de textos 
- Visao geral projeto - terminada versão 1
- Favoritar Grupos - Possibilidade de favoritar um grupo
- recursividade na busca de resultados de grupos relacionados a um usuario
- menu lateral - Alteracao nos botoes de criacao de grupos, quadros e projetos, limpeza no codigo do main
- Menu lateral - mover quadros entre grupos e pastas
- Grupo Favorito completo
- Grupo Favorito - Inicio Grupo favorito, M - Resultados Grupos - Mudanca Logica de Total, Retirando Group Bys Desnecessários
- Menu lateral - nova logica de drag e hover para abrir items
- nova query para buscar todos os grupos com usuarios de uma empresa
- Continuação Roteamento Grupos
- Busca de Resultados de Grupos para Membro, inicio Roteamento da tela
- visao de projetos - inclui opção de excluir etapas

### Alterado

- visão projeto - corrigindo cliques e colocando opção de editar etapas dentro da visão do projeto
- Nova paleta de cores
- arrumando bug de mostrar feedback de erro quando deletar lista
- Correção do Botão Do Cardapio
- Quadro Pessoal -  Permissao de Criador Em Caixa de Entrada
- Tarefa detalhe - Erros de Tarefa Detalhe
- Mudanca de Icones - Novo Padrao
- Perfil - Concertando cagada na lógica de grupo pra usuário
- Tela de Perfil, visao da posicao no grupo favorito
- UsuarioController/Service refatoracao busca de ranking
- Correção varios usuarios no mesmo grupo, passando Cargo para tipo usuarios empresa
- cardapio - fazer aparecer projetos para pessoas relacionadas aquele grupo
- correcao query de buscar grupos de usuario
- verificacao se usuario existe antes de adicionar em projeto
- mensagens de erro como constantes
- Fix enviar grupo completo para o front
- rota de arquivar quadro - corrigindo tratamento para etapas de projeto
- Permissoes - Resolvendo problema de busca de usuarios e descomentando o usuario.service que alguem comentou por algum motivo desconhecido
- QuadroService/Cardapio - fazendo mandar via websockets CRUD de etapas do projeto
- consertando operações de etapas para serem enviadas pelo websocket
- Montando Favoritos de Grupo
- filtros de dia corretamente
- buscas de resultados com recursividade
- pasta/grupo - adiciona arquivos faltando
- acompanhamento de projeto - ordenar etapas por data de entrega
- Tela de Permissão - Melhorias na Visao
- Resultados Grupos - Mudanca Logica de Total, Retirando Group Bys Desnecessários.
- Alteracoes em Permissoes e Grupo
- corrigindo mudança de meses da tela de criação de projetos
- mostrar erro quando escrever motivo menor q 5
- central notificacao - corrige nao abrindo
- bugs de texto e permissoes em projetos
- Modificações na Tela de Perfil
- mudanca rotas para facilitar desenvolvimento futuro
- mudanca na logica de buscar resultados de grupos
- Usuario service - remove valor fixo de usuario
- Notificacao Service - corrige usuario recebendo notificacoes de si mesmo
- QuadroEstatico - remove consolelogs e debugger
- QuadrosEstaticos - Corrige erro de renderização de tarefas membro, responsavel, dono e favoritas


## [1.5.0] - 2018-03-14
### Adicionado

- Central de Notificações, aqui chegarão todos as atualizações de tarefas que você participa.
- Projetos, agora você pode criar projetos com etapas e objetivos e acompanhar o progresso da sua equipe
- Nova tela de gerenciamento de permissões, administradores de grupos podem gerenciar mais facilmente os
níveis de permissões dos membros dos grupos.
- Nova tela de acompanhamento de grupo com uma síntese da atividade dos membros


### Alterado

- Nova paleta de cores



## [1.1.0] - 2018-03-14
### Adicionado

- Lixeira, onde é possível restaurar tarefas, listas, quadros ou grupos deletados
- Indicador do nível de prioridade por cores na lateral esquerda da tarefa
- Tour guiado pelas principais funções do Chord. Acessível pelo botão "Tour" ao lado do calendário
- Contador de tarefas na lista


### Alterado

- Nova paleta de cores
- Correções no layout da tela de Perfil
- Corrigido bug de pausar tarefa e perder status de subtarefas
- Nova ilustração na tela de Login





## [1.0.0] - 2018-02-28
### Adicionado
- WEBSOCKET adicionado, alterações agora acontecem em tempo real para todos os envolvidos (participantes de tarefas, quadros, pastas ou grupos)
- Ao inserir o primeiro membro de uma tarefa, este será atribuído também como responsável
- Opção de deletar comentários
- Novo menu contextual responsivo que se posiciona de acordo com espaço disponível em tela
- Novo indicador de nível de prioridade das tarefas
- Possível remover a responsabilidade de um usuário em uma tarefa
- Pausar tarefas. No menu de data agora é possível pausar uma tarefa, fornecendo uma justificativa para a interrupção.


### Alterado 
- Novo visual de mensagens
- Nova animação de loading
- Nova notificação de atualização disponível
- Subtarefas concluídas continuam visíveis (experimental)
- Durante a criação de tarefas ou subtarefas o texto não é mais perdido caso a input perca o foco
- Ultima mensagem não fica mais atrás da caixa de input
- AutoComplete desabilitado para a caixa de busca de usuários
- Nova Fonte
- Corrigido problema de cache de imagens





## [0.4.0] - 2018-02-24
### Adicionado
- Agora é possível mover tarefas entre quadros. Arrastar a tarefa sobre um quadro no menu lateral 
    abre este quadro e é possível soltar a tarefa na lista desejada.
- Novos ícones de atalho e de notificação
- Campo de busca no menu lateral (Grupos, Pastas, Quadros)
- Hover para leitura de títulos longos sem ser necessário abrir a tarefa


### Alterado
- Campo de mensagens alterado para textArea. Agora é possível dar scroll e visualizar todo o texto digitado.
- Visão detalhada da tarefa não esconde mais as tarefas concluídas
- Comportamento da área de adição de membros na tarefa (Ao clicar para adicionar um membro a area de usuários não fecha mais)
- Corrigido alinhamento de itens da área de adição de membros
- Campos de nova tarefa, subtarefa e lista agora possuem foco ao abrir
- Novo posicionamento da data e quantidade de subtarefas nas tarefas

### Removido
- XXXXX


## [0.3.2] - 2018-02-17
### Adicionado
- Nova tela de login com nova identidade visual Chord.
- Nova Iconografia
- Agora é possível colocar links nos comentários e na descrição da tarefa.
- Novo indicador de presença de comentários e anexos na tarefa. 
- Tarefas agora possuem data de início e fim.
- Links diretos para quadros e pastas. Todo quadro e tarefa gera um link único compartilhável que pode ser usado para acessar tarefas e quadros específicos. É necessário estar logado e ter permissão de visualização na tarefa e quadro.
- Nova opção de observar/seguir tarefas

### Alterado
- Filtro de busca de usuários apenas na mesma empresa.
- Filtro de busca de usuários buscando apenas por nome, caso a busca inicie com @ busca feita por apelido.
- Deletar uma tarefa agora fecha a mesma caso estiver aberta.
- Usuário que está criando a pasta agora aparece por default na lista de membros.
- Histórico agora é exibido em ordem cronológica
- Conserta ordem inversa de subtarefas
- Conserta token de acesso vencido impedindo carregamento da aplicação.
- Conserta cardápio permanecendo após clique em quadro selecionado

### Removido
- Opção equivocada de "Tornar Responsável" no quadro.
