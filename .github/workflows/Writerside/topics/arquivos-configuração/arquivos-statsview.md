# arquivos-statsview

<chapter id="arquivos-statsview" title="Arquivos" collapsible="true">
    <chapter title="settings/" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração
statsview:
  name: statsview
  use-command: true
  permission: ''
  aliases: []
  usage: [jogador] para ver as estatisticas
        </code-block>
    </chapter>
    <chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
options:
  # Tempo em segundos que a ActionBar permanecerá
  delay: 2

# Distância de blocos entre os jogadores
blocks-range: 5

# Lista de mundos que aparecerão as stats
# Caso deixe vazia, mostrará em todos
allowed-worlds: []

message: "&eJogador &f{display} &7{clan}"

hooks:
player:
label: '{player}'
return: '%player_name%'
displayName:
label: '{display}'
return: '%player_displayname%'
currentTag:
label: '{currentTag}'
return: '%leaftags_tag_preset%'
clan:
label: '{clan}'
return: '<when="empty">%simpleclans_clan_color_tag%</when="&cSem clan">'
</code-block>
    </chapter>
</chapter>