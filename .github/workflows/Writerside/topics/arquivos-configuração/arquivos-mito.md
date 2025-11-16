# arquivos-mito

<chapter id="arquivos-mito" title="Clique aqui" collapsible="true">
    <chapter title="lang/" collapsible="true">
        <chapter title="messages_pt.yml" collapsible="true">

<code-block lang="yaml">
broadcasts:
  # Placeholders disponíveis:
  # %player% - nome do mito
  # %display% - display do mito (caso esteja online, caso esteja offline, retornará o nome)
  # %killer% - nome do killer
  # %displaykiller% - display do killer
  #
  # Para desativar um broadcast, deixe-o vazio
  morto:
    - ''
    - '&c[MITO] &fO &7%display% &ffoi morto por &7%displaykiller% &fe perdeu sua tag!'
    - ''
  setado:
    - ''
    - '&c[MITO] &fO &7%display% &fse tornou o novo mito!'
    - ''
  ausente:
    - ''
    - '&c[MITO] &fO &7%player% &fperdeu sua tag por inatividade!'
    - ''
  removido:
    - ''
    - '&c[MITO] &fO &7%player% &fteve sua tag retirada por um Administrador.'
    - ''

command:
npc-setado: '&aLocalização para o NPC setada com sucesso!'
mito-transferencia-ativada: '&aTransferência de mito por morte ativada!'
mito-transferencia-pausada: '&eTransferência de mito por morte pausada até ser reativada ou o servidor reiniciar!'
mito-remover-nenhum: '&cO servidor não possui um mito!'
mito-resetar: '&aQuantidade de vezes que %player% foi mito resetada!'
mito-resetar-block: '&cO jogador %player% é o mito atual ou nunca foi mito.'
mito-random-nenhum: '&cNão há jogadores online para ser sorteado.'
mito-atual:
- '&c[MITO] &f%player% &7é o atual mito do servidor pela &f%times%ª vez&7!'
  mito-atual-nenhum:
- '&c[MITO] &7Nenhum mito definido!'
</code-block>
        </chapter>
    </chapter>
    <chapter title="menus/" collapsible="true">
        <chapter title="mito-menu.yml" collapsible="true">
<code-block lang="yaml">
main-menu:
  title: "Mitos - Principal"
  slots: 27

items:
# Não altere o ID dos seguintes itens: mito-atual, mito-nenhum, top-list
mito-atual:
name: "&6&l➜ &6Mito Atual"
item: "head:%mitoname%"
slot: 13
lore:
- ""
- " &a%mitotimes%ª vez &fde &7%mitoname%"
- ""
- "&8Desde %mitodate%"

  mito-nenhum:
  name: "&c&l➜ &cMito Atual"
  item: "player_head"
  slot: 13
  lore:
  - ""
  - " &fNenhum jogador"
  - " &e&lPODE SER VOCÊ!"
  - ""

  top-list:
  name: "&b&l➜ &bTop Mitos"
  item: "head:a988419dd5b386f698a96913db1d97c2418e16d416d7f439d48acd41e3a436ce"
  slot: 15
  lore:
  - ""
  - " &fConfira o histórico de mitos"
  - ""

  # Itens extras
  player:
  name: '&a&l➜ &aMinhas informações'
  item: 'head:player'
  slot: 11
  lore:
  - ""
  - " &fMito por &a%times% vez(es)"
  - " &fÚltima vez: &7%date%"
  - ""
  # Fechará o inventário caso clique
  closeInventory: false

      # Lista de comandos que o jogador executará
      execute: [ ]

top-menu:
title: "Mitos - Top List"
slots: 54

list:
# Slots que os itens ocuparão
slots: [ 10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 28, 29, 30, 31, 32, 33 ]

    # Formato dos itens dos mitos
    format:
      name: "&c%name%"
      item: "head:%name%"
      lore:
        - ""
        - " &fMito por &a%times% vez(es)"
        - ""

items:
return:
name: "&7Voltar"
item: "head:a988419dd5b386f698a96913db1d97c2418e16d416d7f439d48acd41e3a436ce"
slot: 49
lore:
- ""
- "&7 Você está visualizando o histórico"
- "&7 de mitos do servidor"
- ""
- "&eClique para voltar"

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
mito:
  name: mito
  use-command: true
  permission: ''
  aliases:
    - mitos
    - mitopvp
  usage: ''
</code-block>
    </chapter>
    <chapter title="discord.yml" collapsible="true">
<code-block lang="yaml">
# Insira a Webhook Geral do canal que irá enviar as embeds
# Caso as embeds não hajam "webhook" individuais, serão usadas esta:
webhookURL: ""

# Observação: É necessário ter baixado o LeafDiscord em seu servidor

embeds:
# Placeholders disponíveis:
# %player% - nome do jogador
# %uuid% - uuid do jogador
# %times% - quantidade de vezes
# %player_icon% - URL do icone do jogador
update:
enable: true
webhook: ""
title: ""
color: "#ff3535"
thumbnailURL: "%player_icon%"
description: "## ⚔️ %player% é o **NOVO MITO!**\n # ```Pela %times%ª vez o jogador se mostra IMBATÍVEL!```"
field-inline: true
fields: [ ]
# O que vier antes do -> será o nome da field
# O que vier após o -> será o texto da field
footer: "www.leafplugins.com"
footerURL: ""
inactive:
enable: true
webhook: ""
title: ""
color: "#ffcf1b"
thumbnailURL: "%player_icon%"
description: "## ⚔️ %player%  **PERDEU SEU MITO!**\n # ```O jogador perdeu por inatividade.```"
field-inline: true
fields: [ ]
# O que vier antes do -> será o nome da field
# O que vier após o -> será o texto da field
footer: "www.leafplugins.com"
footerURL: "https://static.wikia.nocookie.net/minecraft_gamepedia/images/3/3e/Clock_JE3_BE3.gif/revision/latest/thumbnail/width/360/height/360?cb=20201125194053"
</code-block>
    </chapter>
    </chapter>
    <chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
# Agradecemos por escolher o LeafMito ♥
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

# [PREMIUM] Abrir menu quando usar /mito sem permissão de gerenciar
open-menu: true

mito:
# Tag do Mito
tag: '&c[MITO]'

# Som enviado a todos os jogadores (Deixe vazio para desativar)
sound: LEVEL_UP

# Cair um efeito de raio no novo mito
thunder: true

# Spawnar entidades ao redor do novo mito (Deixe vazio para desativar)
spawn-entities:
- BAT 5x

# Defina o máximo de dias que o jogador
# poderá ficar com a TAG sem se conectar no servidor
max-days-offline: 20

# Comando que o console executará quando um jogador se tornar o mito
commands:
- give %player% golden_apple 32

# Titulo enviado para todos
title:
enable: true
title: '&6&lMITO'
subtitle: '&c%display% &fse tornou o melhor!'

# Mensagens de Conexão (PlaceholderAPI disponivel)
# Deixe vazio para desativar a mensagem em especifico
connection:
broadcasts:
enable: true
join:
- ''
- '&a[MITO] &fO jogador &7%player_displayname% &fentrou.'
- ''
  leave:
- ''
- '&c[MITO] &fO jogador &7%player_displayname% &fsaiu.'
- ''
  actionbar:
  enable: true
  join: '&a[MITO] &fO jogador &7%player_displayname% &fentrou.'
  leave: '&c[MITO] &fO jogador &7%player_displayname% &fsaiu.'

npc:
# Utilizar o NPC (Necessário usar o Citizens)
enable: true

# Efeito de brilho no NPC
glowing: true

# Efeito de raio quando houver mudança do mito atual
thunder: true

# Nome da skin caso não possua um mito
none-skin: Fleivius

# Holograma do NPC
hologram:
height: 2.9
none:
- '&6&lMITO ATUAL'
- Nenhum &fjogador
- '&b» &e&lPODE SER VOCÊ! &b«'
  current:
- '&6&lMITO ATUAL > %player%'
- '&f&c&lIMBATÍVEL &fdesde &a%date%'
- '&b» &e&l%times%ª VEZ &b«'
</code-block>
    </chapter>
</chapter>
