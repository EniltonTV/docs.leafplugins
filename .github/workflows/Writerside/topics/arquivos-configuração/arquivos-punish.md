# arquivos-punish

<chapter id="arquivos-punish" title="Arquivos" collapsible="true">
    <chapter title="lang/" collapsible="true">
        <chapter title="messages_en.yml" collapsible="true">
<code-block lang="yaml">
punish-expires-never: Never
punish-status-active: Active
punish-status-inactive: Inactive

command-usage-temp-proof: <player> <proof> <duration> <reason> %usage%
command-usage-temp: <player> <duration> <reason> %usage%
command-usage-proof: <player> <proof> <reason> %usage%
command-usage-target: <player> %usage%
command-usage: <player> <reason> %usage%

command-punishment-not-found: '&cPunishment ''%id%'' not found.'
command-punishment-failed: '&cIt was not possible to carry out this punishment.'
command-punishment-failed-2: '&cPlayer &f%player%&c is already punished with &f%type%&c.'
command-punishment-processing: '&aProcessing punishment...'
command-punishment-proof: \\n&aType a test in the chat to continue!\\n&cType &nancel&c to cancel!\\n
command-punishment-confirm: \\n&7You are about to punish &c%player%\\n&7Do you want to confirm this punishment?\\n{cancel} {confirm} {silent}\\n
command-punishment-cancel: '&aPunishment cancelled.'
command-requires-reason: '&cYou must enter a reason.'
command-requires-proof: '&cA proof is required.'
command-requires-proof-link: '&cThe proof must start with one of these addresses: &f%prooflinks%&c.'
command-requires-duration: '&cYou must enter a duration.'
command-requires-duration-examples: '&cUse one of these formats: &f1min, 1h, 1d, 1m, 1y&c.'
command-no-permission-target: '&cYou cannot punish this player.'
command-reason-not-found: '&cThe reason ''%reason%'' was not found.'
command-banning-concluded: '&aYou have successfully banned &f%player% &afor &f%reason%&a!'
command-muting-concluded: '&aYou have successfully muted &f%player% &afor &f%reason%&a!'
command-kick-concluded: '&aYou have successfully kicked &f%player% &afor &f%reason%&a!'
command-warn-concluded: '&aYou have successfully warned &f%player% &afor &f%reason%&a! (%current%/%max%)'
command-warn-punished: '&aThe player &f%player% &ahas exceeded the maximum alerts and has been punished!'
command-warn-failed: '&cUnable to issue this alert.'
command-pardonid-concluded: '&aPunishment ''%id%'' has been revoked successfully!'
command-pardon-concluded: '&f%player% &apunishment revoked successfully!'
command-pardon-concluded-2: '&f%player% &apunishments successfully revoked!'
command-pardon-failed: '&cPlayer &f%player% &chas no punishments.'
command-pardon-failed-2: '&cThe player &f%player% &chas no active &f%type%&c.'
command-punishedit-concluded: '&f''%info%'' &ainformation from &f#%id% &achanged to &f''%result%'''
command-punishedit-examples: '&cInformation that can be changed: &freason, proof, expires, server&c.'
command-clearwarnings-concluded: '&f%player% &awarnings removed!'
command-clearwarnings-failed: '&cPlayer &f%player% &chas no warnings.'
command-clearhistoric-concluded: '&f%player% &ahistoric cleared successfully!'
command-clearhistoric-failed: '&cPlayer &f%player% &cdoes not have a punishment history.'
command-punish-creating-input: '&7You can cancel by typing &fcancel&7!'
command-punish-creating-type: '&cYou need to select the type of punishment.'
command-punish-creating-proof: '&cType in chat to provide the evidence.\n&cThe evidence must start with one of these addresses: &f%prooflinks%&c.'
command-punish-creating-reason: '&cType in chat to provide the reason or select one.'
command-punish-creating-server: '&cType in chat to select the server.\n&cUse &fGlobal &cto punish on all servers or use one of the following servers: &f%servers%'
command-punish-creating-duration: '&cType in chat to set the duration.\n&cUse one of these formats: &f1s, 1min, 1h, 1d, 1m, 1y&c.'

warns:
pardon:
- '&aYour punishment has been revoked!'
- ''
- '&aPunishment: &f%type%'
- '&aPunished on: &f%date%'
- ''
- '&aAfter a review, we have decided to remove it'
- '&aOur team apologizes for &nany inconvenience'
- ''
expired:
- '&aYour punishment has expired!'
- ''
- '&aPunishment: &f%type%'
- '&aPunished on: &f%date%'
- ''
- '&aOur team apologizes for &nany inconvenience'
- ''
warn:
- ''
- '&cYou have been warned!'
- ''
- '&cReason: &f%reason%'
- '&cAuthor: &f%author%'
- '&cChances: &f%current%/%max%'
- ''
- '&cIf you exceed the limit, you will be punished'
- ''
mute:
- ''
- '&cYou are permanently muted!'
- ''
- '&cReason: &f%reason%'
- '&cAuthor: &f%author%'
- '&cEvidence: &f%proof%'
- ''
- '&cPunished unfairly? Contact us at'
- '&c&nleafplugins.com'
- ''
tempmute:
- ''
- '&cYou are temporarily muted!'
- ''
- '&cReason: &f%reason%'
- '&cAuthor: &f%author%'
- '&cEvidence: &f%proof%'
- '&cExpires on: &f%expires%'
- ''
- '&cPunished unfairly? Contact us at'
- '&c&nleafplugins.com'
- ''

broadcasts:
status:
- ''
- ' &4[SERVER PUNISHMENTS]'
- ' &fIn our server, &c&l%total%&f punishments have been recorded.'
- ' &fAround &c&l%bans% &fbans and &c&l%mutes%&f mutes in %hours% hours!'
- ' &cKeep reporting offending players to assist our team.'
- ''
prevented:
- ''
- §c(!) Player &f%player% &ctried to join while banned.
- ''
warn:
- ''
- '&c(!) Player &f%player% &cwas warned.'
- '&c(!) Reason: &f%reason%'
- '&c(!) Author: &f%author%'
- '&c(!) Chances: %current%/%max%'
- ''
kick:
- ''
- '&c(!) The player &f%player% &cwas disconnected.'
- '&c(!) Reason: &f%reason%'
- '&c(!) Author: &f%author%'
- ''
mute:
- ''
- '&c(!) Player &f%player% &chas been permanently muted.'
- '&c(!) Reason: &f%reason%'
- '&c(!) Author: &f%author%'
- ''
tempmute:
- ''
- '&c(!) Player &f%player% &chas been temporarily muted.'
- '&c(!) Reason: &f%reason%'
- '&c(!) Author: &f%author%'
- '&c(!) Expires in: &f%expires%'
- ''
ban:
- ''
- '&c(!) The player &f%player% &chas been permanently banned.'
- '&c(!) Reason: &f%reason%'
- '&c(!) Author: &f%author%'
- ''
tempban:
- ''
- '&c(!) The player &f%player% &chas been temporarily banned.'
- '&c(!) Reason: &f%reason%'
- '&c(!) Author: &f%author%'
- '&c(!) Expires in: &f%expires%'
- ''
pardon:
- ''
- '&c(!) The player &f%player% &chas had their punishment revoked.'
- '&c(!) Type: &f%type%'
- '&c(!) Author: &f%author%'
- ''

disconnects:
kick:
- '&cYou have been disconnected: &f%reason%'
ban:
- '&cYou have been permanently banned.'
- '&cReason: &f%reason%'
- '&cPunishment ID: &f#%id%'
- ''
- '&7Purchase an unban at: &bwww.leafplugins.com'
- '&cBanned unfairly? Contact us at'
- '&cwww.leafplugins.com/appeal'
tempban:
- '&cYou have been temporarily banned.'
- '&cReason: &f%reason%'
- '&cPunishment ID: &f#%id%'
- ''
- '&cExpires on: &f%expires%'
- ''
- '&7Get your unban at: &bwww.leafplugins.com'
- '&cBanned unfairly? Contact us via'
- '&cwww.leafplugins.com/appeal'
</code-block>
        </chapter>
        <chapter title="messages_es.yml" collapsible="true">
<code-block lang="yaml">
punish-expires-never: Nunca
punish-status-active: Activo
punish-status-inactive: Inactivo

command-usage-temp-server: <jugador> <servidor> <duración> <motivo> %usage%
command-usage-temp-server-proof: <jugador> <servidor> <prueba> <duración> <motivo> %usage%
command-usage-temp-target-server-reason: <jugador> <servidor> <duración> <motivo> %usage%
command-usage-server-proof: <jugador> <servidor> <prueba> <motivo> %usage%
command-usage-target-server-reason: <jugador> <servidor> <motivo> %usage%
command-usage-temp-proof: <jugador> <prueba> <duración> <motivo> %usage%
command-usage-temp: <jugador> <duración> <motivo> %usage%
command-usage-proof: <jugador> <prueba> <motivo> %usage%
command-usage-target-server: <jugador> <servidor> %usage%
command-usage-target: <jugador> %usage%
command-usage: <jugador> <motivo> %usage%

command-punishment-processing: '&aProcesando castigo...'
command-punishment-proof: \\n&a¡Escribe una prueba en el chat para continuar!\\n&cEscribe &ncancel&c para cancelar!\\n
command-punishment-confirm: \\n&7Estás a punto de castigar a &c%player%\\n&7¿Deseas confirmar este castigo?\\n{cancel} {confirm} {silent}\\n
command-punishment-cancel: '&aCastigo cancelado.'

command-banning-concluded: '&aHas baneado a &f%player% &apor &f%reason% &acon éxito en &f%server%&a!'
command-muting-concluded: '&aHas silenciado a &f%player% &apor &f%reason% &acon éxito en &f%server%&a!'
command-kick-concluded: '&aHas expulsado a &f%player% &apor &f%reason% &acon éxito en &f%server%&7!'
command-warn-concluded: '&aHas advertido a &f%player%&apor &f%reason% &acon éxito! (%current%/%max%)'
command-warn-punished: '&a¡El jugador &f%player% &aha excedido el máximo de advertencias y ha sido castigado!'
command-pardonid-concluded: '&a¡El castigo ''%id%'' ha sido revocado con éxito!'
command-pardon-concluded: '&aCastigo de &f%player% &arevocado con éxito en &f%server%&a!'
command-pardon-concluded-2: '&aCastigos de &f%player% &arevocados con éxito en &f%server%&a!'
command-punishedit-concluded: '&aInformación &f''%info%'' &ade &f#%id% &aalterada a &f''%result%'''
command-clearwarnings-concluded: '&a¡Advertencias de &f%player% &aeliminadas!'
command-clearhistoric-concluded: '&aHistorial de &f%player% &alimpiado con éxito!'

command-punishment-not-found: '&cNo se encontró el castigo ''%id%''.'
command-punishment-failed: '&cNo se pudo realizar este castigo.'
command-punishment-failed-2: '&cEl jugador &f%player%&c ya está castigado con &f%type% &cen &f%server%&c.'
command-something-is-missing: '&cFalta alguna información.'
command-requires-server: '&cDebes ingresar un servidor.'
command-requires-reason: '&cDebes ingresar un motivo.'
command-requires-proof: '&cDebes ingresar una prueba.'
command-requires-proof-link: '&cLa prueba debe comenzar con uno de estos enlaces: &f%prooflinks%&c.'
command-requires-duration: '&cDebes ingresar una duración.'
command-requires-duration-examples: '&cUsa uno de estos formatos: &f1min, 1h, 1d, 1m, 1a&c.'
command-no-permission-target: '&cNo puedes castigar a este jugador.'
command-blocked-nick: '&cEste jugador está en la lista de nombres que no pueden ser castigados.'
command-target-is-you: '&cNo puedes castigarte a ti mismo.'
command-group-hierarchy: '&cEl rango del jugador es superior o igual al tuyo.'
command-reason-not-found: '&cNo se encontró el motivo ''%reason%''.'
command-server-not-found: '&cUsa &fGlobal &cpara castigar en todos o usa uno de los servidores: &f%servers%'
command-warn-failed: '&cNo se pudo realizar esta advertencia.'
command-pardon-failed: '&cEl jugador &f%player% &cno tiene castigos en &f%server%&c.'
command-pardon-failed-2: '&cEl jugador &f%player% &cno tiene &f%type% &cactivo en &f%server%&c.'
command-punishedit-examples: '&cInformación que se puede cambiar: &fmotivo, prueba, expirar, servidor&c.'
command-clearwarnings-failed: '&cEl jugador &f%player% &cno tiene advertencias.'
command-clearhistoric-failed: '&cEl jugador &f%player% &cno tiene un historial de castigos.'
command-historic-failed: '&cNo se encontraron castigos sufridos por este jugador.'
command-historic-author-failed: '&cNo se encontraron castigos realizados por este jugador.'
command-punish-creating-input: '&7¡Puedes cancelar escribiendo &fcancel&7!'
command-punish-creating-type: '&cDebes seleccionar el tipo de castigo.'
command-punish-creating-proof: '&cEscribe en el chat para ingresar la prueba.\n&cDebe comenzar con uno de estos enlaces: &f%prooflinks%&c.'
command-punish-creating-reason: '&cEscribe en el chat para ingresar el motivo o seleccionarlo.'
command-punish-creating-server: '&cEscribe en el chat para seleccionar el servidor.\n&cUsa &fGlobal &cpara castigar en todos o usa uno de los servidores: &f%servers%'
command-punish-creating-duration: '&cEscribe en el chat para establecer la duración.\n&cUsa uno de estos formatos: &f1s, 1min, 1h, 1d, 1m, 1a&c.'

ban-server-action-cancel: '&cNo puedes hacer esto.'
ban-server-command-cancel: '&cNo puedes usar este comando.'

warns:
pardon:
- '&a¡Tu castigo ha sido revocado!'
- ''
- '&aCastigo: &f%type%'
- '&aCastigado en: &f%date%'
- ''
- '&aTras un análisis, decidimos retirarlo'
- '&aNuestro equipo se disculpa por &ncualquier inconveniente'
- ''
expired:
- '&a¡Tu castigo ha expirado!'
- ''
- '&aCastigo: &f%type%'
- '&aCastigado en: &f%date%'
- ''
- '&aNuestro equipo se disculpa por &ncualquier inconveniente'
- ''
warn:
- ''
- '&c¡Has sido advertido!'
- ''
- '&cMotivo: &f%reason%'
- '&cAutor: &f%author%'
- '&cOportunidades: &f%current%/%max%'
- ''
- '&cSi excedes el límite, serás castigado'
- ''
mute:
- ''
- '&c¡Estás silenciado permanentemente!'
- ''
- '&cMotivo: &f%reason%'
- '&cAutor: &f%author%'
- '&cPrueba: &f%proof%'
- ''
- '&c¿Castigado injustamente? Contáctanos en'
- '&c&nleafplugins.com'
- ''
tempmute:
- ''
- '&c¡Estás silenciado temporalmente!'
- ''
- '&cMotivo: &f%reason%'
- '&cAutor: &f%author%'
- '&cPrueba: &f%proof%'
- '&cExpira en: &f%expires%'
- ''
- '&c¿Castigado injustamente? Contáctanos en'
- '&c&nleafplugins.com'
- ''

broadcasts:
status:
- ''
- ' &4[CASTIGOS DEL SERVIDOR]'
- ' &fEn nuestro servidor, &c&l%total%&f castigos han sido registrados.'
- ' &f¡Alrededor de &c&l%bans% &fbaneos y &c&l%mutes%&f silenciamientos en %hours%
horas!'
- ' &cSigue denunciando jugadores infractores para ayudar a nuestro equipo.'
- ''
# Placeholders disponibles:
# %total% - total de castigos
# %total_period% - total de castigos en el período
# %bans% - baneos en el período
# %mutes% - silenciamientos en el período
# %hours% - horas definidas en el periodo
prevented:
- ''
- §c(!) El jugador &f%player% &cintentó ingresar estando baneado.
- ''
warn:
- ''
- '&c(!) El jugador &f%player% &cfue advertido.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Oportunidades: %current%/%max%'
- ''
kick:
- ''
- '&c(!) El jugador &f%player% &cfue desconectado.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- ''
mute:
- ''
- '&c(!) El jugador &f%player% &cfue silenciado permanentemente.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Servidor: &f%server%'
- ''
tempmute:
- ''
- '&c(!) El jugador &f%player% &cfue silenciado temporalmente.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Expira en: &f%expires%'
- '&c(!) Servidor: &f%server%'
- ''
ban:
- ''
- '&c(!) El jugador &f%player% &cfue baneado permanentemente.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Prueba: &f%proof%'
- '&c(!) Servidor: &f%server%'
- ''
tempban:
- ''
- '&c(!) El jugador &f%player% &cfue baneado temporalmente.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Prueba: &f%proof%'
- '&c(!) Expira en: &f%expires%'
- '&c(!) Servidor: &f%server%'
- ''
pardon:
- ''
- '&c(!) El castigo de &f%player% &cfue revocado.'
- '&c(!) Castigo: &f%type%'
- '&c(!) Autor: &f%author%'
- '&c(!) Servidor: &f%server%'
- ''

disconnects:
kick:
- '&cHas sido desconectado: &f%reason%'
ban:
- '&cHas sido baneado permanentemente.'
- '&cMotivo: &f%reason%'
- '&cPrueba: &f%proof%'
- '&cID del castigo: &f#%id%'
- ''
- '&7Obtén tu desbaneo en: &bwww.leafplugins.com'
- '&c¿Baneado injustamente? Contáctanos vía'
- '&cwww.leafplugins.com/appeal'
tempban:
- '&cHas sido baneado temporalmente.'
- '&cMotivo: &f%reason%'
- '&cPrueba: &f%proof%'
- '&cID del castigo: &f#%id%'
- ''
- '&cExpira en: &f%expires%'
- ''
- '&7Obtén tu desbaneo en: &bwww.leafplugins.com'
- '&c¿Baneado injustamente? Contáctanos vía'
- '&cwww.leafplugins.com/appeal'
</code-block>
        </chapter>
        <chapter title="messages_pt.yml" collapsible="true">
<code-block lang="yaml">
punish-expires-never: Nunca
punish-status-active: Ativo
punish-status-inactive: Inativo

command-usage-temp-server: <jogador> <servidor> <duração> <motivo> %usage%
command-usage-temp-server-proof: <jogador> <servidor> <prova> <duração> <motivo> %usage%
command-usage-temp-target-server-reason: <jogador> <servidor> <duração> <motivo> %usage%
command-usage-server-proof: <jogador> <servidor> <prova> <motivo> %usage%
command-usage-target-server-reason: <jogador> <servidor> <motivo> %usage%
command-usage-temp-proof: <jogador> <prova> <duração> <motivo> %usage%
command-usage-temp: <jogador> <duração> <motivo> %usage%
command-usage-proof: <jogador> <prova> <motivo> %usage%
command-usage-target-server: <jogador> <servidor> %usage%
command-usage-target: <jogador> %usage%
command-usage: <jogador> <motivo> %usage%

command-punishment-processing: '&aProcessando punição...'
command-punishment-proof: \\n&aDigite no chat uma prova para continuar!\\n&cDigite &ncancel&c para cancelar!\\n
command-punishment-confirm: \\n&7Você está prestes a punir &c%player%\\n&7Deseja confirmar esta punição?\\n{cancel} {confirm} {silent}\\n
command-punishment-cancel: '&aPunição cancelada.'

command-banning-concluded: '&aVocê baniu &f%player% &apor &f%reason% &acom sucesso em &f%server%&a!'
command-muting-concluded: '&aVocê silenciou &f%player% &apor &f%reason% &acom sucesso em &f%server%&a!'
command-kick-concluded: '&aVocê expulsou &f%player% &apor &f%reason% &acom sucesso em &f%server%&7!'
command-warn-concluded: '&aVocê alertou &f%player%&a por &f%reason% &acom sucesso! (%current%/%max%)'
command-warn-punished: '&aO jogador &f%player% &aexcedeu o máximo de alertas e foi punido!'
command-pardonid-concluded: '&aA punição ''%id%'' foi revogada com sucesso!'
command-pardon-concluded: '&aPunição de &f%player% &arevogada com sucesso em &f%server%&a!'
command-pardon-concluded-2: '&aPunições de &f%player% &arevogadas com sucesso em &f%server%&a!'
command-punishedit-concluded: '&aInformação &f''%info%'' &ade &f#%id% &aalterada para &f''%result%'''
command-clearwarnings-concluded: '&aAlertas de &f%player% &aremovidos!'
command-clearhistoric-concluded: '&aHistórico de &f%player% &alimpo com sucesso!'

command-punishment-not-found: '&cA punição ''%id%'' não foi encontrada.'
command-punishment-failed: '&cNão foi possível efetuar esta punição.'
command-punishment-failed-2: '&cO jogador &f%player%&c já está punido com &f%type% &cem &f%server%&c.'
command-something-is-missing: '&cAlguma informação está faltando.'
command-requires-server: '&cÉ necessário inserir um servidor.'
command-requires-reason: '&cÉ necessário inserir um motivo.'
command-requires-proof: '&cÉ necessário inserir uma prova.'
command-requires-proof-link: '&cÉ necessário que a prova comece com um destes endereços: &f%prooflinks%&c.'
command-requires-duration: '&cÉ necessário inserir uma duração.'
command-requires-duration-examples: '&cUtilize um destes formatos: &f1min, 1h, 1d, 1m, 1a&c.'
command-no-permission-target: '&cVocê não pode punir este jogador.'
command-blocked-nick: '&cEste jogador está na lista de nomes que não podem ser punidos.'
command-target-is-you: '&cVocê não pode punir a si mesmo.'
command-group-hierarchy: '&cO cargo do jogador é superior ou igual ao seu.'
command-reason-not-found: '&cO motivo ''%reason%'' não foi encontrado.'
command-server-not-found: '&cUse &fGlobal &cpara punir em todos ou use um dos servidores: &f%servers%'
command-warn-failed: '&cNão foi possível efetuar este alerta.'
command-pardon-failed: '&cO jogador &f%player% &cnão possui punições em &f%server%&c.'
command-pardon-failed-2: '&cO jogador &f%player% &cnão possui &f%type% &cativo em &f%server%&c.'
command-punishedit-examples: '&cInformações que podem ser alteradas: &fmotivo, prova, expirar, servidor&c.'
command-clearwarnings-failed: '&cO jogador &f%player% &cnão possui alertas.'
command-clearhistoric-failed: '&cO jogador &f%player% &cnão possui um histórico de punições.'
command-historic-failed: '&cNão foi encontrada punições sofridas por este jogador.'
command-historic-author-failed: '&cNão foi encontrada punições feitas por este jogador.'
command-punish-creating-input: '&7Você pode cancelar escrevendo &fcancel&7!'
command-punish-creating-type: '&cÉ necessário selecionar o tipo de punição.'
command-punish-creating-proof: '&cEscreva no chat para inserir a prova.\n&cÉ necessário que a prova comece com um destes endereços: &f%prooflinks%&c.'
command-punish-creating-reason: '&cEscreva no chat para inserir o motivo ou selecione.'
command-punish-creating-server: '&cEscreva no chat para selecionar o servidor.\n&cUse &fGlobal &cpara punir em todos ou use um dos servidores: &f%servers%'
command-punish-creating-duration: '&cEscreva no chat para definir a duração.\n&cUtilize um destes formatos: &f1s, 1min, 1h, 1d, 1m, 1a&c.'

ban-server-action-cancel: '&cVocê não pode fazer isto.'
ban-server-command-cancel: '&cVocê não pode utilizar este comando.'

warns:
pardon:
- '&aSua punição foi revogada!'
- ''
- '&aPunição: &f%type%'
- '&aPunido em: &f%date%'
- ''
- '&aApós uma analise, decidimos remove-la'
- '&aNossa equipe pede desculpas por &nqualquer incomodo'
- ''
expired:
- '&aSua punição expirou!'
- ''
- '&aPunição: &f%type%'
- '&aPunido em: &f%date%'
- ''
- '&aNossa equipe pede desculpas por &nqualquer incomodo'
- ''
warn:
- ''
- '&cVocê foi alertado!'
- ''
- '&cMotivo: &f%reason%'
- '&cAutor: &f%author%'
- '&cChances: &f%current%/%max%'
- ''
- '&cCaso ultrapasse o limite, você será punido'
- ''
mute:
- ''
- '&cVocê está silenciado permanentemente!'
- ''
- '&cMotivo: &f%reason%'
- '&cAutor: &f%author%'
- '&cEvidência: &f%proof%'
- ''
- '&cPunido injustamente? Contate-nos em'
- '&c&nleafplugins.com'
- ''
tempmute:
- ''
- '&cVocê está silenciado temporariamente!'
- ''
- '&cMotivo: &f%reason%'
- '&cAutor: &f%author%'
- '&cEvidência: &f%proof%'
- '&cExpira em: &f%expires%'
- ''
- '&cPunido injustamente? Contate-nos em'
- '&c&nleafplugins.com'
- ''

broadcasts:
status:
- ''
- ' &4[PUNIÇOES DO SERVIDOR]'
- ' &fEm nosso servidor, &c&l%total%&f punições já foram registradas.'
- ' &fCerca de &c&l%bans% &fbanimentos e &c&l%mutes%&f mutes em %hours% horas!'
- ' &cContinue denunciando jogadores infratores para auxiliar nossa equipe.'
- ''
# Placeholders disponíveis:
# %total% - total de punições
# %total_period% - total de punições no período
# %bans% - banimentos no período
# %mutes% - silenciamentos no período
# %hours% - horas definidas no periodo
prevented:
- ''
- §c(!) O jogador &f%player% &ctentou entrar estando banido.
- ''
warn:
- ''
- '&c(!) O jogador &f%player% &cfoi alertado.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Chances: %current%/%max%'
- ''
kick:
- ''
- '&c(!) O jogador &f%player% &cfoi desconectado.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- ''
mute:
- ''
- '&c(!) O jogador &f%player% &cfoi silenciado permanentemente.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Servidor: &f%server%'
- ''
tempmute:
- ''
- '&c(!) O jogador &f%player% &cfoi silenciado temporariamente.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Expira em: &f%expires%'
- '&c(!) Servidor: &f%server%'
- ''
ban:
- ''
- '&c(!) O jogador &f%player% &cfoi banido permanentemente.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Evidência: &f%proof%'
- '&c(!) Servidor: &f%server%'
- ''
tempban:
- ''
- '&c(!) O jogador &f%player% &cfoi banido temporariamente.'
- '&c(!) Motivo: &f%reason%'
- '&c(!) Autor: &f%author%'
- '&c(!) Evidência: &f%proof%'
- '&c(!) Expira em: &f%expires%'
- '&c(!) Servidor: &f%server%'
- ''
pardon:
- ''
- '&c(!) O jogador &f%player% &cteve sua punição revogada.'
- '&c(!) Punição: &f%type%'
- '&c(!) Autor: &f%author%'
- '&c(!) Servidor: &f%server%'
- ''

disconnects:
kick:
- '&cVocê foi desconectado: &f%reason%'
ban:
- '&cVocê foi banido permanentemente.'
- '&cMotivo: &f%reason%'
- '&cEvidência: &f%proof%'
- '&cID da punição: &f#%id%'
- ''
- '&7Adquira seu unban em: &bwww.leafplugins.com'
- '&cBanido injustamente? Contate-nos via'
- '&cwww.leafplugins.com/appeal'
tempban:
- '&cVocê foi banido temporariamente.'
- '&cMotivo: &f%reason%'
- '&cEvidência: &f%proof%'
- '&cID da punição: &f#%id%'
- ''
- '&cExpira em: &f%expires%'
- ''
- '&7Adquira seu unban em: &bwww.leafplugins.com'
- '&cBanido injustamente? Contate-nos via'
- '&cwww.leafplugins.com/appeal'
</code-block>
        </chapter>
        </chapter>
        <chapter title="menus/" collapsible="true">
            <chapter title="historic-menu.yml" collapsible="true">
<code-block lang="yaml">
# Menu principal
main-menu:
  title: "Histórico de punições"
  slots: 27
  # Sinta-se a vontade para por novos itens
  # apenas respeite os ids padrões para o funcionamento correto
  items:
    punishments:
      name: "&bPunições Sofridas"
      item: "head:afd2400002ad9fbbbd0066941eb5b1a384ab9b0e48a178ee96e4d129a5208654"
      slot: 11
      lore:
        - "&7Confira as punições"
        - "&7que este jogador sofreu"
        - ""
        - "&7Punições &aAtivas&7 e &cInativas"
        - ""
        - "&eClique para conferir"
      # Fechará o inventário caso clique
      closeInventory: false
      # Lista de comandos que o jogador executará
      execute: [ ]
    punishments-author:
      name: "&bPunições Aplicadas"
      item: "head:7a9566056da48a8b845e874f010f38a21089b914bf8eeb7f4e6d5e7f01c052ff"
      slot: 12
      lore:
        - "&7Confira as punições"
        - "&7que este jogador aplicou"
        - ""
        - "&eClique para conferir"
      # Fechará o inventário caso clique
      closeInventory: false
      # Lista de comandos que o jogador executará
      execute: [ ]
    head:
      name: "&b%target%"
      item: "head:%target%"
      slot: 15
      lore:
        - ""
        - "&7 Você está visualizando o histórico"
        - "&7 deste &fjogador"
        - ""
      # Fechará o inventário caso clique
      closeInventory: false
      # Lista de comandos que o jogador executará
      execute: [ ]

# Menu de listagem das punições
punishments-menus:
# Sinta-se a vontade para por novos itens
# apenas respeite os ids padrões para o funcionamento correto

punishments:
title: "Punições Sofridas"
slots: 54

    # Listagem das punições
    list:
      # Slots que os itens ocuparão
      slots: [ 10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 28, 29, 30, 31, 32, 33 ]

      # Formato dos itens de punição
      format:
        name: "%status_color%%type%"
        item: "writable_book"
        lore:
          - "&7ID: &f#%id%"
          - "&7Status: %status_colored%"
          - "&7Servidor: &f%server%"
          - ""
          - "&7Data: &f%date%"
          - "&7Término: &f%expiresdate%"
          - ""
          - "&7Autor: &f%author%"
          - "&7Motivo: &f%reason%"
          - "&7Prova: &f%proof%"

    items:
      type:
        name: "&bTipo de punição"
        item: "paper"
        slot: 47
        lore:
          - ""
          - "&7 Atual: &a%type%"
          - " &8Todos, banimentos e silenciamentos"
          - ""
          - "&eClique para alternar"

      order:
        name: "&bOrdem"
        item: "clock"
        slot: 48
        lore:
          - ""
          - "&7 Atual: &a%order%"
          - " &8Recente, mais antigo"
          - ""
          - "&eClique para alternar"

      status:
        name: "&bStatus de punição"
        item: "nether_star"
        slot: 49
        lore:
          - ""
          - "&7 Atual: &a%status%"
          - " &8Todos, ativos e inativos"
          - ""
          - "&eClique para alternar"

      return:
        name: "&b%target%"
        item: "head:%target%"
        slot: 51
        lore:
          - ""
          - "&7 Você está visualizando punições"
          - "&7 sofridas por este &fjogador"
          - ""
          - "&eClique para voltar"
        # Fechará o inventário caso clique
        closeInventory: false
        # Lista de comandos que o jogador executará
        execute: [ ]

      glass1:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 46
        lore: [ ]

      glass2:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 45
        lore: [ ]

      glass3:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 50
        lore: [ ]

      glass4:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 52
        lore: [ ]

      glass5:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 53
        lore: [ ]

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

punishments-author:
title: "Punições Aplicadas"
slots: 54
# Listagem das punições
list:
# Slots que os itens ocuparão
slots: [ 10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 28, 29, 30, 31, 32, 33 ]

      # Formato dos itens de punição
      format:
        name: "%status_color%%type%"
        item: "writable_book"
        lore:
          - "&7ID: &f#%id%"
          - "&7Status: %status_colored%"
          - "&7Servidor: &f%server%"
          - ""
          - "&7Jogador: &f%player%"
          - ""
          - "&7Data: &f%date%"
          - "&7Término: &f%expiresdate%"
          - ""
          - "&7Motivo: &f%reason%"
          - "&7Prova: &f%proof%"

    items:
      type:
        name: "&bTipo de punição"
        item: "paper"
        slot: 47
        lore:
          - ""
          - "&7 Atual: &a%type%"
          - " &8Todos, banimentos e silenciamentos"
          - ""
          - "&eClique para alternar"

      order:
        name: "&bOrdem"
        item: "clock"
        slot: 48
        lore:
          - ""
          - "&7 Atual: &a%order%"
          - " &8Recente, mais antigo"
          - ""
          - "&eClique para alternar"

      status:
        name: "&bStatus de punição"
        item: "nether_star"
        slot: 49
        lore:
          - ""
          - "&7 Atual: &a%status%"
          - " &8Todos, ativos e inativos"
          - ""
          - "&eClique para alternar"

      return:
        name: "&b%target%"
        item: "head:%target%"
        slot: 51
        lore:
          - ""
          - "&7 Você está visualizando punições"
          - "&7 sofridas por este &fjogador"
          - ""
          - "&eClique para voltar"
        # Fechará o inventário caso clique
        closeInventory: false
        # Lista de comandos que o jogador executará
        execute: [ ]

      glass1:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 46
        lore: [ ]

      glass2:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 45
        lore: [ ]

      glass3:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 50
        lore: [ ]

      glass4:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 52
        lore: [ ]

      glass5:
        name: "&7<->"
        item: "stained_glass_pane:7"
        slot: 53
        lore: [ ]

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
        <chapter title="punishments-menu.yml" collapsible="true">
<code-block lang="yaml">
# Menu principal
main-menu:
  title: "Punições"
  slots: 27
  # Sinta-se a vontade para por novos itens
  # apenas respeite os ids padrões para o funcionamento correto
  items:
    punishments:
      name: "&bTodas as Punições"
      item: "head:afd2400002ad9fbbbd0066941eb5b1a384ab9b0e48a178ee96e4d129a5208654"
      slot: 11
      lore:
        - "&7Confira as punições"
        - "&7que foram feitas no servidor"
        - ""
        - "&eClique para conferir"
      # Fechará o inventário caso clique
      closeInventory: false
      # Lista de comandos que o jogador executará
      execute: [ ]

    players:
      name: "&bPlayers Punidos"
      item: "head:player"
      slot: 12
      lore:
        - "&7Confira os jogadores"
        - "&7que foram e estão punidos"
        - ""
        - "&eClique para conferir"
      # Fechará o inventário caso clique
      closeInventory: false
      # Lista de comandos que o jogador executará
      execute: [ ]

    book:
      name: "&bPunições"
      item: "book"
      slot: 15
      lore:
        - ""
        - "&7 Você está visualizando"
        - "&7 as punições do &fservidor"
        - ""
      # Fechará o inventário caso clique
      closeInventory: false
      # Lista de comandos que o jogador executará
      execute: [ ]

# Menu de listagem de players
players-menu:
title: "Players Punidos"
slots: 54
# Listagem dos players
list:
# Slots que os itens ocuparão
slots: [ 10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 28, 29, 30, 31, 32, 33 ]

    # Formato dos itens de player
    format:
      name: "%color%%target%"
      item: "head:%target%"
      lore-active:
        - ""
        - "&7 Possui punições &aativa(s)"
        - ""
        - "&eClique para conferir"
      lore-inactive:
        - ""
        - "&7 Possui punições &cinativa(s)"
        - ""
        - "&eClique para conferir"

items:
status:
name: "&bStatus"
item: "nether_star"
slot: 48
lore:
- ""
- "&7 Atual: &a%status%"
- " &8Todos, ativos e inativos"
- ""
- "&eClique para alternar"
# Fechará o inventário caso clique
closeInventory: false
# Lista de comandos que o jogador executará
execute: [ ]

    return:
      name: "&bVoltar"
      item: "book"
      slot: 50
      lore:
        - ""
        - "&7 Você está visualizando jogadores"
        - "&7 que foram ou estão punidos"
        - ""
        - "&eClique para voltar"
      # Fechará o inventário caso clique
      closeInventory: false
      # Lista de comandos que o jogador executará
      execute: [ ]

    glass1:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 45
      lore: [ ]

    glass2:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 46
      lore: [ ]

    glass3:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 47
      lore: [ ]

    glass4:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 49
      lore: [ ]

    glass5:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 51
      lore: [ ]

    glass6:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 52
      lore: [ ]

    glass7:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 53
      lore: [ ]

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

# Menu de listagem das punições
punishments-menu:
title: "Punições"
slots: 54
# Listagem dos players
list:
# Slots que os itens ocuparão
slots: [ 10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 28, 29, 30, 31, 32, 33 ]

    # Formato dos itens de punição
    format:
      name: "%status_color%Punição de %player%"
      item: "head:%player%"
      lore:
        - "&8%type%"
        - ""
        - "&7ID: &f#%id%"
        - "&7Status: %status_colored%"
        - "&7Servidor: &f%server%"
        - ""
        - "&7Jogador: &f%player%"
        - ""
        - "&7Data: &f%date%"
        - "&7Término: &f%expiresdate%"
        - ""
        - "&7Autor: &f%author%"
        - "&7Motivo: &f%reason%"
        - "&7Prova: &f%proof%"

items:
type:
name: "&bTipo de punição"
item: "paper"
slot: 47
lore:
- ""
- "&7 Atual: &a%type%"
- " &8Todos, banimentos e silenciamentos"
- ""
- "&eClique para alternar"

    order:
      name: "&bOrdem"
      item: "clock"
      slot: 48
      lore:
        - ""
        - "&7 Atual: &a%order%"
        - " &8Recente, mais antigo"
        - ""
        - "&eClique para alternar"

    status:
      name: "&bStatus de punição"
      item: "nether_star"
      slot: 49
      lore:
        - ""
        - "&7 Atual: &a%status%"
        - " &8Todos, ativos e inativos"
        - ""
        - "&eClique para alternar"

    return:
      name: "&bVoltar"
      item: "book"
      slot: 50
      lore:
        - ""
        - "&7 Você está visualizando"
        - "&7 as punições registradas"
        - ""
        - "&eClique para voltar"
      # Fechará o inventário caso clique
      closeInventory: false
      # Lista de comandos que o jogador executará
      execute: [ ]

    glass1:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 45
      lore: [ ]

    glass2:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 46
      lore: [ ]

    glass3:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 47
      lore: [ ]

    glass4:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 49
      lore: [ ]

    glass5:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 51
      lore: [ ]

    glass6:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 52
      lore: [ ]

    glass7:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 53
      lore: [ ]

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
        <chapter title="punishment-menu.yml" collapsible="true">
<code-block lang="yaml">
# Menu principal
main-menu:
  title: "Nova punição"
  slots: 5
  # Sinta-se a vontade para por novos itens
  # apenas respeite os ids padrões para o funcionamento correto
  items:
    # Itens extras
    target:
      name: "&aPunindo \"%target%\""
      item: "head:%target%"
      slot: 19
      lore:
        - ""
        - " &7Você está punindo o jogador"
        - ""
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute: [ ]

    reasons:
      name: "&aPunições pré-definidas"
      item: "comparator"
      slot: 21
      lore:
        - ""
        - " &7Use punições pré-definidas"
        - " &8(Punição rápida)"
        - ""
        - "&eClique para continuar"

    create:
      name: "&aCriar punição"
      item: "writable_book"
      slot: 22
      lore:
        - ""
        - " &7Criar uma punição customizada"
        - " &8(Punição avançada)"
        - ""
        - "&eClique para continuar"

    historic:
      name: "&aHistórico"
      item: "head:43aff57724f5ed04db450db874c6c0c6ef4a10e1406b77fbaffdcb98191bf204"
      slot: 24
      lore:
        - ""
        - " &7Consultar o histórico"
        - " &7de punições do jogador"
        - " &8(Punições feitas e sofridas)"
        - ""
        - "&eClique para continuar"
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará
      execute:
        - "/historic %target%"

    userinfo:
      name: "&aInformações"
      item: "head:8a6d2f471b54047148b355255c7f556e2187fd4e8338b111dbf3adcd2850c498"
      slot: 25
      lore:
        - ""
        - " &7Consultar informações"
        - " &7armazenadas do jogador"
        - " &8(IP, contas alternativas e mais)"
        - ""
        - "&eClique para continuar"
      # Fechará o inventário caso clique
      closeInventory: false

      # Lista de comandos que o jogador executará (use / no inicio)
      execute:
        - "/userinfo %target%"

    glassheader1:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 0
      lore: [ ]

    glassheader2:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 1
      lore: [ ]

    glassheader3:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 2
      lore: [ ]

    glassheader4:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 3
      lore: [ ]

    glassheader5:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 4
      lore: [ ]

    glassheader6:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 5
      lore: [ ]

    glassheader7:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 6
      lore: [ ]

    glassheader8:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 7
      lore: [ ]

    glassheader9:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 8
      lore: [ ]

    glass1:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 36
      lore: [ ]

    glass2:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 37
      lore: [ ]

    glass3:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 38
      lore: [ ]

    glass4:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 39
      lore: [ ]

    glass5:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 40
      lore: [ ]

    glass6:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 41
      lore: [ ]

    glass7:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 42
      lore: [ ]

    glass8:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 43
      lore: [ ]

    glass9:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 44
      lore: [ ]

# Menu de pré-definidos
reasons-menu:
title: "Motivos pré-definidos"
slots: 54
# Listagem dos players
list:
# Slots que os itens ocuparão
slots: [ 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34 ]

    requires-proof:
      true: "§aSim"
      false: "§7Não"
    # Formato dos itens de player
    format:
      name: "&amp;b%reason%"
      item: "%icon%"
      lore:
        - ''
        - ' &amp;fTipo: &amp;a%type%'
        - ' &amp;fDuração: &amp;a&lt;when="not-temporary"&gt;%duration%&lt;/when="Permanente"&gt;'
        - ' &amp;fProva obrigatoria: &amp;7%requires%'
        - ''
        - '&amp;eClique para selecionar'

items:
glassheader1:
name: "&amp;7&lt;-&gt;"
item: "stained_glass_pane:7"
slot: 0
lore: [ ]

    glassheader2:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 1
      lore: [ ]

    glassheader3:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 2
      lore: [ ]

    glassheader4:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 3
      lore: [ ]

    glassheader5:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 4
      lore: [ ]

    glassheader6:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 5
      lore: [ ]

    glassheader7:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 6
      lore: [ ]

    glassheader8:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 7
      lore: [ ]

    glassheader9:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 8
      lore: [ ]

    glass1:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 45
      lore: [ ]

    glass2:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 46
      lore: [ ]

    glass3:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 47
      lore: [ ]

    glass4:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 48
      lore: [ ]

    glass5:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 49
      lore: [ ]

    glass6:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 50
      lore: [ ]

    glass7:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 51
      lore: [ ]

    glass8:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 52
      lore: [ ]

    glass9:
      name: "&amp;7&lt;-&gt;"
      item: "stained_glass_pane:7"
      slot: 53
      lore: [ ]

    type:
      name: "&amp;bTipo de punição"
      item: "paper"
      slot: 48
      lore:
        - ""
        - "&amp;7 Atual: &amp;a%type%"
        - ""
        - "&amp;eClique para alternar"

    return:
      name: "&amp;bPunindo \"%target%\""
      item: "head:%target%"
      slot: 50
      lore:
        - ""
        - "&amp;7 Você está punindo"
        - "&amp;7 este jogador"
        - ""
        - "&amp;eClique para voltar"

    previous-page:
      name: "&amp;7Pág. anterior &amp;7(&amp;b%previouspage%&amp;7/&amp;b%maxpages%&amp;7)"
      item: "arrow"
      slot: 45
      lore:
        - ""
        - " &amp;7Ir para &amp;fpágina anterior"
        - ""

    next-page:
      name: "&amp;7Próx. página &amp;7(&amp;b%page%&amp;7/&amp;b%maxpages%&amp;7)"
      item: "arrow"
      slot: 53
      lore:
        - ""
        - " &amp;7Ir para &amp;fpróxima página"
        - ""
# Menu de pré-definidos
create-menu:
title: "Criando punição"
slots: 54
items:
glassheader1:
name: "&7<->"
item: "stained_glass_pane:7"
slot: 0
lore: [ ]

    glassheader2:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 1
      lore: [ ]

    glassheader3:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 2
      lore: [ ]

    glassheader4:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 3
      lore: [ ]

    glassheader5:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 4
      lore: [ ]

    glassheader6:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 5
      lore: [ ]

    glassheader7:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 6
      lore: [ ]

    glassheader8:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 7
      lore: [ ]

    glassheader9:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 8
      lore: [ ]

    glass1:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 45
      lore: [ ]

    glass2:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 46
      lore: [ ]

    glass3:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 47
      lore: [ ]

    glass4:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 48
      lore: [ ]

    glass5:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 49
      lore: [ ]

    glass6:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 50
      lore: [ ]

    glass7:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 51
      lore: [ ]

    glass8:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 52
      lore: [ ]

    glass9:
      name: "&7<->"
      item: "stained_glass_pane:7"
      slot: 53
      lore: [ ]

    server:
      name: 'Selecionar servidor'
      item: "head:438cf3f8e54afc3b3f91d20a49f324dca1486007fe545399055524c17941f4dc"
      slot: 20
      lore:
        - ""
        - " &7Servidor da punição"
        - " &8Padrão: &fGlobal"
        - ""
        - "&eClique para alterar"

    type:
      name: 'Selecionar punição'
      item: "beacon"
      slot: 22
      lore:
        - ""
        - " &7Tipo de punição"
        - ""
        - "&eClique para alterar"

    silent:
      name: '%color%Silent'
      item: "%is-selected%"
      slot: 24
      lore:
        - ""
        - " &7Punir sem anunciar"
        - ""
        - "&eClique para alterar"

    duration:
      name: 'Selecionar duração'
      item: "head:af8cdb9f4ca3a26d638b7c93dd30bd8461e0a3d65e85c4607ff3d4fc244df3b7"
      slot: 29
      lore:
        - ""
        - " &7Duração da punição"
        - ""
        - "&eClique para alterar"

    reason:
      name: 'Selecionar motivo'
      item: "head:7e2eb4751e3c50d50ff16352576663d8fedfe3e04b2f0b8a2aa803b419363ca1"
      slot: 31
      lore:
        - ""
        - " &7Motivo da punição"
        - ""
        - "&eClique para alterar"

    proof:
      name: 'Inserir prova'
      item: "head:924e825b25ff7938b58af52f58e4d54ec5143bd5a1b484f1ff9dd6ba0aca9dcb"
      slot: 33
      lore:
        - ""
        - " &7Prova da punição"
        - ""
        - "&eClique para alterar"

    confirm:
      name: '&aConfirmar punição'
      item: "ink_sac:10"
      slot: 48
      lore:
        - ""
        - " &7Confirmar e punir o jogador"
        - ""
        - "&eClique para confirmar"

    return:
      name: "&bPunindo \"%target%\""
      item: "head:%target%"
      slot: 50
      lore:
        - ""
        - "&7 Você está punindo"
        - "&7 este jogador"
        - ""
        - "&eClique para voltar"
</code-block>
        </chapter>
        </chapter>
        <chapter title="settings/" collapsible="true">
            <chapter title="commands.yml" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração
warn:
  name: warn
  use-command: true
  aliases:
    - alertar
    - avisar
  usage: para alertar um jogador.

punish:
name: punish
use-command: true
aliases:
- punir
usage: <motivo> para punir um jogador.

ban:
name: ban
use-command: true
aliases:
- banir
usage: para banir um jogador.

kick:
name: kick
use-command: true
aliases:
- expulsar
usage: para expulsar um jogador.

mute:
name: mute
use-command: true
aliases:
- silenciar
usage: para silenciar um jogador.

ipban:
name: ipban
use-command: true
aliases:
- banir-ip
- ban-ip
- ip-ban
usage: para banir o endereço-ip de um jogador.

tempban:
name: tempban
use-command: true
aliases:
- temp-ban
- ban-temp
usage: para banir temporariamente um jogador.

tempipban:
name: tempipban
use-command: true
aliases:
- temp-ipban
- ipban-temp
- temp-ip-ban
usage: para banir temporariamente o endereço-ip de um jogador.

tempmute:
name: tempmute
use-command: true
aliases:
- temp-mute
- mute-temp
usage: para silenciar temporariamente um jogador.

pardon:
name: pardon
use-command: true
aliases:
- perdoar
- revogar
usage: para revogar todas as punições de um jogador.

pardonid:
name: pardonid
use-command: true
aliases:
- perdoar-id
usage: para revogar uma punição pelo id.

unban:
name: unban
use-command: true
aliases:
- desbanir
usage: para revogar o banimento um jogador.

unmute:
name: unmute
use-command: true
aliases: []
usage: para revogar o silenciamento de um jogador.

punishments:
name: punishments
use-command: true
aliases:
- punicoes
- banlist
usage: para ver as punições do servidor.

historic:
name: historic
use-command: true
aliases:
- historico
usage: para ver o histórico de um jogador.

clearhistoric:
name: clearhistoric
use-command: true
aliases:
- clearhc
usage: para limpar o histórico de um jogador.

clearwarnings:
name: clearwarnings
use-command: true
aliases:
- clearwarns
usage: para retirar os alertas de um jogador.

punishedit:
name: punishedit
use-command: true
aliases:
- editar-punicao
usage: para editar uma punição.

punishinfo:
name: punishinfo
use-command: true
aliases:
- ver-punicao
- punish-info
usage: para ver as informações de uma punição.

checkplayer:
name: checkplayer
use-command: true
aliases:
- checkban
- checkmute
- checkpunish
- checarpunicao
- checarjogador
usage: para checar um jogador.
</code-block>
            </chapter>
            <chapter title="discord.yml" collapsible="true">
<code-block lang="yaml">
# Insira a Webhook Geral do canal que irá enviar as embeds
# Caso as embeds não hajam "webhook" individuais, serão usadas esta:
webhookURL: "https://discordapp.com/api/webhooks/1360889371812823051/n0hJ7vOPZ-BDWIki4JL1eFxDx-vDcilE0mXRhJL9ErIJIbNzzO7sREebwKl1PHQwKB3g"

# Observação: É necessário ter baixado o LeafDiscord em seu servidor

embeds:
# Placeholders disponíveis:
# %player% - nome do jogador
# %uuid% - uuid do jogador
# %player_icon% - URL do icone do jogador
# %author_icon% - URL do icone do autor
#
# %id% - id da punição
# %author% - nome do autor
# %type% - tipo de punição
# %reason% - motivo da punição
# %server% - servidor da punição
# %proof% - prova da punição
# %date% - data da punição
# %expires% - tempo até expirar
# %expiresDate% - data de expiração
# %expiresTimeStamp% - timestamp de expiração
punishment:
enable: true
webhook: ""
title: "%player% foi punido!"
color: "#ff0000"
thumbnailURL: "%player_icon%"
description: "Na próxima vez leia as regras!"
field-inline: true
fields:
# O que vier antes do -> será o nome da field
# O que vier após o -> será o texto da field
- "ID -> #%id%"
- "Punição -> %type%"
- "Motivo -> %reason%"
- "Servidor -> %server%"
- "Prova -> %proof%"
- "Quem puniu -> %author%"
footer: "UUID do usuário: %uuid%"
footerURL: "%player_icon%"

# [Premium]
pardon:
enable: true
webhook: ""
title: "%player% foi perdoado!"
color: ""
thumbnailURL: "%player_icon%"
description: ""
field-inline: true
fields:
- "ID -> #%id%"
- "Punição -> %type%"
- "Motivo -> %reason%"
- "Quem revogou -> %author%"
footer: "UUID do usuário: %uuid%"
footerURL: "%player_icon%"

# [Premium]
warn:
enable: true
webhook: ""
title: "%player% foi alertado!"
color: ""
thumbnailURL: "%player_icon%"
description: ""
field-inline: true
fields:
- "Motivo -> %reason%"
- "Quem alertou -> %author%"
footer: "UUID do usuário: %uuid%"
footerURL: "%player_icon%"

# [Premium]
prevented:
enable: true
webhook: ""
title: "%player% foi barrado!"
color: "#ff0000"
thumbnailURL: "%player_icon%"
description: "%player% tentou entrar estando banido."
field-inline: true
fields:
- "Punição -> %type%"
footer: "UUID do usuário: %uuid%"
footerURL: "%player_icon%"
</code-block>
            </chapter>
            <chapter title="punishments.yml" collapsible="true">
<code-block lang="yaml">
warn:
  # Nome do tipo de punição
  name: "Aviso"
  # Permitirá que este tipo de punição seja anunciado
  broadcasts:
    # Anunciar no servidor
    server: true
    # Anunciar no discord
    discord: true

kick:
name: "Expulsão"
# Permitirá que este tipo de punição seja anunciado
broadcasts:
# Anunciar no servidor
server: true
# Anunciar no discord
discord: true

ban:
name: "Banimento"
# Permitirá que este tipo de punição seja anunciado
broadcasts:
# Anunciar no servidor
server: true
# Anunciar no discord
discord: true

ipban:
name: "Banimento por IP"
# Permitirá que este tipo de punição seja anunciado
broadcasts:
# Anunciar no servidor
server: true
# Anunciar no discord
discord: true

tempban:
name: "Banimento temporário"
# Permitirá que este tipo de punição seja anunciado
broadcasts:
# Anunciar no servidor
server: true
# Anunciar no discord
discord: true

tempipban:
name: "Banimento por IP temporário"
# Permitirá que este tipo de punição seja anunciado
broadcasts:
# Anunciar no servidor
server: true
# Anunciar no discord
discord: true

mute:
name: "Silenciamento"
# Permitirá que este tipo de punição seja anunciado
broadcasts:
# Anunciar no servidor
server: true
# Anunciar no discord
discord: true

tempmute:
name: "Silenciamento temporário"
# Permitirá que este tipo de punição seja anunciado
broadcasts:
# Anunciar no servidor
server: true
# Anunciar no discord
discord: true
</code-block>
            </chapter>
            <chapter title="reasons.yml" collapsible="true">
<code-block lang="yaml">
Hack:
  name: "Uso de Hack"
  aliases: [ "cheating", "trapaças", "trapaça", "cheat" ]
  # Caso queira utilizar uma head customizada, utilize: 'head:codigo'
  icon: "ink_sac:1"

# Tipo de punição que será aplicada (Caso o progress não esteja sendo usado)
# tipos: <ipban, ban, mute, kick> (Caso haja duração definida, automaticamente será temp(tipo)[tempban,etc...])
type: Ban

# Permissão necessária para aplicar esta punição
permission: "leafpunish.command.ban"

# Fará que seja obrigatório inserir uma prova
requires-proof: true

# A duração até o término desta punição
# Deixe vazio para que seja permanente ou caso a punição não haja versão temporária
# formato: <1min, 1h, 1d, 1m, 1a>
duration: ""

# [Premium]
# Faça com esta punição seja progressiva (Desative deixando a lista vazia)
# Exemplo: 1x sendo punido será banido temporariamente por 30 dias,
# a partir da segunda será ipban permanente
progress:
- "ban 60d"
- "ipban"

Divulgacao-grave:
name: "Divulgação Grave"
aliases: [ "divugrave" ]
icon: "ink_sac:1"
type: Ban
permission: "leafpunish.command.ban"
requires-proof: true
duration: ""
progress:
- "mute 10d"
- "ban"

Bug:
name: "Abuso de bugs"
aliases: [ "bugs" ]
icon: "ink_sac:1"
type: IpBan
permission: "leafpunish.command.ipban"
requires-proof: true
duration: ""
progress:
- "ban 30d"
- "ipban"

Comercio:
name: "Comércio não autorizado"
aliases: [ ]
icon: "ink_sac:1"
type: Ban
permission: "leafpunish.command.tempban"
requires-proof: true
duration: "7d"
progress:
- "ban 7d"
- "ban"

Comportamento-toxico:
name: "Comportamento Tóxico"
aliases: [ ]
icon: "ink_sac:1"
type: Ban
permission: "leafpunish.command.tempban"
requires-proof: true
duration: "2d"
progress:
- "ban 2d"
- "ban 10d"
- "ban 30d"
- "ban"

Ofensa-ao-servidor:
name: "Ofensa ao servidor/staff"
aliases: [ ]
icon: "ink_sac:1"
type: Ban
permission: "leafpunish.command.tempban"
requires-proof: true
duration: "2d"
progress:
- "ban 1d"
- "ban"

Anti-jogo:
name: "Anti-Jogo"
aliases: [ ]
icon: "ink_sac:1"
type: Ban
permission: "leafpunish.command.tempban"
requires-proof: true
duration: "1d"
progress: [ ]

# Punições de silenciamento
Flood-grave:
name: "Spam/Flood Grave"
aliases: [ ]
icon: "ink_sac:1"
type: Mute
permission: "leafpunish.command.mute"
requires-proof: false
duration: ""
progress:
- "mute 10h"
- "mute"

Flood:
name: "Spam/Flood"
aliases: [ ]
icon: "ink_sac:1"
type: Mute
permission: "leafpunish.command.tempmute"
requires-proof: false
duration: "1h"
progress:
- "mute 1h"
- "mute 5h"
- "mute 10h"

Ofensa-a-jogadores:
name: "Ofensa a jogadores"
aliases: [ ]
icon: "ink_sac:1"
type: Mute
permission: "leafpunish.command.tempban"
requires-proof: true
duration: "12h"
progress:
- "mute 12h"
- "mute 1d"

Divulgacao:
name: "Divulgação"
aliases: [ ]
icon: "ink_sac:1"
type: Mute
permission: "leafpunish.command.tempmute"
requires-proof: false
duration: "5h"
progress:
- "mute 5h"
- "mute 10h"
- "mute"

Ofensas:
name: "Ofensas no bate-papo"
aliases: [ ]
icon: "ink_sac:1"
type: Mute
permission: "leafpunish.command.mute"
requires-proof: false
duration: "3d"
progress:
- "mute 1h"
- "mute 10h"
- "mute 3d"
</code-block>
            </chapter>
        </chapter>
        <chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
# Agradecemos por escolher o LeafPunish ♥
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

# Ativará o filtro Log4j para desativar logs de desconnects (Necessário reiniciar)
log-filter: false

# Ative esse modo caso o servidor seja o servidor de bans
# Isso desabilitará todas as interações do servidor
ban-server: false

# Lista de nicknames que não poderão ser punidos
blocked-nicks:
- nome-aqui

# Comandos que não poderão ser usados quando estiver silenciado
blocked-mute-commands:
- /g
- /l
- /r
- /tell

# Hierarquia dos cargos (Deixe vazio para desativar)
# Lembre-se de deixar exatamente como está em seu plugin de permissões
# Caso o cargo do jogador seja inferior ao alvo, a punição será cancelada
group-hierarchy:
- Master
- Admin
- Mod
- Helper
- default

# Fará que a prova precise começar com um destes endereços
# Caso a lista esteja vazia, não exigirá nenhum endereço específico
proof-domains:
- https://
- youtube.com
- prints.com

# Servidores BungeeCord permitidos para serem selecionados nas punições
allowed-servers:
- RankUP
- Lobby
- Survival
- HungerGames
- SkyWars

punishment:
# Caso a punição seja Global, esta será a mensagem
global: Todos

# Caso a punição não haja uma prova definida esta será a mensagem
no-proof: Nenhuma

# Caso a punição não haja um motivo definido esta será a mensagem
no-reason: Nenhum motivo

# Caso a punição seja feita pelo console, este será o nome do autor
console-name: Servidor

options:
# Nome do servidor que o jogador será punido
# Caso esteja "Global" as punições feitas neste servidor servirá para todos
# que utilizarem o mesmo banco de dados
server: Global

# Fará que o autor possa selecionar o servidor que o jogador vai ser punido
select-server: true

# Usará os anúncios de punições
broadcasts: true

# Quando o jogador for desconectado, será expulso do Proxy
disconnect-proxy: false

# Notificar o jogador quando entrar caso esteja punido
# Exemplo: Silenciamentos
notify-join: true

# O staffer poderá punir ele mesmo. (É recomendado que apenas ative para testar o plugin)
self-punish: true

# Fará que seja obrigatório inserir uma prova ao punir (fora do /punir)
# Caso esteja 'true', o motivo também será obrigatório
requires-proof: false

# Fará que seja obrigatório confirmar ao punir (/punir)
requires-confirm: true

# Fará que seja obrigatório inserir um motivo ao punir
requires-reason: true

# Caso a punição não haja uma evidência definida, a linha que possuir %proof% será pulada
# Exemplo: disconnects, warns e broadcasts
skip-proof-lines: true

# Fará que a punição silenciosa envie o webhook para o discord normalmente
# Para usar, é necessário que no motivo da punição termine com "-s"
# Exemplo: /ban Hacker Uso de Hack -s
silent-webhooks: true

# [Premium]
# Permitir que as punições tenham progresso (reasons.yml)
# Tipos disponíveis:
# ==> 0 (Desativar)
# ==> 1 (Funcionará apenas no /punir)
# ==> 2 (Funcionará em todas as punições [As que não são temporarias, exemplo: /tempmute])
progressive-punishments: 1

# Caso o jogador seja punido por IP, todas as contas
# que possuirem o mesmo IP serão banidas individualmente (Contas alternativas)
ban-alternate-accounts: true

# Opções do comando punir
punish:
# Abrirá o menu [Premium]
open-menu: true

# Mensagem em cima da lista
reasons-list-top: §eTipos de infrações disponíveis

# Mensagem em baixo da lista
reasons-list-footer: '&eClique no motivo desejado'

# Formato do motivo na lista
reason-format: '&b* &f%reason%'

# [Premium]
warn:
# Máximo de alertas até o jogador ser punido pelo motivo do aviso
# Deixe 0 para desativar esta função
max-warns: 3

# Duração para que a warn seja expirada
# formato: <1min, 1h, 1d, 1m, 1a>
# Deixe vazio para que seja permanente
alert-duration: 1d

# Tipo de punição que será aplicada após exceder o máximo de avisos
type: Mute

# Tipos disponíveis:
# ==> Global (Punir em todos os servidores)
# ==> Current (Punir no servidor definido em options.server)
server: Global

# Duração da punição que será aplicada após exceder o máximo de avisos
# Deixe vazio para que seja permanente ou caso a punição não haja versão temporária
punishment-duration: 5h

# Broadcasts configuraveis no arquivo de mensagens
broadcasts:
# Define se as punições devem ser anunciadas apenas no servidor onde foram aplicadas
# Exemplo: um jogador foi banido no servidor "Survival", então o anúncio será feito somente lá
# Útil para evitar anúncios globais em toda a rede
announce-only-local: false

# [Premium]
status:
enable: true

    # Som que irá tocar quando o anúncio for feito (Deixe vazio para desativar)
    sound: WOOD_CLICK
    
    # Tempo em minutos para que o status seja anunciado
    delay: 30
    
    # Os periodos apenas funcionam em MySQL
    # Irá listar as punições que estiverem neste período
    # Exemplo: 0 = %bans% e %mutes% será a quantia total de punições
    # Exemplo: 24 = %bans% e %mutes% será a quantia de punições no período de 24 horas
    # Exemplo: 168 = %bans% e %mutes% será a quantia de punições no período de 7 dias (24x7)
    period: 24
    
    # Enviará este anúncio para o console
    console-log: false

staff:
# Permissão necessária para receber estes anúncios
permission: leafpunish.announce.staff

    # Anunciará caso um jogador tente entrar no servidor estando banido
    prevented: true
    
    # Avisará ao console caso um jogador tente entrar no servidor estando banido
    prevented-log: true
    
    # Mensagem que será enviada no console
    prevented-log-message: '&c(!) O jogador &f%player%[%address%] &ctentou entrar estando banido. (#%id%)'

punishments:
# Anunciará as punições de banimento
bans: true

    # Anunciará as punições de expulsão
    kicks: true
    
    # Anunciará as punições de silenciamento
    mutes: true
    
    # Anunciará os alertas
    warns: true
    
    # Anunciará as revogações
    pardons: true
    
    # Permissão necessária para receber estes anúncios
    permission: ''
    
    # Som que irá tocar quando algum dos anúncios for feito (Deixe vazio para desativar)
    sound: WOOD_CLICK
</code-block>
        </chapter>
</chapter>

