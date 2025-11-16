# arquivos-guilds

<chapter id="arquivos-guilds" title="Arquivos" collapsible="true">
    <chapter title="lang/" collapsible="true">
        <chapter title="messages_pt" collapsible="true">
<code-block lang="yaml">
menus:
  permission:
    leader: '&cNecessário ser Líder'
    moderator: '&cNecessário ser Moderador'
    recruiter: '&cNecessário ser Recrutador'
    allowed: '&eClique para gerenciar'

discord:
buttons:
link:
name: https://discord.gg/%discord%
description: '&7Entrar no Discord'
update:
name: '&e[Alterar]'
description: '&aClique para atualizar'
usage: '{n}&9Escreva no chat o link do Discord.{n}&7Você pode cancelar escrevendo &c&ncancel{n}&r '
update: '{n}&a&lDISCORD ATUALIZADO!{n}&r&fDiscord atualizado para:{n}&ahttps://discord.gg/%discord%{n}&r '
message: '{n}&9&lNOSSO DISCORD {update}{n}&r&fEntre em nosso Discord:{n}&a{link}{n}&r '

guilds:
notifications:
server-guild-created: '{n}&e&l(!) %guild_colortag% &fAcaba de ser fundada por &f%player_displayname%&f!{n}&r '
server-guild-deleted: '{n}&e&l(!) %guild_colortag% &fFoi excluida por &f%player_displayname%&f!{n}&r '

    guild-delete: '{n}&c&l(!) GUILDA EXCLUIDA{n}&r&7Sua Guilda %guild_colortag% &7foi excluida.{n}&r '
    guild-upgrade: '%guild_colortag% &a[+] &7A Guilda foi aprimorada por &f%author%&7!'
    join-server: '%guild_colortag% %role_prefix% &f%player% &7entrou neste servidor.'
    new-member: '%guild_colortag% &a[+] &7O jogador &f%player% &7se juntou a Guilda!'
    leave-member: '%guild_colortag% &c[-] &7O jogador &f%player% &7abandonou a Guilda!'
    kick-member: '%guild_colortag% &c[!] &7O membro &f%player% &7foi &cexpulso(a) &7da Guilda por &f%author%&7!'
    promote-member: '%guild_colortag% &b[+] &f%player% &7foi &bpromovido(a) &7para %role_color%%role_name%&7!'
    demote-member: '%guild_colortag% &e[-] &f%player% &7foi &erebaixado(a) &7para %role_color%%role_name%&7!'
    transfer-member: '%guild_colortag% &b[+] &7A posse de &f%role_prefix% &7de &f%leader% &7foi &btransferida &7para &f%player%&7!'

online:
result: '{n}&eMembros online: &r%online%{n} '
not-in-guild: '&cVocê não está em uma guilda.'

chat:
command-usage: <mensagem> para enviar uma mensagem.
not-in-guild: '&cVocê não está em uma guilda.'

info:
not-in-guild: '&cVocê não está em uma guilda.'

transfer:
buttons:
time:
name: '%time%'
description: '&7Desde &f%joined_at%'
confirm:
name: CONFIRMAR
description: '&aConfirmar transferência'
not-in-guild: '&cVocê não está em uma guilda.'
no-permission: '&cApenas o Líder pode transferir a posse para outro membro.'
title:
title: '&b&lNOVO LÍDER'
subtitle: '&f%player% se tornou o novo líder!'
leader:
command-usage: <jogador> para transferir sua posse.
confirm: '{n}&b&l(!) TRANSFERIR POSSE{n}&r&7Deseja transferir a posse de &f%guild_name% &f%guild_colortag% &7para &f%player%&7?{n}&r&7O membro faz parte da Guilda há &b{time}&7.{n}&r&c(!) Essa ação é irreversível e você será rebaixado.{n}&r&a&l{confirm}{n} '
target-is-you: '&cVocê já é o líder da Guilda.'
player-new-member: '&cA posse só pode ser transferida a Membros que estejam pelo menos há &f7 dias&c. Este jogador está há &f{time}&c.'
player-not-in-guild: '&cEste jogador não está na Guilda.'

promote:
not-in-guild: '&cVocê não está em uma guilda.'
no-permission: '&cApenas o Líder pode promover outros membros.'
title:
title: '&b&lPROMOVIDO'
subtitle: '&f%player% &ffoi promovido a &a%role_prefix%'
leader:
command-usage: <jogador> para promover um membro.
target-is-you: '&cVocê não pode alterar o seu cargo.'
player-max-role: '&cEste jogador já está no cargo máximo.'
player-not-in-guild: '&cEste jogador não está na Guilda.'

demote:
not-in-guild: '&cVocê não está em uma guilda.'
no-permission: '&cApenas o Líder pode rebaixar outros membros.'
title:
title: '&c&lREBAIXADO'
subtitle: '&f%player% &ffoi rebaixado para &a%role_prefix%'
leader:
command-usage: <jogador> para rebaixar um membro.
target-is-you: '&cVocê não pode alterar o seu cargo.'
player-min-role: '&cEste jogador já está no cargo mínimo.'
player-not-in-guild: '&cEste jogador não está na Guilda.'

kick:
buttons:
time:
name: '%time%'
description: '&7Desde &b%joined_at%'
confirm:
name: CONFIRMAR
description: '&aConfirmar expulsão'
not-in-guild: '&cVocê não está em uma Guilda.'
no-permission: '&cApenas moderadores+ podem expulsar outros jogadores.'
player:
title:
title: '&c&lEXPULSO'
subtitle: '&fVocê foi expulso da Guilda!'
message: '{n}&c&l(!) EXPULSO DA GUILDA{n}&r&7Você foi expulso de &f%guild_name% &f%guild_colortag%&7{n}&r&7Expulso por: &f%author%{n} '
moderator:
confirm: '{n}&c&l(!) EXPULSAR MEMBRO{n}&r&7Deseja expulsar &f%player% &7de &f%guild_name% &f%guild_colortag%&7?{n}&r&7O membro faz parte da Guilda há &b{time}&7.{n}&a&l{confirm}{n} '
command-usage: <jogador> para expulsar um membro.
no-permission: '&cVocê não pode expulsar este jogador, pois ele possui um cargo igual ou maior que o seu.'
player-not-in-guild: '&cEste jogador não está na Guilda.'

delete:
buttons:
time:
name: '%time%'
description: '&7Criado em &b%creation%'
confirm:
name: CONFIRMAR
description: '&cConfirmar exclusão'
not-in-guild: '&cVocê não está em uma Guilda.'
no-permission: '&cApenas o líder pode excluir a Guilda.'
sucessfull: '&aVocê excluiu a Guilda com sucesso!'
confirm: '{n}&c&l(!) EXCLUIR A GUILDA{n}&r&7Deseja excluir &f%guild_name% &f%guild_colortag%&7?{n}&r&7A guilda possui uma história de &b{time}&7.{n}&c&l{confirm}{n} '

leave:
buttons:
time:
name: '%time%'
description: '&7Desde &b%joined_at%'
confirm:
name: CONFIRMAR
description: '&cConfirmar saída'
sucessfull: '&aVocê abandonou a Guilda com sucesso!'
the-leader: '&cVocê é o Líder da Guilda. Para abandona-la, sua posse deve ser transferida ou a Guilda deve ser excluida.'
not-in-guild: '&cVocê não está em uma Guilda.'
confirm: '{n}&b&l(!) SAIR DA GUILDA{n}&r&7Deseja abandonar &f%guild_name% &f%guild_colortag%&7?{n}&r&7Você faz parte da Guilda há &b{time}&7.{n}&c&l{confirm}{n} '

invites:
no-invites: '&cVocê não possui nenhum convite pendente.'
already-in-guild: '&cVocê já está em uma guilda.'

invite:
buttons:
accept:
name: ACEITAR
description: '&aAceitar convite'
deny:
name: RECUSAR
description: '&cRecusar convite'
not-in-guild: '&cVocê não está em uma Guilda.'
recruiter:
invite: '{n}&b&l(!) CONVITE DE GUILDA{n}&r&7Você convidou &f%player% &7para &f%guild_name% &f%guild_colortag%{n}&r&7O jogador possui &b%expires%&7 para aceitar.{n} '
command-usage: <jogador> para convidar um jogador.
no-permission: '&cApenas recrutadores+ podem convidar outros jogadores.'
searching-player: '{n}&a(!) &7Escreva no &a&nbate-papo&r &7o nome do jogador que deseja convidar!{n}&c(!) &7Ou escreva &c&ncancel&7 para cancelar.{n} '
player-already-in-guild: '&cO jogador já está em uma guilda.'
player-already-invited: '&cJá existe um convite pendente para este jogador.'
player:
accept-title:
title: '%colortag%'
subtitle: '&fVocê entrou na Guilda!'
receive: '{n}&b&l(!) CONVITE DE GUILDA{n}&r&7Você foi convidado para entrar em &f%guild_name% &f%guild_colortag%{n}&r&7Você possui &b%expires%&7 para aceitar.{n}&8&l> &a&l{accept} &8&l- &c&l{deny} &8&l<{n} '
accept: '&aVocê aceitou o convite para participar de &f%guild_name%&a.'
decline: '&cVocê recusou o convite para participar de &f%guild_name%&c.'
invite-not-found: '&cVocê não possui um convite pendente de ID #%id%.'
deny-command-usage: <id> para recusar um convite.
accept-command-usage: <id> para aceitar um convite.
already-in-guild: '&cVocê já está em uma guilda.'

creation:
buttons:
confirm:
name: CONFIRMAR
description: '&aConfirmar decisão'
retry:
name: ALTERAR
description: '&eTentar novamente'
cancel:
name: CANCELAR
description: '&cCancelar criação'
money:
name: MONEY
description: '&7Custará &e$%price% &7de seu Saldo'
cash:
name: CASH
description: '&7Custará &2$%price% &7de seu Cash'

    title:
      title: '%colortag%'
      subtitle: '&fVocê fundou sua Guilda!'
    
    select-name: '{n}&a(!) &7Escreva no &a&nbate-papo&r &7o nome que deseja para sua Guilda! &c&l{cancel}{n} '
    blocked-name: '&c(!) Não é permitido que o nome possua "%blocked%". Tente novamente.'
    name-special-char: '&c(!) Não é permitido que o nome possua caracteres especiais. Tente novamente.'
    name-space: '&c(!) Não é permitido que o nome possua espaços. Tente novamente.'
    name-length: '&c(!) O nome da guilda deve conter entre %min% e %max% caracteres. Tente novamente.'
    name-taken: '&c(!) Este nome já está sendo utilizado por uma Guilda. Tente novamente.'
    confirm-name: '&a(!) &7Deseja confirmar &f"%name%" &7como nome da Guilda?{n}&8&l> &a&l{confirm} &8&l- &e&l{retry} &8&l- &c&l{cancel} &8&l<'
    
    select-tag: '{n}&a(!) &7Escreva no &a&nbate-papo&r &7a TAG que deseja para sua Guilda! &c&l{cancel}{n} '
    blocked-tag: '&c(!) Não é permitido que a tag possua "%blocked%". Tente novamente.'
    tag-special-char: '&c(!) Não é permitido que a tag possua caracteres especiais. Tente novamente.'
    tag-space: '&c(!) Não é permitido que a tag possua espaços. Tente novamente.'
    tag-length: '&c(!) A tag deve conter entre %min% e %max% caracteres. Tente novamente.'
    tag-taken: '&c(!) Esta tag já está sendo utilizada por uma Guilda. Tente novamente.'
    confirm-tag: '&a(!) &7Deseja confirmar &f"%tag%" &7como tag da Guilda?{n}&8&l> &a&l{confirm} &8&l- &e&l{retry} &8&l- &c&l{cancel} &8&l<'
    
    confirm-price: '&a(!) &7Qual método de pagamento deseja utilizar?{n}&8&l> &e&l{money} &8&l- &a&l{cash} &8&l- &c&l{cancel} &8&l<'
    money-removed: '&a(!) &7Foi retirado do seu saldo de money &f$%cust% &7para a criação!'
    cash-removed: '&a(!) &7Foi retirado do seu saldo de cash &f$%cust% &7para a criação!'
    money-not-enough: '&c(!) Você não possui saldo de money o suficiente.'
    cash-not-enough: '&c(!) Você não possui saldo de cash o suficiente.'
    
    guild-created: '{n}&a(!) &7Guilda &a%name% &7[&f%tag%&7] &7criada com sucesso!{n}&7Defina suas preferências como &aícone &7e mais em &a/guild gerenciar{n} '
    cancelled: '&cCriação de guilda cancelada.'
    already-in-guild: '&cNão é possível criar uma guilda estando em uma.'
</code-block>
        </chapter>
    </chapter>
    <chapter title="menus/" collapsible="true">
        <chapter title="guild-info-menu.yml" collapsible="true">
<code-block lang="yaml">
# Informação da guilda que estiver
info-menu:
  title: "%name% - Guilda"
  slots: 6
  # Sinta-se a vontade para por novos itens
  # apenas respeite os ids padrões para o funcionamento correto

items:
g:
name: "&dGUILD"
item: "head:58c336dedfe197b434b5ab67988cbe9c2c9f285ec1871fdd1ba434855b"
slot: 1
lore: []
u:
name: "&eGUILD"
item: "head:9fdc4f321c78d67484135ae464af4fd925bd57d459383a4fe9d2f60a3431a79"
slot: 2
lore: []
i:
name: "&6GUILD"
item: "head:c148a8865bc4afe0747f3415138b96bbb4e8bbb7261f45e5d11d7219f368e4"
slot: 3
lore: []
l:
name: "&bGUILD"
item: "head:cc58321d4bffbec2ddf66bf38cf2f9e9ddf3fa2f1387dc7d30c62b4d010c8"
slot: 4
lore: []
d:
name: "&aGUILD"
item: "head:59aa69229ffdfa182889bf3097d32215c1b2159d987103b1d5843646faac"
slot: 5
lore: []


    # Itens extras
    # Vidro verde nos slots de 9 a 17
    glass_1:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 9
      lore: []

    glass_2:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 10
      lore: []

    glass_3:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 11
      lore: []

    glass_4:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 12
      lore: []

    glass_5:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 13
      lore: []

    glass_6:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 14
      lore: []

    glass_7:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 15
      lore: []

    glass_8:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 16
      lore: []

    glass_9:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 17
      lore: []

    # Vidro verde nos slots de 36 a 44
    glass_10:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 45
      lore: []

    glass_11:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 46
      lore: []

    glass_12:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 47
      lore: []

    glass_13:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 48
      lore: []

    glass_14:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 49
      lore: []

    glass_15:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 50
      lore: []

    glass_16:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 51
      lore: []

    glass_17:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 52
      lore: []

    glass_18:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 53
      lore: []

    icon:
      name: "%colortag%"
      item: "%icon%"
      slot: 7
      lore:
        - "%description%"
        - ""
        - "&eInformações:"
        - " &a▸ &fNome: &a%name%"
        - " &a▸ &fCriado em: &a%creation%"
        - " &b▸ &fLíder: &b%leader%"
        - ""
        - "&eOpcões:"
        - " &e▸ &fPúblico: %public%"
        - " &e▸ &fStatus: %visibility%"
        - " &e▸ &fAceita pedidos: %requests%"
        - ""
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    leave:
      name: "&cAbandonar Guilda"
      item: "barrier"
      slot: 8
      lore:
        - ""
        - " &fClique para abandonar"
        - ""
      # Fechará o inventário caso clique
      closeInventory: true

      # Lista de comandos que o jogador executará
      execute: ["/guild leave"]

    delete:
      name: "&cDeletar Guilda"
      item: "barrier"
      slot: 8
      lore:
        - ""
        - " &fDeletar sua Guilda."
        - ""
        - "&eObservações:"
        - " &fPerderá o nome &7%name%"
        - " &fPerderá a tag &f%colortag%"
        - " &fPerderá seus &a%members% membros&f."
        - ""
        - "&c(!) Esta ação é irreversível!"

      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: ["/guild delete"]

    player:
      name: "&aSobre Mim"
      item: "head:player"
      slot: 28
      lore:
        - " "
        - " %player_displayname% %colortag%"
        - ""
        - " &fEntrou em: &a%guild_joined_at%"
        - " &fCargo atual: &a%role_color%%role_name%"
        - ""
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    settings:
      name: "&aGerenciar Guilda"
      item: "comparator"
      slot: 29
      lore:
        - ""
        - " &fEditar configurações"
        - ""
        - "%permission%"
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    level:
      name: "&aNível da Guilda"
      item: "brewing_stand"
      slot: 30
      lore:
        - ""
        - " &6Guilda VIP: &f%premium%"
        - ""
        - "&7Ao ser &6VIP&7, a guilda possui mais vantagens"
        - "&7e mais espaço para membros na guilda"
        - ""

      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    members:
      name: "&aMembros"
      item: "head:b06c31249636361efd15dac1402cb3c8144a1798bd1af7257b95b12b8240399a"
      slot: 31
      lore:
        - ""
        - " &fConferir os membros"
        - ""
        - "&eInformações:"
        - " &a▸ &fPossui: &a%members% membro(s)"
        - " &b▸ &fMáximo: &b%maxmembers% membro(s)"
        - ""
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    invite:
      name: "&aConvidar jogador"
      item: "writable_book"
      slot: 32
      lore:
        - ""
        - " &fConvidar para %colortag%"
        - ""
        - "%permission%"

    discord:
      name: "&aDiscord"
      item: "head:739ee7154979b3f87735a1c8ac087814b7928d0576a2695ba01ed61631942045"
      slot: 34
      lore:
        - ""
        - " &fClique para entrar"
        - " &7discord.gg/&9%discord%"
        - ""
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    invites:
      name: "&aConvites e pedidos"
      item: "head:8d1b28f886ca3c8fc4301b785bf38c619ea66b68352a882bf8080e63034e0"
      slot: 33
      lore:
        - ""
        - " &fConferir &bconvites enviados"
        - " &fConferir &epedidos recebidos"
        - ""
        - "%permission%"
</code-block>
        </chapter>
        <chapter title="guild-invite-menu.yml" collapsible="true">
<code-block lang="yaml">
# Menu de convidar alguém online
main-menu:
  title: "%name% - Convidar"
  slots: 5

list:
# Slots que os itens ocuparão
slots: [ 10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34]

    # Formato dos itens de player
    format:
      name: "%target_displayname%"
      item: "head:%target%"
      invited:
        - ""
        - " &aConvite enviado"
        - ''
      lore:
        - ""
        - " &fO jogador está &a&lONLINE"
        - ''
        - '&eClique para convidar'

# Sinta-se a vontade para por novos itens
# apenas respeite os ids padrões para o funcionamento correto
items:
icon:
name: "%colortag%"
item: "%icon%"
slot: 39
lore:
- ""
- " &fVocê está convidando"
- " &fcom o cargo de %role_color%%role_name%"
- ""
# Fechará o inventário caso clique
closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    return:
      name: "&cVoltar"
      item: "arrow"
      slot: 40
      lore:
        - ""
        - " &fClique para voltar"
        - ""

    invite:
      name: "&aBuscar por Nome"
      item: "writable_book"
      slot: 41
      lore:
        - ""
        - " &fConvidar alguém pelo nome"
        - " &fmesmo não estando online"
        - ""

    previous-page:
      name: "&7Pág. anterior &7(&b%previouspage%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 18
      lore:
        - ""
        - " &7Ir para &fpágina anterior"
        - ""

    next-page:
      name: "&7Próx. página &7(&b%page%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 26
      lore:
        - ""
        - " &7Ir para &fpróxima página"
        - ""
</code-block>
        </chapter>
        <chapter title="guild-member-menu" collapsible="true">
<code-block lang="yaml">
# Menu de convidar alguém online
main-menu:
  title: "%member% - Gerenciar"
  slots: 4

# Sinta-se a vontade para por novos itens
# apenas respeite os ids padrões para o funcionamento correto
items:
return:
name: "&cVoltar"
item: "arrow"
slot: 31
lore:
- ""
- " &fClique para voltar"
- ""

    player:
      name: "%role_prefix% %member%"
      item: "head:%member%"
      slot: 10
      lore:
        - ""
        - "&fMembro da guilda desde:"
        - "&a%joined_at%"
        - ""
        - "&eVocê está gerenciando"

    promote:
      name: "&aPromover"
      item: "emerald"
      slot: 12
      lore:
        - ""
        - "&fPromover membro de cargo"
        - ""
        - "&eEsta ação é reversível"
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute:
        - "/%label% promote %member%"

    demote:
      name: "&cRebaixar"
      item: "redstone"
      slot: 13
      lore:
        - ""
        - "&fRebaixar cargo do membro"
        - ""
        - "&eEsta ação é reversível"

      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute:
        - "/%label% demote %member%"

    transfer:
      name: "&bTransferir posse"
      item: "nether_star"
      slot: 14
      lore:
        - ""
        - "&fConceder sua possa de líder"
        - ""
        - "&cEsta ação é irreversível"
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute:
        - "/%label% transfer %member%"

    kick:
      name: "&4Expulsar"
      item: "barrier"
      slot: 16
      lore:
        - ""
        - "&fExpulsa-lo da guilda"
        - ""
        - "&cEsta ação é irreversível"

      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute:
        - "/%label% kick %member%"
</code-block>
        </chapter>
        <chapter title="guild-members.yml" collapsible="true">
<code-block lang="yaml">
# Menu de convidar alguém online
main-menu:
  title: "%name% - Membros"
  slots: 5

list:
# Slots que os itens ocuparão
slots: [ 10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34]

    # Formato dos itens de player
    format:
      name: "%role_prefix% %member%"
      item: "head:%member%"
      lore:
        - ""
        - " &fMembro da guilda desde:"
        - " &a%joined_at%"
        - ""
        - "%permission%"

# Sinta-se a vontade para por novos itens
# apenas respeite os ids padrões para o funcionamento correto
items:
icon:
name: "%colortag%"
item: "%icon%"
slot: 39
lore:
- ""
- " &fConferindo membros"
- ""
# Fechará o inventário caso clique
closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    return:
      name: "&cVoltar"
      item: "arrow"
      slot: 40
      lore:
        - ""
        - " &fClique para voltar"
        - ""

    filter:
      name: "&aFiltro de Pesquisa"
      item: "nether_star"
      slot: 41
      lore:
        - ""
        - "&fExibir somente:"
        - "%options%"
        - ""
        - "&eClique para alternar"

    previous-page:
      name: "&7Pág. anterior &7(&b%previouspage%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 18
      lore:
        - ""
        - " &7Ir para &fpágina anterior"
        - ""

    next-page:
      name: "&7Próx. página &7(&b%page%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 26
      lore:
        - ""
        - " &7Ir para &fpróxima página"
        - ""
</code-block>
        </chapter>
        <chapter title="guilds-settings.yml" collapsible="true">
<code-block lang="yaml">
# Menu principal
main-menu:
  title: "%name% - Config"
  slots: 4

# Sinta-se a vontade para por novos itens
# apenas respeite os ids padrões para o funcionamento correto
items:
return:
name: "&cVoltar"
item: "arrow"
slot: 31
lore:
- ""
- " &fClique para voltar"
- ""

    icon:
      name: "&aIcone da Guilda"
      item: "%icon%"
      slot: 10
      lore:
        - ""
        - " &8Atual: %icon_name%"
        - " &fAltere o ícone exibido"
        - ""
        - "&e(Visual da Guilda)"

    tag:
      name: "&aTag da Guilda"
      item: "name_tag"
      slot: 11
      lore:
        - ""
        - " &8Atual: %tag%"
        - " &fAltere a tag ao lado do nome"
        - ""
        - "&e(Visual da Guilda)"

    colortag:
      name: "&aCor da Tag da Guilda"
      item: "red_dye"
      slot: 12
      lore:
        - ""
        - " &8Atual: %colortag%"
        - " &fAltere a cor da tag ao lado do nome"
        - ""
        - "&e(Visual da Guilda)"

    visibility:
      name: "&aVisível no Localizador"
      item: "compass"
      slot: 13
      lore:
        - ""
        - " &8Atual: %visibility%"
        - " &fDefina se a Guilda poderá ser"
        - " &fexibida no localizador de Guildas"
        - ""
        - "&e(Ajuda a encontrar novos membros)"

    public:
      name: "&aGuilda Pública"
      item: "sunflower"
      slot: 14
      lore:
        - ""
        - " &8Atual: %public%"
        - " &fDefina se qualquer pessoa poderá entrar"
        - " &fna guilda através do localizador de guildas."
        - ""
        - " &fQualquer membro poderá recrutar outros jogadores."
        - ""
        - "&e(Ajuda a encontrar novos membros)"

    requests:
      name: "&aAceitar pedidos"
      item: "head:8d1b28f886ca3c8fc4301b785bf38c619ea66b68352a882bf8080e63034e0"
      slot: 15
      lore:
        - ""
        - " &8Atual: %requests%"
        - " &fDefina se a Guilda poderá"
        - " &freceber pedidos para entrar"
        - ""
        - "&e(Controle de Membros)"

    description:
      name: "&aDescrição da Guilda"
      item: "writable_book"
      slot: 16
      lore:
        - ""
        - " &8Atual: %description_name%"
        - " &fDefina a descrição que"
        - " &fmelhor defina sua Guilda"
        - ""
        - "&e(Controle de Membros)"

icon-menu:
title: "%name% - Icones"
slots: 54

list:
# Slots que os itens ocuparão
slots: [10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34, 37, 38, 39, 40, 41, 42, 43]

    # Formato dos itens dos ícones
    format:
      name: "%name%"
      item: "%icon%"
      lore:
        - ""
        - " &7Clique para selecionar"
        - ""

# Sinta-se a vontade para por novos itens
# apenas respeite os ids padrões para o funcionamento correto
items:
return:
name: "&cVoltar"
item: "arrow"
slot: 50
lore:
- ""
- " &fClique para voltar"
- ""

    icon:
      name: "%colortag%"
      item: "%icon%"
      slot: 48
      lore:
        - ""
        - " &8Atual: &7%icon_name%"
        - ""
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    previous-page:
      name: "&7Pág. anterior &7(&b%previouspage%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 45
      lore:
        - ""
        - " &7Ir para &fpágina anterior"
        - ""

    next-page:
      name: "&7Próx. página &7(&b%page%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 53
      lore:
        - ""
        - " &7Ir para &fpróxima página"
        - ""

colortag-menu:
title: "%name% - Cores para Tag"
slots: 54

list:
# Slots que os itens ocuparão
slots: [10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34, 37, 38, 39, 40, 41, 42, 43]

    # Formato dos itens dos ícones
    format:
      name: "%name%"
      item: "%icon%"
      lore:
        - ""
        - " %preview%"
        - " &7Clique para selecionar"
        - ""

# Sinta-se a vontade para por novos itens
# apenas respeite os ids padrões para o funcionamento correto
items:
return:
name: "&cVoltar"
item: "arrow"
slot: 50
lore:
- ""
- " &fClique para voltar"
- ""

    icon:
      name: "%colortag%"
      item: "%icon%"
      slot: 48
      lore: []

    previous-page:
      name: "&7Pág. anterior &7(&b%previouspage%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 45
      lore:
        - ""
        - " &7Ir para &fpágina anterior"
        - ""

    next-page:
      name: "&7Próx. página &7(&b%page%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 53
      lore:
        - ""
        - " &7Ir para &fpróxima página"
        - ""

description-menu:
title: "%name% - Descrições"
slots: 54

list:
# Slots que os itens ocuparão
slots: [10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34, 37, 38, 39, 40, 41, 42, 43]

    # Formato dos itens dos ícones
    format:
      name: "%name%"
      item: "%icon%"
      lore:
        - ""
        - "%message%"
        - ""
        - " &7Clique para selecionar"
        - ""

# Sinta-se a vontade para por novos itens
# apenas respeite os ids padrões para o funcionamento correto
items:
return:
name: "&cVoltar"
item: "arrow"
slot: 50
lore:
- ""
- " &fClique para voltar"
- ""

    icon:
      name: "%colortag%"
      item: "%icon%"
      slot: 48
      lore:
        - ""
        - " &8Atual: &f%description_name%"
        - ""

    previous-page:
      name: "&7Pág. anterior &7(&b%previouspage%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 45
      lore:
        - ""
        - " &7Ir para &fpágina anterior"
        - ""

    next-page:
      name: "&7Próx. página &7(&b%page%&7/&b%maxpages%&7)"
      item: "arrow"
      slot: 53
      lore:
        - ""
        - " &7Ir para &fpróxima página"
        - ""
</code-block>
        </chapter>
    </chapter>
    <chapter title="settings/" collapsible="true">
        <chapter title="commands.yml" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração
guild:
  name: guild
  use-command: true
  permission: ''
  aliases:
    - guilda
    - clan
  usage: ''

guildadmin:
name: guildadmin
use-command: true
aliases:
- clanadmin
usage: ''
</code-block>
        </chapter>
    </chapter>
    <chapter title="colors.yml" collapsible="true">
<code-block lang="yaml">
gradient:
  name: "&lt;GRADIENT:#d373ff&gt;Gradiente&lt;/GRADIENT:#5377f5&gt;"
  color: "&lt;GRADIENT:#d373ff&gt;[{tag}]&lt;/GRADIENT:#5377f5&gt;"
  icon: "golden_apple"
  permission:
    only-vip: true
    only-admin: false

preto:
name: "&amp;0Preto"
color: "&amp;0[{tag}]"
icon: "black_dye"

# Permissão necessária

permission:

# Apenas Guildas VIPs podem selecionar

only-vip: false

    # Apenas administradores da equipe podem defini-la em uma guilda
    only-admin: false

vermelho_escuro:
name: "&amp;4Vermelho Escuro"
color: "&amp;4[{tag}]"
icon: "redstone"
permission:
only-vip: false
only-admin: false

vermelho:
name: "&amp;cVermelho"
color: "&amp;c[{tag}]"
icon: "red_dye"
permission:
only-vip: false
only-admin: false

verde_escuro:
name: "&amp;2Verde Escuro"
color: "&amp;2[{tag}]"
icon: "green_dye"
permission:
only-vip: false
only-admin: false

verde:
name: "&amp;aVerde"
color: "&amp;a[{tag}]"
icon: "lime_dye"
permission:
only-vip: false
only-admin: false

azul_escuro:
name: "&amp;1Azul Escuro"
color: "&amp;1[{tag}]"
icon: "blue_dye"
permission:
only-vip: false
only-admin: false

ciano:
name: "&amp;3Ciano"
color: "&amp;3[{tag}]"
icon: "cyan_dye"
permission:
only-vip: false
only-admin: false

azul:
name: "&amp;9Azul"
color: "&amp;9[{tag}]"
icon: "light_blue_dye"
permission:
only-vip: false
only-admin: false

cinza:
name: "&amp;7Cinza"
color: "&amp;7[{tag}]"
icon: "light_gray_dye"

# Permissão necessária

permission:

# Apenas Guildas VIPs podem selecionar

only-vip: false

    # Apenas administradores da equipe podem defini-la em uma guilda
    only-admin: false

cinza_escuro:
name: "&amp;8Cinza Escuro"
color: "&amp;8[{tag}]"
icon: "gray_dye"
permission:
only-vip: false
only-admin: false

amarelo:
name: "&amp;eAmarelo"
color: "&amp;e[{tag}]"
icon: "yellow_dye"
permission:
only-vip: false
only-admin: false

laranja:
name: "&amp;6Laranja"
color: "&amp;6[{tag}]"
icon: "orange_dye"
permission:
only-vip: false
only-admin: false

roxo_escuro:
name: "&amp;5Roxo Escuro"
color: "&amp;5[{tag}]"
icon: "purple_dye"
permission:
only-vip: false
only-admin: false

rosa:
name: "&amp;dRosa"
color: "&amp;d[{tag}]"
icon: "pink_dye"
permission:
only-vip: false
only-admin: false

branco:
name: "&amp;fBranco"
color: "&amp;f[{tag}]"
icon: "white_dye"
permission:
only-vip: false
only-admin: false
</code-block>
    </chapter>
    <chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
# Agradecemos por escolher o LeafGuilds ♥
# Desejamos que tudo ocorra da melhor forma para você,
# e que seus esforços sejam recompensados!

# Seção de configuração do banco de dados individual
database:
# Tipos disponíveis:
# ==> SQLite
# ==> MySQL
type: SQLite

# Caso esteja 'true', não usará o banco de dados global do LeafPlugins (NÃO ATIVE SEM TER CERTEZA)
# Caso não saiba, você pode configurar todos os banco de dados dos plugins Leaf através do LeafPlugins
enable: false

# Configurações para o banco de dados MySQL
mysql:
host: localhost
user: root
password: ''
port: 3306
database: leaf

# Configurações de pool da conexão MYSQL (AVANÇADO)
pool-settings:
enable: true
max-pool-size: 30
min-idle: 10
max-lifetime: 1800000
connection-timeout: 5000

# Ativar/desativar modo de depuração
# Quando ativado, o plugin registrará informações detalhadas de depuração
# Útil para diagnóstico de problemas
debug-mode: false

# Ativar o modo BungeeCord
bungee-mode: false

# Plugins de Economia que serão utilizados
# https://docs.leafplugins.com/tutorials/economies
economies:
# Plugin para Money
money: Vault

# Plugin para Cash
cash: PlayerPoints

# Opções gerais de Guilda
guilds:
# Formato do chat
chat-format: '&c[Chat da Guilda] %role_prefix% &f%player% %role_color%» &f%message%'

# Atalhos para enviar mensagem para Guilda
# Exemplos:
# => /. <mensagem>
# => /gc <mensagem>
chat-shortcuts:
- /.
- /c
- /gc

# Enviar os titulos de anúncio da Guilda
# Exemplo: Alterações de cargo, expulsão.
announce-title: true

# Tempo para os convites expirarem desde seu envio
invite-expire: 7d

# Dias necessário para que o membro possa ser
# apto a ser líder através da transferência de posse
# Deixe 0 para desativar
transfer-required-days: 7

# Anúncios para todos do servidor atual
broadcasts:
# Anunciar quando uma guilda for criada
guild-created:
enable: true

      # Som que será tocado, deixe em branco ("") para desativar
      sound: ENDER_DRAGON_GROWL
    
    # Anunciar quando uma guilda for excluída
    guild-deleted:
      enable: true
      
      # Som que será tocado, deixe em branco ("") para desativar
      sound: ENDER_DRAGON_GROWL

# Máximo de membros em uma guilda (Incluindo todos)
max-members:
# Guildas comuns
default: 8

    # Guildas Premiums
    premium: 0

# Não remova/crie os cargos, apenas modifique-os
roles:
leader:
name: Lider
color: '&b'
prefix: '&b[Líder]'
moderator:
name: Moderador
color: '&a'
prefix: '&a[Moderador]'
recruiter:
name: Recrutador
color: '&6'
prefix: '&6[Recrutador]'
member:
name: Membro
color: '&7'
prefix: '&7[Membro]'

# Melhoria da Guilda para VIP
upgrade:
# Permissão necessária (Deixe "" para não exigir)
permission: ''

    # Preço para a melhoria (Deixe zero em ambos para não exigir)
    economy:
      # Caso esteja 'true' fará que exija os dois ao mesmo tempo
      requires-both: false
      
      # Se Money estiver zero, só será possível pagar com Cash
      money-price: 100000
      
      # Se Cash estiver zero, só será possível pagar com money
      cash-price: 10000
      
      # Permissão para não exigir pagamento (Deixe "" para desativar)
      bypass-permission: leafguilds.upgrade.pricebypass

# Criação da Guilda
create:
# Permissão necessária (Deixe "" para não exigir)
permission: ''

    # Preço para a criação (Deixe zero em ambos para não exigir)
    economy:
      # Caso esteja 'true' fará que exija os dois ao mesmo tempo
      requires-both: false
      
      # Se Money estiver zereo, só será possível pagar com Cash
      money-price: 100000
      
      # Se Cash estiver zero, só será possível pagar com money
      cash-price: 10000
      
      # Permissão para não exigir pagamento (Deixe "" para desativar)
      bypass-permission: leafguilds.create.pricebypass
    
    # Opções por padrão após a criação
    default:
      # Icone padrão (icons.yml)
      icon: banner
      
      # Cor da tag padrão (colors.yml)
      color-tag: cinza
      
      # Descrição padrão (descriptions.yml)
      description: default
      
      # Deixe 'true' caso queira que seja público por padrão
      public: false
    
    options:
      name:
        # Tamanho máximo
        max-length: 16
        
        # Tamanho minimo
        min-length: 3
        
        # Permitir caracteres especiais
        allow-special-char: true
        
        # Permitir espaçamento
        allow-space: true
        
        # Fará que sempre seja em caixa alta (Tudo maiúsculo)
        always-uppercase: false
        
        # Os nomes das Guildas não irão poder conter estas palavras
        blocked-names:
          - admin
          - admins
          - helper
          - staff
          - staffer
          - server
      
      tag:
        # Tamanho máximo (Não recomendado que aumente em servidores de versão inferior a 1.12)
        max-length: 8
        
        # Tamanho minimo
        min-length: 3
        
        # Fará que sempre seja em caixa alta (Tudo maiúsculo)
        always-uppercase: true
        
        # Permitir caracteres especiais
        allow-special-char: false
        
        # Permitir espaçamento (Não recomendado para servidores de versão inferior a 1.12)
        allow-space: false
        
        # As tags das Guildas não irão poder conter estas palavras
        blocked-tags:
          - admin
          - admins
          - helper
          - staff
          - staffer
          - server
</code-block>
    </chapter>
    <chapter title="descriptions.yml" collapsible="true">
<code-block lang="yaml">
default:
  # Nome da descrição
  name: "&cNenhuma"

# Icone da descrição
icon: "sign"

# Mensagem da descrição
message:
- "&cNenhuma descrição"

# Permissão necessária
permission:
# Apenas Guildas VIPs podem selecionar
only-vip: false

    # Apenas administradores da equipe podem defini-la em uma guilda
    only-admin: false

sopa:
name: "&aSopeiros!"
icon: "mushroom_stew"
message:
- "&7Focados em PvP com Sopa"
permission:
only-vip: false
only-admin: false

foguete:
name: "&aOs Foguetes!"
icon: "firework_rocket"
message:
- "&7Somos imparáveis!"
permission:
only-vip: false
only-admin: false
</code-block>
    </chapter>
    <chapter title="icons.yml" collapsible="true">
<code-block lang="yaml">
# Icones disponiveis
banner:
  # Nome de exibição
  name: "&7Banner Preto"

# Item
item: "black_banner"

# Permissão necessária
permission:
# Apenas Guildas VIPs podem selecionar
only-vip: false

    # Apenas administradores da equipe podem defini-la em uma guilda
    only-admin: false

red_banner:
name: "&cBanner Vermelho"
item: "red_banner"
permission:
only-vip: false
only-admin: false

green_banner:
name: "&2Banner Verde"
item: "green_banner"
permission:
only-vip: false
only-admin: false

brown_banner:
name: "&6Banner Marrom"
item: "brown_banner"
permission:
only-vip: false
only-admin: false

blue_banner:
name: "&9Banner Azul"
item: "blue_banner"
permission:
only-vip: false
only-admin: false

purple_banner:
name: "&5Banner Roxo"
item: "purple_banner"
permission:
only-vip: false
only-admin: false

cyan_banner:
name: "&3Banner Ciano"
item: "cyan_banner"
permission:
only-vip: false
only-admin: false

light_gray_banner:
name: "&7Banner Cinza Claro"
item: "light_gray_banner"
permission:
only-vip: false
only-admin: false

gray_banner:
name: "&8Banner Cinza"
item: "gray_banner"
permission:
only-vip: false
only-admin: false

pink_banner:
name: "&dBanner Rosa"
item: "pink_banner"
permission:
only-vip: false
only-admin: false

lime_banner:
name: "&aBanner Verde Limão"
item: "lime_banner"
permission:
only-vip: false
only-admin: false

yellow_banner:
name: "&eBanner Amarelo"
item: "yellow_banner"
permission:
only-vip: false
only-admin: false

light_blue_banner:
name: "&bBanner Azul Claro"
item: "light_blue_banner"
permission:
only-vip: false
only-admin: false

magenta_banner:
name: "&dBanner Magenta"
item: "magenta_banner"
permission:
only-vip: false
only-admin: false

orange_banner:
name: "&6Banner Laranja"
item: "orange_banner"
permission:
only-vip: false
only-admin: false

white_banner:
name: "&fBanner Branco"
item: "white_banner"
permission:
only-vip: false
only-admin: false
</code-block>
    </chapter>
    <chapter title="placeholders.yml" collapsible="true">
<code-block lang="yaml">
# Configuração das placeholders pro jogador
# Você pode criar, remover e editar
# Formato: %leafguilds_&lt;placeholder&gt;%
# Exemplo: %leafguilds_customtag%
customname:
  noClan: "&amp;cSem Clan"
  result: "%guild_name%"
customtag:
  noClan: "&amp;cSem Clan"
  result: "&amp;8[%guild_colortag%&amp;8]"
abovename:
  noClan: ""
  result: "&amp;8(%guild_colortag%&amp;8) &amp;f- %role_color%%role_name%"
</code-block>
    </chapter>
</chapter>