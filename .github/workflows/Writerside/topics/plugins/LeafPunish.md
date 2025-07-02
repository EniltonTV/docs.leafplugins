# LeafPunish
<secondary-label ref="gratuita"/>
<secondary-label ref="premium"/>

<p>Torne a gestão de seu servidor mais eficaz com um sistema de punições avançado.</p>

## Compatibilidades

<list>
    <li>
        <p>Leaf Discord - Anuncie punições aplicadas em seu servidor no discord;</p>
    </li>
    <li>
        <p>nChat/LegendChat - O jogador silenciado não poderá interagir em nenhum canal de texto;</p>
    </li>
    <li>
        <p>LuckPerms - Sistema de hierarquia(Usuários com permissão para aplicar punições não poderão aplicar punições sob cargos superiores ao que ele ocupa);</p>
    </li>
</list>

## Premium

Ao adquirir uma versão aprimorada de nossos serviços você estará apoiando nosso projeto e adquirindo vantagens
exclusivas.

<procedure title="Quais sãos as vantagens?">
    <list>
        <li>
            <p>BungeeCord - Aplique punições pelo servidor proxy;</p>
        </li>
        <li>
            <p>Anuncie quantas punições foram aplicadas durante um período(Customizável);</p>
        </li>
        <li>
            <p>Sistema de <code>/punir, /historic e /punishesments</code> em menu;</p>
        </li>
        <li>
            <p>Servidor de banimento(Direcione os jogadores para um servidor sempre que ele foram banidos)</p>
        </li>
        <li>
            <p>Punições progressivas(A cada punição sofrida pelo mesmo motivo maior será a penalidade);</p>
        </li>
    </list>
</procedure>

## Ultilitários

<tabs>
    <tab title="Placeholders">
        <procedure title="Placeholders">
            <p><control>PlaceholderAPI</control></p>
            <p>
                <code>%leafpunish_is_mute%</code> - Retornará true ou false caso o jogador esteja silenciado;<br>
                <code>%leafpunish_warns%</code> - Retornará a quantidade de warns atuais do jogador;
            </p>
        </procedure>
    </tab>
    <tab title="Permissões">
        <procedure title="Permissões">
            <p>Abaixo você pode visualizar as permissões disponíveis para este plugin.</p>
            <p>
                <code>leafpunish.command.historic</code> - /historic;<br>
                <code>leafpunish.command.punishments</code> - /punishments;<br>
                <code>leafpunish.command.clearhistoric</code> - /clearhistoric;<br>
                <code>leafpunish.command.clearwarns</code> - /clearwarnings;<br>
                <code>leafpunish.command.warn</code> - /warn;<br>
                <code>leafpunish.command.checkplayer</code> - /checkplayer;<br>
                <code>leafpunish.command.punishedit</code> - /punishedit;<br>
                <code>leafpunish.command.punishinfo</code> - /punishinfo;<br>
                <code>leafpunish.command.punish</code> - /punir;<br>
                <code>leafpunish.command.kick</code> - /kick;<br>
                <code>leafpunish.command.mute</code> - /mute;<br>
                <code>leafpunish.command.tempmute</code> - /tempmute;<br>
                <code>leafpunish.command.ban</code> - /ban;<br>
                <code>leafpunish.command.tempban</code> - /tempban;<br>
                <code>leafpunish.command.ipban</code> - /ipban;<br>
                <code>leafpunish.command.tempipban</code> - /tempipban;<br>
                <code>leafpunish.command.pardon</code> - /pardon;<br>
                <code>leafpunish.command.pardonid</code> - /pardonid;<br>
                <code>leafpunish.command.unmute</code> - /unmute;<br>
                <code>leafpunish.command.unban</code> - /unban;
            </p>
        </procedure>
    </tab>
    <tab title="Comandos">
        <procedure title="Comandos">
            <p>Abaixo você pode visualizar os comandos disponíveis para este plugin.</p>
            <p>
                <code>/checkplayer</code> - Cheque se o jogador está punido;<br>
                <code>/punishedit</code> - Edite uma punição pelo ID;<br>
                <code>/punishinfo</code> - Veja uma punição pelo ID;<br>
                <code>/kick</code> - Expulsar um jogador;<br>
                <code>/mute</code> - Silenciar um jogador permanentemente;<br>
                <code>/tempmute</code> - Silenciar um jogador temporariamente;<br>
                <code>/ban</code> - Banir um jogador permanentemente;<br>
                <code>/tempban</code> - Banir um jogador temporariamente;<br>
                <code>/pardon</code> - Revogar todas as punições de um jogador;<br>
                <code>/pardonid</code> - Revogue uma punição pela ID;<br>
                <code>/unmute</code> - Revogue o silenciamento de um jogador;<br>
                <code>/unban</code> - Revogue o banimento de um jogador;
            </p>
            <p><control>Comandos(Versão Premium)</control></p>
            <p>
                <code>/historic</code> - Visualizar histórico de punições de um jogador;<br>
                <code>/punishments</code> - Visualizar punições do servidor;<br>
                <code>/clearhistoric</code> - Limpar histórico de punições de um jogador;<br>
                <code>/clearwarnings</code> - Remover os alertas de um jogador;<br>
                <code>/ipban</code> - Banir o endereço-ip de um jogador permanentemente;<br>
                <code>/tempipban</code> - Banir o endereço-ip de um jogador temporariamente;<br>
                <code>/warn</code> - Alertar um jogador;<br>
                <code>/punir</code> - Punir um jogador;
            </p>
        </procedure>
    </tab>
</tabs>

## Arquivos de Configuração

<p>Abaixo você poderá consultar os arquivos de configuração que este plugin disponibiliza.</p>

<include from="arquivos-punish.md" element-id="arquivos-punish"></include>

## Tutoriais

<p>Logo abaixo estaremos disponibilizandos alguns tutoriais para sanar dúvidas em relação ao plugin.</p>

<chapter title="Clique aqui" collapsible="true">
    <deflist>
        <def title="Como usar LeafDiscord + LeafPunish?">
            <p>Abaixo você aprenderá a como configurar aplicações webhooks para o LeafPunish.</p>
            <video src="https://www.youtube.com/watch?v=zVm-nnQJII4"/>
        </def>
    </deflist>
</chapter>
