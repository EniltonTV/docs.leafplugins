# arquivos-tags

<chapter id="arquivos-tags" title="Arquivos" collapsible="true">
<chapter title="Lang/" collapsible="true">
<chapter title="messages_en.yml" collapsible="true">
<code-block lang="YAML">
# Tag list message
tag-list: '&aYour tags: &f%tags%'

# Visual of tags in the list
tag-list-visual: '%tag_preset%'

# Visual of what will separate the tags in the list
tag-list-separe: '&f, '

# Preview visual when hovering the mouse over the tag
tag-list-preview:
- '%tag_preview%'
- ''
- '&eClick to select'

tag-set: '&aYour tag has been changed to %tag_name%.'
tag-give: '&aTag %tag_name% given to %player%.'
tag-remove: '&aTag %tag_name% removed from %player%.'
tag-target-set: '&a%player% tag changed to %tag_name%.'
tag-already-set: '&cYou are already using %tag_name%.'
tag-no-permission: '&cThis tag was not found or you do not have it.'
tag-not-found: '&cThis tag was not found or you do not have it.'
tag-blocked-world: '&cTag switching is not allowed in this world.'
command-set-usage: <player> <tag> %usage%

suffixes:
# Suffix list message
suffix-list: '&aYour suffixes: &f%suffixes%'

# Visual of suffixes in the list
suffix-list-visual: '%suffix_preset%'

# Visual of what will separate the suffixes in the list
suffix-list-separe: '&f, '

# Visual preview when hovering the mouse over the suffix
suffix-list-preview:
- '%suffix_preview%'
- ''
- '&eClick to select'

suffix-set: '&aYour suffix has been changed to %suffix_name%.'
suffix-already-set: '&cYou already have the suffix %suffix_name%.'
suffix-no-permission: '&cThis suffix was not found or you do not have permission to use it.'
suffix-not-found: '&cThis suffix was not found or you do not have permission to use it.'

</code-block>
</chapter>
<chapter title="messages_es.yml" collapsible="true">
<code-block lang="yaml">
# Mensaje de la lista de etiquetas
tag-list: '&aTus tags: &f%tags%'

# Visual de las etiquetas en la lista
tag-list-visual: '%tag_preset%'

# Visual de lo que separará las etiquetas en la lista
tag-list-separe: '&f, '

# Visual previo al pasar el mouse sobre la etiqueta
tag-list-preview:
- '%tag_preview%'
- ''
- '&eHaz clic para seleccionar'

tag-set: '&aTu tag ha sido cambiada a %tag_name%.'
tag-give: '&aTag %tag_name% otorgada a %player%.'
tag-remove: '&aTag %tag_name% eliminada de %player%.'
tag-target-set: '&aTag de %player% cambiada a %tag_name%.'
tag-already-set: '&cYa tienes la tag %tag_name%.'
tag-no-permission: '&cEsta tag no se encontró o no la tienes.'
tag-not-found: '&cEsta tag no se encontró o no la tienes.'
tag-blocked-world: '&cNo se permite cambiar de tag en este mundo.'
command-set-usage: <jugador> <tag> %usage%

suffixes:
# Mensaje de la lista de sufijos
suffix-list: '&aTus sufijos: &f%suffixes%'

# Visual de los sufijos en la lista
suffix-list-visual: '%suffix_preset%'

# Visual de lo que separará los sufijos en la lista
suffix-list-separe: '&f, '

# Visual previo al pasar el mouse sobre el sufijo
suffix-list-preview:
- '%suffix_preview%'
- ''
- '&eHaz clic para seleccionar'

suffix-set: '&aTu sufijo ha sido cambiado a %suffix_name%.'
suffix-already-set: '&cYa tienes el sufijo %suffix_name%.'
suffix-no-permission: '&cEste sufijo no se encontró o no lo tienes.'
suffix-not-found: '&cEste sufijo no se encontró o no lo tienes.'
suffix-blocked: '&cNo se permite el uso de sufijos en tu tag actual.'
</code-block>
</chapter>
<chapter title="messages.pt.yml" collapsible="true">
<code-block lang="yaml">
# Mensagem da lista de tags
tag-list: '&aSuas tags: &f%tags%'

# Visual das tags na lista
tag-list-visual: '%tag_preset%'

# Visual do que separará as tags na lista
tag-list-separe: '&f, '

# Visual do preview ao passar o mouse em cima da tag
tag-list-preview:
- '%tag_preview%'
- ''
- '&eClique para selecionar'

tag-set: '&aSua tag foi alterada para %tag_name%.'
tag-give: '&aTag %tag_name% concedida a %player%.'
tag-remove: '&aTag %tag_name% removida de %player%.'
tag-target-set: '&aTag de %player% alterada para %tag_name%.'
tag-already-set: '&cVocê já está com a tag %tag_name%.'
tag-no-permission: '&cEsta tag não foi encontrada ou você não a possui.'
tag-not-found: '&cEsta tag não foi encontrada ou você não a possui.'
tag-blocked-world: '&cNão é permitido a troca de tag neste mundo.'
command-set-usage: <jogador> <tag> %usage%

suffixes:
# Mensagem da lista de suffix
suffix-list: '&aSeus sufixos: &f%suffixes%'

# Visual das suffixes na lista
suffix-list-visual: '%suffix_preset%'

# Visual do que separará as suffixes na lista
suffix-list-separe: '&f, '

# Visual do preview ao passar o mouse em cima da suffix
suffix-list-preview:
- '%suffix_preview%'
- ''
- '&eClique para selecionar'

suffix-set: '&aSeu sufixo foi alterado para %suffix_name%.'
suffix-already-set: '&cVocê já está com o sufixo %suffix_name%.'
suffix-no-permission: '&cEste sufixo não foi encontrado ou você não o possui.'
suffix-not-found: '&cEste sufixo não foi encontrado ou você não o possui.'
suffix-blocked: '&cNão é permitido o uso de sufixos na sua atual tag.'
</code-block>
</chapter>
</chapter>
<chapter title="menus/" collapsible="true">
<chapter title="suffixes-menu.yml" collapsible="true">
<code-block lang="yaml">
main-menu:
  title: "Seus Sufixos"
  slots: 54

# Fechará o menu ao selecionar
closeInventory: true

list:
# Slots que os itens ocuparão
slots: [10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34, 37, 38, 39, 40, 41, 42, 43]

    # Formato dos itens dos sufixos
    format:
      name: "%preset%"
      item: "%icon%"
      lore:
        - ""
        - " &fPreview: &7%preview%"
        - ""
        - "&eClique para selecionar"

items:
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
<chapter title="tags-menu.yml" collapsible="true">
<code-block lang="yaml">
main-menu:
  title: "Suas Tags"
  slots: 54

# Fechará o menu ao selecionar
closeInventory: true

list:
# Slots que os itens ocuparão
slots: [10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34, 37, 38, 39, 40, 41, 42, 43]

    # Formato dos itens das tags
    format:
      name: "%color%%name%"
      item: "%icon%"
      lore:
        - ""
        - " &fPreview: &7%preview%"
        - ""
        - "&eClique para selecionar"

# Altere como quiser
items:
# Vidros de decoração
glass_1:
name: "&5"
item: "stained_glass_pane:15"
slot: 0
lore: []

    glass_2:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 1
      lore: []

    glass_3:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 2
      lore: []

    glass_4:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 3
      lore: []

    glass_5:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 4
      lore: []

    glass_6:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 5
      lore: []

    glass_7:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 6
      lore: []

    glass_8:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 7
      lore: []

    glass_9:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 8
      lore: []

    # Preenchendo verticalmente (coluna 1 e 2)
    glass_10:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 9
      lore: []

    glass_11:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 17
      lore: []

    glass_12:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 18
      lore: []

    glass_13:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 26
      lore: []

    glass_14:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 27
      lore: []

    glass_15:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 35
      lore: []

    glass_16:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 36
      lore: []

    glass_17:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 44
      lore: []

    # Preenchendo mais verticalmente (coluna 1 e 2)
    glass_18:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 45
      lore: []

    glass_19:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 46
      lore: []

    glass_20:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 47
      lore: []

    glass_21:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 48
      lore: []

    glass_22:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 49
      lore: []

    glass_23:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 50
      lore: []

    glass_24:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 51
      lore: []

    glass_25:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 52
      lore: []

    glass_26:
      name: "&5"
      item: "stained_glass_pane:15"
      slot: 53
      lore: []

    player:
      name: "&a%player%"
      item: "head:player"
      slot: 49
      lore:
        - "&7Usando: %leaftags_tag_color%%leaftags_tag_name%"
        - ""
        - "&eClique para fechar"

      closeInventory: true

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
<chapter title="prefixes/" collapsible="true">
<chapter title="default.yml" collapsible="true">
<code-block lang="yaml">
Dono:
  visual:
    name: "Dono"
    color: "&4"
    prefix: "&4[Dono] "
    suffix: ""
    preset: "&4Dono"
    aboveName: "&6[EQUIPE]"
    tablistPrefix: "&4[Dono] "
    tablistSuffix: ""
  options:
    icon: "head:252559f2bcead983f4b6561c2b5f2b588f0d6116d44666ceff1202079d27ca74"
    position: 1
    visible: true
    customSuffix: false
    description:
      - "&7Tag destinada aos &4Donos&7."
    permission: "leaftags.tag.dono"
    aliases: ["subdono", "master", "owner"]

Admin:
visual:
name: "Admin"
color: "&c"
prefix: "&c[Admin] "
suffix: ""
preset: "&cAdmin"
aboveName: "&6[EQUIPE]"
tablistPrefix: "&c[Admin] "
tablistSuffix: ""
options:
icon: "diamond_axe"
position: 2
visible: true
customSuffix: false
description:
- "&7Tag destinada aos &cAdministradores&7."
  permission: "leaftags.tag.admin"
  aliases: ["adm"]

Moderador:
visual:
name: "Moderador"
color: "&a"
prefix: "&a[Moderador] "
suffix: ""
preset: "&aModerador"
aboveName: "&6[EQUIPE]"
tablistPrefix: "&a[Moderador] "
tablistSuffix: ""
options:
icon: "diamond_pickaxe"
position: 3
visible: true
customSuffix: false
description:
- "&7Tag destinada aos &aModeradores&7."
  permission: "leaftags.tag.mod"
  aliases: ["mod", "moderator"]

Ajudante:
visual:
name: "Ajudante"
color: "&b"
prefix: "&b[Ajudante] "
suffix: ""
preset: "&bAjudante"
aboveName: "&6[EQUIPE]"
tablistPrefix: "&b[Ajudante] "
tablistSuffix: ""
options:
icon: "paper"
position: 4
visible: true
customSuffix: false
description:
- "&7Tag destinada aos &bAjudantes&7."
  permission: "leaftags.tag.ajudante"
  aliases: ["helper", "ajuda"]

YoutuberPlus:
visual:
name: "YouTuber+"
color: "&3"
prefix: "&3[YT+] "
suffix: ""
preset: "&3YouTuber+"
aboveName: "&6[Influenciador]"
tablistPrefix: "&3[Youtuber+] "
tablistSuffix: ""
options:
icon: "head:c0c9a3a4ffbee61d1ee1c3a533355bda9cdc377e07b0ff8bc618d3977b7f86cc"
position: 5
visible: true
customSuffix: false
description:
- "&7Tag destinada aos &3Youtubers&f+&7."
  permission: "leaftags.tag.ytPlus"
  aliases: ["yt+", "ytplus"]

Youtuber:
visual:
name: "YouTuber"
color: "&b"
prefix: "&b[YT] "
suffix: ""
preset: "&bYouTuber"
aboveName: "&6[Influenciador]"
tablistPrefix: "&b[Youtuber] "
tablistSuffix: ""
options:
icon: "head:c767ed79ede7b581de4c6c731f5b8598924cf456e5a4040e27fdf25ac602531d"
position: 6
visible: true
customSuffix: false
description:
- "&7Tag destinada aos &bYoutubers&7."
  permission: "leaftags.tag.yt"
  aliases: ["yt"]

MVP:
visual:
name: "MvP+"
color: "&b"
prefix: "&b[MVP&6+&b] "
suffix: ""
preset: "&bMvP&6+"
aboveName: "&6[VIP]"
tablistPrefix: "&b[MVP&6+&b] "
tablistSuffix: ""
options:
icon: "nether_star"
position: 7
visible: true
customSuffix: false
description:
- "&7Tag destinada aos &bMVPs&6+&7."
  permission: "leaftags.tag.mvpPlus"
  aliases: ["mvp+", "mvpplus", "vip2", "vipplus", "plus"]

VIP:
visual:
name: "Vip"
color: "&a"
prefix: "&a[VIP] "
suffix: ""
preset: "&aVip"
aboveName: "&6[VIP]"
tablistPrefix: "&a[VIP] "
tablistSuffix: ""
options:
icon: "gold_ingot"
position: 8
visible: true
customSuffix: false
description:
- "&7Tag destinada aos &aVIPs&7."
  permission: "leaftags.tag.vip"
  aliases: []

Membro:
visual:
# Nome da nametag
name: "Membro"

    # Cor da nametag
    color: "&7"

    # Prefixo da nametag (Antes do nome)
    prefix: "&7"

    # Suffix da nametag (Depois do nome)
    suffix: ""

    # Preset da nametag (Geralmente utilizado em menus, mensagens e scoreboards)
    preset: "&7Membro"

    # [Premium] Texto em cima do nome
    aboveName: ""

    # Prefix da nametag na TabList (Caso deixe vazio irá utilizar o prefix/suffix padrão da tag)
    tablistPrefix: "&7[Membro] "
    tablistSuffix: ""

options:
# Icone que aparecerá no menu
icon: "name_tag"

    # Posição do jogador na TabList
    position: 26

    # Caso esteja 'false', fará que o nickname
    # do jogador não apareça em cima do jogador
    visible: true

    # Permitirá que os jogadores usem outros sufixos
    # Caso esteja 'false', fará que use o suffix da tag
    customSuffix: false

    # Descrição da tag
    description:
      - "&7Tag destinada aos &fjogadores&7."

    # Permissão da nametag (Deixe vazio para que não seja necessário)
    permission: ""

    # Variáveis de como utilizar a tag - /tag <variavel>
    aliases: ["player", "padrão", "default", "padrao", "jogador"]
</code-block>
</chapter>
</chapter>
<chapter title="settings/" collapsible="true">
<chapter title="commands.yml" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração

tag:
name: tag
use-command: true
permission: ''
aliases:
- tags
- prefix
- prefixes
- prefixos

suffix:
name: suffix
use-command: true
permission: ''
aliases:
- suffixes
- customsuffix
- sufixo
- sufixos

settag:
name: settag
use-command: true
permission: leaftags.command.settag
aliases:
- tagset
- setprefix
  usage: para alterar o prefixo de alguém.
# Caso queira fazer que o console execute algum comando, utilize:
# execute:
# - pex user %player% group set %tag_id%
execute:
- lp user %player% parent set %tag_id%

givetag:
name: givetag
use-command: true
permission: leaftags.command.givetag
aliases:
- dartag
- darprefix
  usage: para dar um prefixo a alguém.
  execute:
- lp user %player% permission set %tag_permission%
  #- pex user %player% add %tag_permission%

removetag:
name: removetag
use-command: true
permission: leaftags.command.removetag
aliases:
- removertag
- removerprefix
  usage: para retirar um prefixo de alguém.
  execute:
- lp user %player% permission unset %tag_permission%
  #- pex user %player% remove %tag_permission%
</code-block>
</chapter>
</chapter>
<chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
# Agradecemos por escolher o LeafTags ♥
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

# Arquivo que será usado para os prefixos
tags-file: default.yml

# Opções de bloqueio
block-options:
# Removerá a tag da tablist nos mundos bloqueados
disable-tablist: true

# Removerá a nametag nos mundos bloqueados
disable-nametag: false

# Removerá a displayName nos mundos bloqueados
disable-display-name: false

# Removerá o aboveName nos mundos bloqueados
disable-above-name: true

# Não permitirá a mudança de tag em mundos bloqueados
block-change-tag: true

# Caso esteja 'true', fará que apenas os mundos da lista "worlds"
# tenha nametags/tag (Invertendo de blocked para whitelist)
white-list: false

# Mundos que terão a tag bloqueada
# Caso o white-list esteja 'true',
# fará que somente estes mundos tenham nametag/tag
worlds:
- blockedWorld

# Desative 'nickname, display-name' caso prefira usar outro plugin de NameTag (ex: NametagEdit)
# Desativando a função de NameTag, você poderá usa-lo como plugins de tags especiais e afins ;)
nametag:
# O prefix e o suffix serão aplicados em seu nickname (Em cima do jogador)
# (Caso não tenha um plugin de tab, também aparecerá no tab)
nickname: true

# O prefix será aplicado no displayName
# (Serve para placeholders como %player_displayname%)
display-name: true

# Fará que ignore o limite de tamanho do prefix no nickname
# (Ativa-lo pode causar bugs em seu servidor caso use como NameTag, a menos que use o high-limit true)
ignore-size: false

# [Premium]
# Nosso sistema que permite limites ainda maiores para nametags e mais
hologram:
# Substituir o nome em cima do jogador pelo nosso sistema
# que permite tags ainda maiores mesmo em versões 1.8+
# (Automaticamente ativará o ignore-size internamente)
high-limit: true

# Formato do nome do jogador (SUPORTA PLACEHOLDERAPI)
# Valores padrões:
# ==> {prefix}: Prefixo
# ==> {suffix}: Sufixo
# ==> {player}: Nome do jogador
nick-format: '{prefix}{player}{suffix}'

# Alturas dos hologramas
heights:
# Altura do nome do jogador
nickname: -0.3

    # Altura dos textos em cima do nome
    abovename: 0.1

# Visibilidade dos hologramas
visibility:
# Caso esteja 'true', o jogador poderá ver seu próprio nickname
# (Somente com tags animadas ou high-limit)
# [RECOMENDADO SOMENTE PARA TESTES]
self-nickname: false

    # Caso esteja 'true', o jogador poderá ver o próprio texto em cima do nome
    # [RECOMENDADO SOMENTE PARA TESTES]
    self-abovename: false
    
    # Caso esteja 'true', sempre exibirá os hologramas para TODOS mesmo se o jogador estiver AGACHADO
    always-visible: false

# [Premium]
# Compatibilidade com plugins de fakes e nomes customizados
# Mudará o nome do jogador no displayName, tablist e holograma.
custom-name:
enable: false

# Placeholder que retornará o nome fake ou customizado do jogador
placeholder: '%plugin_name%'

options:
# Sempre que o jogador entrar no servidor, entrará com a última tag usada
# (Recomendado para servidores BungeeCord)
# Observação: Caso seu servidor seja BungeeCord,
# só funcionará caso a tag exista em todos os servidores
last-tag: true

# Sempre que o jogador entrar no servidor, entrará com o último sufixo customizado usado
# (Recomendado para servidores BungeeCord)
# Observação: Caso seu servidor seja BungeeCord,
# só funcionará caso o sufixo exista em todos os servidores
last-suffix: true

# Fará que sempre que o jogador altere sua tag, atualize instantaneamente no banco de dados
database-update: true

# Organizar as tags pela "position" definida
# Isso influenciará na checagem da maior tag do jogador e organização do /tag
# Deixe 'false' caso queira manter como antigamente
organize-by-position: true

# Formato do nome do jogador no Tablist (SUPORTA PLACEHOLDERAPI)
# Valores padrões:
# ==> {prefix}: Prefixo
# ==> {suffix}: Sufixo
# ==> {player}: Nome do jogador
tab-format: '{prefix}{player}{suffix}'

# Sempre que o jogador alterar sua tag manualmente,
# será enviada uma log ao console
log-console: true

# Mensagem que será enviada na log (Suporta cores)
log-console-message: '&9[Tag] &rO jogador &a%player% &ralterou sua tag para %tag_name%'

updates:
# Atualizar a tag do jogador quando mudar de mundo
on-world-change: true

# Atualizar a tag do jogador quando ter seu cargo alterado
on-group-change: true

# Qualquer ação detectada sobre o clan irá atualizar a tag
# (Ajuda a manter o suffix atualizado)
# Exemplos: Sair, entrar, atualização do clan
on-clan-update: true

# Segundos para atualizar a tag automaticamente
# (Deixe 0 para desativar) [Ajuda a manter o suffix atualizado]
seconds-to-update: 8

# O jogador sempre terá sua tag alterada para a máxima
# quando houver alguma tag update
always-max-tag: false

command:
# Tempo em segundos para poder alterar a tag novamente
# (Deixe 0 para desativar)
cooldown: 1

# Permissão para não ter cooldown
# (Deixe vazio para desativar)
cooldown-permission: leaftags.cooldown

# Fará que caso o jogador tenha sua tag alterada por outra pessoa
# ela receba a mensagem 'tag-set'
target-set-message: true

# Fará que as tags sejam selecionadas através do menu
select-menu: false

# Fará que os sufixos sejam selecionadas através do menu
select-menu-suffix: false

# Fará que as tags possam ser selecionadas clicando
# (Funcionará apenas com 'select-menu' estando 'false')
json-click: true

# Fará que apareça de forma crescente conforme a configuração
reverse-list: true

# Enviará um titulo quando a tag for alterada
title:
enable: true
title: '%tag_preset%'
subtitle: Tag selecionada

# Som que irá tocar quando mudar de tag
# (Deixe vazio para desativar)
sound: CHICKEN_EGG_POP

</code-block>
</chapter>
<chapter title="suffixes.yml" collapsible="true">
<code-block lang="yaml">
leaf:
  name: 'Leaf'
  icon: 'head:97bb4da93df2de92ba639ba33437c14911c29be2ea57fbf305b80effaecc4bfc'
  preset: '&5Leaf'
  suffix: ' &8[&5Leaf&8]'
  permission: ''

heart:
name: 'Coração'
icon: 'head:1d0f2925df37fbd5f80829cafb3e9e9ac00f75a991b2131c26e0b2198e300018'
preset: '&dCoração'
suffix: ' &d&l❤'
permission: ''

medal:
name: 'Medalha'
icon: 'head:33178d01aaf11e5ccfa38b190d7085ff37dd048d09b664f02570776f9b981466'
preset: '&eMedalha'
suffix: ' %leafmedals_medals%'
permission: ''

clan:
name: 'Meu clan'
icon: 'head:a8832c1466c841cc79d5f10295d464279967975a2451c7a533c7996897408bea'
preset: '&bMeu clan'
suffix: '<whennot="">%simpleclans_clan_color_tag%</whennot=" &8[%simpleclans_clan_color_tag%&8]">'
permission: ''

# Não remova
none:
# Nome do suffix
name: 'Nenhum'

# Icone
icon: 'name_tag'

# Preset do suffix
preset: '&fNenhum'

# Como será exibido
suffix: ''

# Permissão do suffix
permission: ''
</code-block>
</chapter>
</chapter>