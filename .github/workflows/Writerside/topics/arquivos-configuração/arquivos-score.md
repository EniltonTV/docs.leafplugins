# arquivos-score

<chapter id="arquivos-score" title="Arquivos" collapsible="true">
    <chapter title="lang/" collapsible="true">
        <chapter title="messages_en.yml" collapsible="true">
<code-block lang="yaml">
command-usage:
  - ''
  - '&a/%label% list &8- &7List of scoreboards and tablists'
  - '&a/%label% reset &8- &7Stop experimenting'
  - '&a/%label% scoreboard [id] &8- &7Try a scoreboard'
  - '&a/%label% tablist [id] &8- &7Try a tablist'
  - ''

command-list:
- '&7Scoreboards available: &a%scoreboards%'
- '&7Tablists available: &a%tablists%'

command-reset: '&aScoreboard and Tablist redefined.'
scoreboard-change: '&aScoreboard changed to &f%scoreboard%&a!'
scoreboard-not-found: '&cScoreboard not found or does not have permission.'
scoreboard-enable: '&e&lWARNING: &eYour scoreboard has been activated! You can opt out at any time.'
scoreboard-disable: '&e&lWARNING: &eYour scoreboard has been disabled! You can reactivate at any time.'
tablist-change: '&aTablist changed to &f%tablist%&a!'
tablist-not-found: '&cTablist not found or does not have permission.'
</code-block>
        </chapter>
        <chapter title="messages_es.yml" collapsible="true">
<code-block lang="yaml">
command-usage:
  - ''
  - '&a/%label% lista &8- &7Lista de scoreboards y tablists'
  - '&a/%label% reiniciar &8- &7Detener la experimentación'
  - '&a/%label% scoreboard [id] &8- &7Experimentar un scoreboard'
  - '&a/%label% tablist [id] &8- &7Experimentar una tablist'
  - ''

command-list:
- '&7Scoreboards disponibles: &a%scoreboards%'
- '&7Tablists disponibles: &a%tablists%'

command-reset: '&aScoreboard y Tablist restablecidos.'
scoreboard-change: '&a¡Scoreboard cambiado a &f%scoreboard%&a!'
scoreboard-not-found: '&cScoreboard no encontrado o no tiene permisos.'
scoreboard-enable: '&e&lADVERTENCIA: &e¡Su scoreboard ha sido activada! Puede desactivarla en cualquier momento.'
scoreboard-disable: '&e&lADVERTENCIA: &e¡Su scoreboard ha sido desactivada! Puede volver a activarla en cualquier momento.'
tablist-change: '&a¡Tablist cambiada a &f%tablist%&a!'
tablist-not-found: '&cTablist no encontrada o no tiene permisos.'
</code-block>
        </chapter>
        <chapter title="messages_pt.yml" collapsible="true">
<code-block lang="yaml">
command-usage:
  - ''
  - '&a/%label% list &8- &7Lista de scoreboards e tablists'
  - '&a/%label% reset &8- &7Parar de experimentar'
  - '&a/%label% scoreboard [id] &8- &7Experimentar uma scoreboard'
  - '&a/%label% tablist [id] &8- &7Experimentar uma tablist'
  - ''

command-list:
- '&7Scoreboards disponíveis: &a%scoreboards%'
- '&7Tablists disponíveis: &a%tablists%'

command-reset: '&aScoreboard e Tablist redefinida.'
scoreboard-change: '&aScoreboard alterada para &f%scoreboard%&a!'
scoreboard-not-found: '&cScoreboard não encontrada ou não possui permissão.'
scoreboard-enable: '&e&lWARNING: &eSua scoreboard foi ativada! Você pode desativar a qualquer momento.'
scoreboard-disable: '&e&lWARNING: &eSua scoreboard foi desativada! Você pode reativar a qualquer momento.'
tablist-change: '&aTablist alterada para &f%tablist%&a!'
tablist-not-found: '&cTablist não encontrada ou não possui permissão.'
</code-block>
        </chapter>
    </chapter>
    <chapter title="scores/" collapsible="true">
        <chapter title="scoreboards.yml" collapsible="true">
<code-block lang="yaml">
# https://docs.leafplugins.com/v/score/tutorials
# O LeafScore suporta scoreboards da versão beta

# Exemplo de Scoreboard por mundo
plotme:
titles:
frames:
- '&6&lTERRENOS'
interval: 0.0
lines:
1:
frames: ['']
interval: 0.0
condition: ""
2:
frames:
- '&fAdquira um terreno usando:'
- '&fDúvidas?'
interval: 5
condition: ''
3:
frames:
- '&a/plot auto'
- '&b/plot help'
interval: 5
condition: ''
4:
frames: ['']
interval: 0.0
condition: ''
5:
frames:
- "&fJogadores: &a%server_online%"
interval: 0.0
condition: ''
6:
frames: ['']
interval: 0.0
condition: ''
site:
frames:
- "&ewww.leafplugins.com"
interval: 0.0
condition: ''
options:
worlds: ['plotme', 'plotme_world', 'Plotme', 'Plots']
regions: []
permission: ''

# Exemplo de Scoreboard por região
regions:
titles:
frames:
- '&a&lREGION'
- '&a&lSCORE'
interval: 0.6
lines:
1:
frames: ['']
interval: 0
condition: ""
2:
frames:
- 'Você está em uma região'
- 'com scoreboard exclusiva'
interval: 2
condition: ''
3:
frames:
- ''
interval: 0.0
condition: ''
5:
frames:
- '&ewww.leafplugins.com'
interval: 0.2
condition: ''
options:
worlds: []
# Regiões que a scorebord será enviada
regions: [spawn]
permission: ''

# Scoreboard padrão do servidor (Configuração antiga)
# O plugin suporta esse formato para scoreboards estáticas
# Além disso, os parametros de animação também funcionam
default-legacy:
# Caso haja mais de um nesta lista, fará um título animado
titles:
- '<rainbow:5>&lLEAF</rainbow> &8▪ &7%server_online%'
- '<rainbow:5>&lSCORE</rainbow> &8▪ &7%server_online%'
# Linhas da scoreboard
lines:
- ''
- '&fCargo: &7%leaftags_tag_preset%'
- '&fClan: '%simpleclans_clan_color_tag%'
- '%simpleclans_clan_total_kdr%">%simpleclans_clan_color_tag%'
- ''
- '&eBanco:'
- ' &fCoins: &2$&f%vault_eco_balance_formatted%'
- ' &fCash: &6✪%playerpoints_points%'
- ''
- '&fJogadores: &a%server_online%'
- ''
- '&7leafplugins.com'
options:
# Tempo em segundos para que o titulo atualize para o próximo da lista (ANIMAÇÃO)
title-update: 0.8
# Mundos que a scoreboard será enviada
worlds: []
# Essa scoreboard será enviada apenas para quem ter a permissão (Deixe vazio para ser para todos)
permission: ''

# Scoreboard padrão do servidor
default:
# Titulo da Scoreboard
titles:
# Caso haja mais de um nesta lista, fará um titulo animado
frames:
- '<rainbow:13>&lLeaf Plugins</rainbow>'
- 'stay:5 &lLeaf Plugins'
- '<rainbow:1>&l<scroll:left>Leaf Plugins</scroll></rainbow>'
- '<rainbow:1>&l<scroll:rightt>Leaf Plugins</scroll></rainbow>'
interval: 0.2

# Linhas da Scoreboard
lines:
1:
# Caso haja mais de um nesta lista, fará uma linha animada
frames: ['']
# Intervalo para mudar de frame (0.1 minimo para animações)
interval: 0.0
# Condição para visualizar esta linha
condition: ""
2:
frames:
- '&fCargo: &7%leaftags_tag_preset%'
interval: 0.5
condition: ''
3:
frames: ['']
interval: 0.0
condition: ''
4:
frames:
- '&fClan: %simpleclans_clan_color_tag%'
interval: 0.0
condition: ''
5:
frames: ['']
interval: 0.0
condition: 'noClan'
6:
frames:
- ' <rainbow:5>»</rainbow> &fKDR: &a%simpleclans_clan_total_kdr%'
- ' <rainbow:5>»</rainbow> &fKills: &a%simpleclans_clan_total_kills%'
- ' <rainbow:5>»</rainbow> &fDeaths: &a%simpleclans_clan_total_deaths%'
interval: 1
condition: 'hasClan'
7:
frames:
- ''
interval: 0.0
condition: 'hasClan'
8:
frames:
- '&eBanco:'
interval: 0.0
condition: ''
9:
frames:
- ' &fCoins: &2$&f%vault_eco_balance_formatted%'
interval: 0.0
condition: ''
10:
frames:
- ' &fCash: &6✪%playerpoints_points%'
interval: 0.0
condition: ''
11:
frames: ['']
interval: 0.0
condition: ''
12:
frames:
- 'Jogadores: &a%server_online%'
interval: 0.0
condition: ''
13:
frames: ['']
interval: 0.0
condition: ''
site:
frames:
- '<rainbow:13>www.leafplugins.com</rainbow>'
- 'stay:5 &ewww.leafplugins.com'
interval: 0.2
condition: ''
options:
# Mundos que a scoreboard será enviada
worlds: []
# Regiões que a scorebord será enviada
regions: []
# Essa scoreboard será enviada apenas para quem ter a permissão (Deixe vazio para ser para todos)
permission: ''
</code-block>
        </chapter>
        <chapter title="tablists.yml" collapsible="true">
<code-block lang="yaml">
plotme:
  header:
    - ""
    - "&6&lTERRENOS"
    - ""
    - "&7Seu cargo: %leaftags_tag_preset%"
    - "&7Sua conexão: &a%player_ping%ms"
    - ""
  footer:
    - ""
    - "&7Nossa loja: &bwww.leafplugins.com"
    - "&7Nosso discord: &9discord.leafplugins.com"
    - ""
  options:
    # Mundos que a tablist será enviada
    worlds: ["Plotme"]
    # Essa tablist será enviada apenas para quem ter a permissão (Deixe vazio para ser para todos)
    permission: ""

default:
header:
- ""
- "&b&lLEAFSCORE"
- ""
- "&7Seu cargo: %leaftags_tag_preset%"
- "&7Sua conexão: &a%player_ping%ms"
- ""
footer:
- ""
- "&7Nossa loja: &bwww.leafplugins.com"
- "&7Nosso discord: &9discord.leafplugins.com"
- ""
options:
# Mundos que a tablist será enviada
worlds: []
# Essa tablist será enviada apenas para quem ter a permissão (Deixe vazio para ser para todos)
permission: ""
</code-block>
        </chapter>
    </chapter>
    <chapter title="settings/" collapsible="true">
        <chapter title="commands.yml" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração

changescore:
name: changescore
use-command: true
permission: leafscore.command.score
aliases:
- changescoreboard
- mudarscoreboard
- mudarscore
usage: ''

scoreboardtoggle:
name: scoreboardtoggle
use-command: true
permission: ''
aliases:
- sb
- scoreboard
- stoggle
usage: <true:false> para ativar/desativar sua scoreboard.
</code-block>
        </chapter>
    </chapter>
    <chapter title="conditions.yml" collapsible="true">
<code-block lang="yaml">
# Condições de Scoreboard e linhas
conditions:
  hasClan:
    placeholder: "%simpleclans_clan_color_tag%"
    condition: "not-empty"
    # Caso a placeholder não esteja vazia o resultado será 'true'
    result: true
  noClan:
    placeholder: "%simpleclans_clan_color_tag%"
    condition: "empty"
    # Caso a placeholder esteja vazia o resultado será 'true'
    result: true
</code-block>
    </chapter>
    <chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
# Agradecemos por escolher o LeafScore ♥
# Desejamos que tudo ocorra da melhor forma para você,
# e que seus esforços sejam recompensados!

# https://docs.leafplugins.com/v/score/tutorials

defaults:
# Tablist padrão do servidor (Deixe vazio para desativar)
tablist: default

# Scoreboard padrão do servidor (Deixe vazio para desativar)
scoreboard: default

# Ativar/desativar modo de depuração
# Quando ativado, o plugin registrará informações detalhadas de depuração
# Útil para diagnóstico de problemas
debug-mode: false

# Fará que as expansões básicas sejam baixadas
expansions-download: true

# Segundos para as scoreboards serem reenviadas (Deixe 0 para desativar)
resend-scoreboard: 20

# Opções de bloqueio
block-options:
# Removerá a scoreboard nos mundos bloqueados
disable-scoreboard: true

# Caso esteja 'true', fará que apenas os mundos da lista "worlds"
# tenha scoreboards (Invertendo de blocked para whitelist)
white-list: false

# Mundos que terão a scoreboard bloqueada
# Caso o white-list esteja 'true',
# fará que somente estes mundos tenham scoreboards
worlds:
- blockedWorld
</code-block>
</chapter>
</chapter> 