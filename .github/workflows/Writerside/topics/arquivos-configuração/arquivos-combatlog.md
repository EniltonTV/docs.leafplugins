# arquivos-combatlog

<chapter id="arquivos-combatlog" title="Arquivos" collapsible="true">
    <chapter title="lang/" collapsible="true">
        <chapter title="messages_en.yml" collapsible="true">
            <code-block lang="yaml">
regions-reload: '&aThe combat regions cache has been cleared.'
combat-leave: '&aYou are no longer in combat! Feel free to disconnect.'
combat-join: '&cYou have entered combat with &7%player%&c! Do not log out or you will lose your items.'
combat-target-invalid: '&cPlayer &7%player% &cis not your opponent.'
combat-target-already: '&cPlayer &7%player% &cis already in combat.'
combat-command-cancel: '&cYou cannot use this command in combat.'
combat-enderpeal-cancel: '&cYou cannot use enderpearl in combat.'
combat-elytra-cancel: '&cNo se permite el uso de Elytra.'
combat-elytra-cancel-drop: '&cNo se permite el uso de Elytra. Tu objeto fue tirado por falta de espacio en el inventario.'
combat-elytra-cancel-removed: '&cNo se permite el uso de Elytra. Tu objeto ha sido colocado en tu inventario.'
combat-actionbar-end: '&aYou are no longer in combat!'
combat-actionbar-time: '&cYou are in combat for %time%s'
combat-actionbar-region-leave: '&cYou cannot leave your PvP region!'
combat-actionbar-region-protect: '&cYou cannot enter non-PvP regions!'
broadcast-player-quit: '&c[Combat] Player &7%player% &cdisconnected while in combat.'
            </code-block>
        </chapter>
        <chapter title="messaes_es.yml" collapsible="true">
            <code-block lang="yaml">
regions-reload: '&aSe ha borrado el caché de las regiones de combate.'
combat-leave: '&a¡Ya no estás en combate! Siéntete libre de desconectarte.'
combat-join: '&c¡Has entrado en combate con &7%player%&c! No te desconectes o perderás tus objetos.'
combat-target-invalid: '&cEl jugador &7%player% &cno es tu oponente.'
combat-target-already: '&cEl jugador &7%player% &cya está en combate.'
combat-command-cancel: '&cNo puedes usar este comando en combate.'
combat-enderpeal-cancel: '&cNo puedes usar enderpearl en combate.'
combat-elytra-cancel: '&cThe use of Elytra is not allowed.'
combat-elytra-cancel-drop: '&cThe use of Elytra is not allowed. Your item was dropped due to lack of inventory space.'
combat-elytra-cancel-removed: '&cThe use of Elytra is not allowed. Your item has been placed in your inventory.'
combat-actionbar-end: '&a¡Ya no estás en combate!'
combat-actionbar-time: '&cEstás en combate por %time%s'
combat-actionbar-region-leave: '&c¡No puedes salir de tu región de PvP!'
combat-actionbar-region-protect: '&c¡No puedes entrar en regiones sin PvP!'
broadcast-player-quit: '&c[Combate] El jugador &7%player% &cse desconectó estando en combate.'
            </code-block>
        </chapter>
        <chapter title="messaes_pt.yml" collapsible="true">
            <code-block lang="yaml">
regions-reload: '&aO cache de regiões de combate foi limpo.'
combat-leave: '&aVocê não está mais em combate! Sinta-se a vontade em desconectar.'
combat-join: '&cVocê entrou em combate com &7%player%&c! Não deslogue ou perderá seus itens.'
combat-target-invalid: '&cO jogador &7%player% &cnão é seu oponente.'
combat-target-already: '&cO jogador &7%player% &cjá está em combate.'
combat-command-cancel: '&cVocê não pode usar esse comando em combate.'
combat-enderpeal-cancel: '&cVocê não pode usar enderpearl em combate.'
combat-elytra-cancel: '&cNão é permitido o uso de elytra em combate.'
combat-elytra-cancel-drop: '&cNão é permitido o uso de elytra em combate. Seu item foi dropado por não haver espaço no inventário.'
combat-elytra-cancel-removed: '&cNão é permitido o uso de elytra em combate. Seu item foi colocado em seu inventário.'
combat-actionbar-end: '&aVocê não está mais em combate!'
combat-actionbar-time: '&cVocê está em combate por %time%s'
combat-actionbar-region-leave: '&cVocê não pode sair da sua região de PvP!'
combat-actionbar-region-protect: '&cNão pode entrar em regiões sem PvP!'
broadcast-player-quit: '&c[Combate] O jogador &7%player% &cdesconectou em combate.'
            </code-block>
        </chapter>
    </chapter>
    <chapter title="settings/" collapsible="true">
        <chapter title="commands.yml" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração

combatlog:
name: combatlog
use-command: true
permission: leafcombatlog.command.combatlog
aliases:
- combat
- sairdecombate
- cancelarcombate
- leavecombat
- cancelcombat

reloadregions:
name: reloadregions
use-command: true
permission: leafcombatlog.Admin
aliases:
- combatlogregions
</code-block>
        </chapter>
    </chapter>
    <chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
combatlog:
  # Tempo em segundos para que o combatlog termine
  combat-time: 15

# Manter o jogador em combate mesmo que aconteça uma destas coisas:
# Oponente morrer | Oponente desconectar
keep-after-end: false

# Fará que os jogadores entrem no modo SURVIVAL ao entrar em combate
auto-gamemode: true

# Fará que o fly seja desabilitado ao entrar em combate
disable-fly: true

# Matará o jogador ao desconectar em combate
kill-on-leave: true

# Forçará um drop seguro, fazendo que seja dropado no lugar onde morreu
# Evitando conflitos com plugins de auto-respawn
force-drop: true

# Não permitirá usar a Elytra em combate
cancel-elytra: true

# Fará que qualquer teleporte em combate para outro mundo seja cancelado
cancel-teleport: true

# Fará que não seja possível usar enderpeal em combate
cancel-enderpearl: true

# Fará que não entre em combate caso seja atingido por tais projéteis
# Você pode utilizar "ALL" para bloquear todos os projeteis
# Exemplo: enderpearl, snowball, arrow
cancel-entering-by-projectiles:
- enderpearl
- snowball

# Esta função é uma compatibilidade com WorldGuard
# Recomendamos que não crie multi-regiões dentro de uma para evitar conflitos
regions:
# O jogador visualizará blocos ao redor da região evitando que saia
# Observação: Somente com 'cancel-leave' ou 'cancel-protected' ativado
# Caso o servidor possua ProtocolLib, será usado um sistema melhor e mais otimizado
use-blocks: true

# Material do bloco que será exibido
# Padrão: RED_STAINED_GLASS
block-material: RED_STAINED_GLASS

# Efetuar os cálculos necessários no iniciamento do servidor
# Para evitar problemas de desempenho futuros
optimize-blocks: true

# Forçar o uso do sistema nativo de blocos mesmo tendo ProtocolLib
# Observação: Necessário reiniciar
native-blocks-method: false

# Não permitirá que o jogador saia da região que o combate iniciou
cancel-leave: true

# Fará que não permita o jogador entrar em uma região com "pvp" deny
# Isso desabilitará a opção "cancel-leave" caso "use-blocks" esteja true
cancel-protected: false

# Regiões que serão ignoradas no sistema
ignore-regions:
- IgnoredRegion

# Regiões que não usarão os blocos
blocks-ignore-regions:
- IgnoredRegion

bypass:
# Usará o sistema de bypass
enable: true

# Gamemode que permitirá o bypass
# Gamemodes -> ALL | SURVIVAL | CREATIVE | ADVENTURE
gamemode: ALL

# Permitir de usar qualquer comando
allow-commands: true

# Fará que não entre em combate
cancel-combat: false

# Permissão para ter bypass
permission: leafcombatlog.bypass

placeholders:
# A mensagem é separada por "<-->"
# Respeite o formato para que não haja erros
inCombat: '&aEm combate <--> &cFora de combate'

options:
# Usará a actionbar
action-bar: true

# Anunciará para todos quando um jogador desconectar em combate
# Caso desativado, enviará apenas para seu oponente
broadcast: true

# Avisar o jogador ao entrar em combate
combat-start-message: true

# Avisar o jogador ao sair de combate
combat-leave-message: true

# Sons que serão usados (Deixe vazio para desativar)
sounds:
# Som ao iniciar o combate
combat-start: WOOD_CLICK

    # Som ao encerrar o combate
    combat-end: LEVEL_UP

# Comandos que o console executará ao jogador vencedor
commands-on-win:
- money add %player% 10

# Comandos que o console executará ao jogador sair em combate
commands-on-leave:
- money remove %player% 10

# Comandos que serão permitidos usar em combate
allowed-commands:
- /l
- /g
- /tell

# Mundos que não será permitido "atrapalhar" combates (anti 2v1 etc)
# - Players em combate não poderão ser atingidos por outros jogadores, apenas pelo oponente
# - Players em combate não poderão atingir outros jogadores, apenas seu oponente
anti-boring-worlds:
- world
- MinaPvP
- ArenaPvP

# Mundos que não será usado o CombatLog
blocked-worlds:
- Lobby
- Spawn
- MainLobby
</code-block>
    </chapter>
</chapter>