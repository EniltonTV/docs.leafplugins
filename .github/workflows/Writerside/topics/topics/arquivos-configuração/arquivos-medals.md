# arquivos-medals

<chapter id="arquivos-medals" title="Arquivos" collapsible="true">
<chapter title="lang/" collapsible="true">
<chapter title="messages_en.yml" collapsible="true">
<code-block lang="YAML">
# Medal list message
medal-list: '&aYour medals: &f%medals%'

# Visual representation of the medals in the list
medal-list-visual: '%medal_preset%'

# Visual that separates the medals in the list
medal-list-separe: '&f, '

# Visual of the preview when hovering over the medal
medal-list-preview:
- '%medal_color%%medal_name% %medal_icon%'
- ''
- '&eClick to select'

medal-set: '&aYour medal has been changed to %medal_name%&a.'
medal-already-set: '&cYou already have the %medal_name% medal&c.'
medal-target-set: '&aSlot #%slot% set with %medal_name% for %player%.'
medal-target-set-failed-1: '&cThe player does not have permission for the slot.'
medal-target-set-failed-2: '&cThe player does not have the medal.'
medal-no-permission: '&cThis medal was not found or you do not have it.'
medal-not-found: '&cThis medal was not found or you do not have it.'
command-set-usage: <player> <slot> <medal> %usage%
</code-block>
</chapter>
<chapter title="messages.pt.yml" collapsible="true">
<code-block lang="yaml">
# Mensagem da lista de medalhas
medal-list: '&aSuas medalhas: &f%medals%'

# Visual das medalhas na lista
medal-list-visual: '%medal_preset%'

# Visual do que separará as medalhas na lista
medal-list-separe: '&f, '

# Visual do preview ao passar o mouse em cima da medalha
medal-list-preview:
- '%medal_color%%medal_name% %medal_icon%'
- ''
- '&eClique para selecionar'

medal-set: '&aSua medalha foi alterada para %medal_name%&a.'
medal-already-set: '&cVocê já está com a medalha %medal_name%&c.'
medal-target-set: '&aSlot #%slot% definido com %medal_name% para %player%.'
medal-target-set-failed-1: '&cO jogador não possui permissão para o slot.'
medal-target-set-failed-2: '&cO jogador não possui a medalha.'
medal-no-permission: '&cEsta medalha não foi encontrada ou você não a possui.'
medal-not-found: '&cEsta medalha não foi encontrada ou você não a possui.'
command-set-usage: <jogador> <slot> <medalha> %usage%
</code-block>
</chapter>
</chapter>
<chapter title="medals/" collapsible="true">
<chapter title="medals.yml" collapsible="true">
<code-block lang="yaml">
Cafe:
  visual:
    name: "Café"
    color: "&e"
    icon: "&e☕"
    prefix: "&e☕ "
    suffix: " &e☕"
    preset: "&e☕"
  options:
    permission: "leafmedals.medal.cafe"
    itemId: head:f2b89f5487548bf67f9ba2bcbb3a791733184586b3208f6d37f2e3548feaf7e4
    rarity: "&9Raro"
    description:
      - "Quem não ama um café?"

Flash:
visual:
name: "Flash"
color: "&6"
icon: "&6⚡"
prefix: "&6⚡ "
suffix: " &6⚡"
preset: "&6⚡"
options:
permission: "leafmedals.medal.flash"
itemId: head:313f8768b3f5b614d7589fb273c6d3b9b0208310a025bb99a271c73c4b36eb70
rarity: "&9Raro"
description:
- "&7Exclusivo do &6Passe de"
- "&6Batalha &7da &aTemporada 1"

Musico:
visual:
name: "Músico"
color: "&6"
icon: "&5♬"
prefix: "&5♬ "
suffix: " &5♬"
preset: "&5♬"
options:
permission: "leafmedals.medal.musico"
itemId: name_tag
rarity: "&9Raro"
description:
- "&7Exclusivo do &6Passe de"
- "&6Batalha &7da &aTemporada 1"

YinYang:
visual:
name: "YinYang"
color: "&f"
icon: "&f☯"
prefix: "&f☯ "
suffix: " &f☯"
preset: "&f☯"
options:
permission: "leafmedals.medal.yinyang"
itemId: name_tag
rarity: "&fComum"
description:
- "&7Exclusivo do &6Passe de"
- "&6Batalha &7da &aTemporada 1"

Toxico:
visual:
name: "Tóxico"
color: "&a"
icon: "&a☣"
prefix: "&a☣ "
suffix: " &a☣"
preset: "&a☣"
options:
permission: "leafmedals.medal.toxico"
itemId: name_tag
rarity: "&fComum"
description:
- "&7Exclusivo do &6Passe de"
- "&6Batalha &7da &aTemporada 1"

None:
visual:
name: "Nenhuma"
color: ""
icon: ""
prefix: ""
suffix: ""
preset: "&7Nenhuma"
options:
permission: ""
itemId: name_tag
rarity: "&fComum"
description: []
</code-block>
</chapter>
</chapter>
<chapter title="menus/" collapsible="true">
<chapter title="medals-menu.yml" collapsible="true">
<code-block lang="yaml">
main-menu:
  title: "Suas medalhas"
  slots: 5
  items:
    # Você pode remover os itens, como também pode por mais
    # caso queira por mais um slot de medalha no menu, é só seguir o mesmo padrão
    # medal1, medal2, medal3, medal4, medal5...
    medal1:
      name: '%color%&amp;l➜ %color%&lt;when="empty"&gt;%medal_name%&lt;/when="Slot de Medalha #1"&gt;'
      item: '&lt;when="empty"&gt;%medal_item%&lt;/when="RED_STAINED_GLASS_PANE"&gt;'
      slot: 20
      permission:
        - "&amp;7Você não tem permissão"
        - "&amp;7para usar este slot."
        - ""
        - "&amp;cSem permissão"
      selected:
        - "&amp;7Medalha com o"
        - "&amp;7símbolo %medal_icon%"
        - ""
        - "&amp;eClique para trocar"
      undefined:
        - "&amp;7Escolha uma Medalha para colocar"
        - "&amp;7nesta posição."
        - ""
        - "&amp;eClique para selecionar"

    medal2:
      name: '%color%&amp;l➜ %color%&lt;when="empty"&gt;%medal_name%&lt;/when="Slot de Medalha #2"&gt;'
      item: '&lt;when="empty"&gt;%medal_item%&lt;/when="RED_STAINED_GLASS_PANE"&gt;'
      slot: 22
      permission:
        - "&amp;7Você não tem permissão"
        - "&amp;7para usar este slot."
        - ""
        - "&amp;cSem permissão"
      selected:
        - "&amp;7Medalha com o"
        - "&amp;7símbolo %medal_icon%"
        - ""
        - "&amp;eClique para trocar"
      undefined:
        - "&amp;7Escolha uma Medalha para colocar"
        - "&amp;7nesta posição."
        - ""
        - "&amp;eClique para selecionar"

    medal3:
      name: '%color%&amp;l➜ %color%&lt;when="empty"&gt;%medal_name%&lt;/when="Slot de Medalha #3"&gt;'
      item: '&lt;when="empty"&gt;%medal_item%&lt;/when="RED_STAINED_GLASS_PANE"&gt;'
      slot: 24
      permission:
        - "&amp;7Você não tem permissão"
        - "&amp;7para usar este slot."
        - ""
        - "&amp;cSem permissão"
      selected:
        - "&amp;7Medalha com o"
        - "&amp;7símbolo %medal_icon%"
        - ""
        - "&amp;eClique para trocar"
      undefined:
        - "&amp;7Escolha uma Medalha para colocar"
        - "&amp;7nesta posição."
        - ""
        - "&amp;eClique para selecionar"

    reset:
      name: '&amp;c&amp;l➜ &amp;cRemover todas as Medalhas'
      item: 'barrier'
      slot: 36
      lore:
        - "&amp;7Remova todas as medalhas equipadas."

      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    # Itens extras
    book:
      name: '&amp;a&amp;l➜ &amp;aInformações'
      item: 'book'
      slot: 37
      lore:
        - "&amp;7Você pode adquirir &amp;6Medalhas"
        - "&amp;7jogando ou adquirindo em nosso site."
        - ""
        - "&amp;7É possível selecionar até"
        - "&amp;6Três Medalhas &amp;7ao mesmo tempo!"
        - ""
        - "&amp;7Adquira suas medalhas em"
        - "&amp;bhttps://site.com/medalhas"
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: []

    leave:
      name: '&amp;c&amp;l➜ &amp;cSair'
      item: 'red_dye'
      slot: 40
      lore: []

      # Fechará o inventário caso clique
      closeInventory: true

      # Lista de comandos que o jogador executará
      execute: []

select-menu:
title: "Selecione a Medalha #%slot%"
slots: 54

# Exibir todas as medalhas, mesmo se não houver permissão

show-all: false

# Itens das medalhas

medals:

# Slots que ocuparão

slots: [10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34]
name: "%color%&amp;l➜ %color%%medal_name%"
none:

- "&amp;eClique para remover"
  select:
- "&amp;7Medalha com o"
- "&amp;7símbolo %medal_icon%"
- ""
- "&amp;7Preview:"
- "%player_displayname% &amp;7%medals%"
- ""
- "&amp;eCategoria: %medal_rarity%"
- ""
- "&amp;eClique para equipar"
  permission:
- "&amp;7Você não tem permissão"
- "&amp;7para usar esta medalha."
- ""
- "&amp;7Medalha com o"
- "&amp;7símbolo %medal_icon%"
- ""
- "&amp;eCategoria: %medal_rarity%"
- ""
- "&amp;cSem permissão"

items:
leave:
name: '&amp;c&amp;l➜ &amp;cSair'
item: 'red_dye'
slot: 49
lore: []

      # Fechará o inventário caso clique
      closeInventory: false

    previous-page:
      name: "&amp;cPág. anterior"
      item: "arrow"
      slot: 45
      lore: []

    next-page:
      name: "&amp;cPróx. página"
      item: "arrow"
      slot: 53
      lore: []

</code-block>
</chapter>
</chapter>
<chapter title="settings/" collapsible="true">
<chapter title="commands.yml" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração

medal:
use-command: true
permission: ''
aliases:
- medals
- medalha
- medalhas

setmedal:
use-command: true
permission: leaftags.command.setmedal
aliases:
- setarmedalha
  usage: para definir uma medalha a alguém.
</code-block>
</chapter>
</chapter>
<chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
# Agradecemos por escolher o LeafMedals ♥
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

options:
# Fará que sempre que o jogador altere sua medalha, atualize instantaneamente no banco de dados
# Recomendado para desenvolvedores experientes
database-update: true

# Máximo de medalhas que o jogador poderá equipar
max-medals: 3

# Definir automaticamente no suffix do LeafTags
# caso não esteja sendo usado um suffix customizado
auto-suffix: false

# Selecionar as medalhas através de menu
# (Só funcionará desativado caso o máximo de medalhas seja 1)
select-menu: true
</code-block>
</chapter>
</chapter>