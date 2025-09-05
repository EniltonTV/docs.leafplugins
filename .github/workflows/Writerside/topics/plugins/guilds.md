# LeafGuilds
<secondary-label ref="premium"/>

<p>Um sistema de clãs & guildas Simples e dinâmico.</p>

## Compatibilidades

<list>
    <li>
        <p>nChat e LegendChat & PlaceholderAPI;</p>
    </li>
    <li>
        <p>Bungeecord (apenas comunicação)</p>
    </li>
    <li>
        <p>nLogin - Notifique sempre que um membro logar após autenticação;</p>
    </li>
    <li>
        <p>Suporte para economias (<a href="dependencias-utilitarios.md" anchor="economies">Clique aqui</a> para consultar as economias disponíveis).</p>
    </li>
</list>

## Premium

<p>Ao adquirir uma versão aprimorada de nossos serviços você estará apoiando nosso projeto e adquirindo vantagens exclusivas.</p>

<procedure title="Quais sãos as vantagens?">
    <list>
        <li>
            <p>Criação de placeholders customizáveis;</p>
        </li>
        <li>
            <p>Plugin 100% configurável;</p>
        </li>
        <li>
            <p>Sistema de ícone, descrição, tags e <control>muito mais</control>.</p>
        </li>
    </list>
</procedure>

## Utilitários

<tabs>
    <tab title="Placeholders">
        <procedure title="Placeholders">
            <p><control>PlaceholderAPI</control></p>
            <p>
                <code>%leafguilds_in_guild%</code> - Retornará se o jogador está em uma guilda ("true" ou "false");<br>
                <code>%leafguilds_role%</code> - Retornará o nome do cargo do jogador.
            </p>
            <p>
                <code>%leafguilds_role_﹤informação﹥% </code>- Retornará a informação do cargo do jogador;<br>
                Altere <code>﹤informação﹥</code> para alguma destas:<br>
            </p>
            <p><code>name, prefix, color.</code></p>
            <p>
                <code>%leafguilds_guild_﹤informação﹥% </code>- Retornará a informação do cargo do jogador;<br>
                Altere <code>﹤informação﹥</code> para alguma destas:<br>
            </p>
            <p><code>id, name, tag, colortag, icon, creation, is_premium, founder, leader, leaderUUID.</code></p>
        </procedure>
    </tab>
    <tab title="Permissões">
        <procedure title="Permissões">
            <p>Abaixo você pode visualizar as permissões disponíveis para este plugin.</p>
            <p>
                <code>leafguilds.admin</code> - Permissão para abrir paínel administrativo;
            </p>
        </procedure>
    </tab>
    <tab title="Comandos">
        <procedure title="Comandos">
            <p>Abaixo você pode visualizar os comandos disponíveis para este plugin.</p>
            <p>
                <code>/guilds</code> - Menu das Guildas no servidor;  <br>
                <code>/guildadmin</code> - Abrir o painel de admin no chat;<br>
                <code>/guild</code> - Abrir o painel no chat;<br>
                <code>/guild info</code> - Informações da Guilda;<br>  
                <code>/guild criar</code> - Criar uma Guilda;<br>
                <code>/guild excluir</code> - Excluir a guilda;<br>
                <code>/guild sair</code> - Sair da guilda;<br>
                <code>/guild online</code> - Membros da guilda online;<br>  
                <code>/guild expulsar &lt;jogador&gt;</code> - Expulsar um membro da guilda;<br> 
                <code>/guild promover &lt;jogador&gt;</code> - Promover um membro para moderador;<br> 
                <code>/guild rebaixar &lt;jogador&gt;</code> - Rebaixar um moderador para membro;<br>
                <code>/guild transferir &lt;jogador&gt;</code> - Transferir a posse para um moderador;<br>
                <code>/guild convidar &lt;jogador&gt;</code> - Convidar um jogador;<br>
                <code>/guild convites</code> - Consultar os convites recebidos.
            </p>
        </procedure>
    </tab>
</tabs>

## Arquivos de Configuração

<p>Abaixo você poderá consultar os arquivos de configuração que este plugin disponibiliza.</p>

<include from="arquivos-guilds.md" element-id="arquivos-guilds"></include>

## Tutoriais
<secondary-label ref="breve"/>

<p>Logo abaixo estaremos disponibilizandos alguns tutoriais para sanar dúvidas em relação ao plugin.

<seealso title="Veja mais sobre">
    <category ref="wrs">
        <a href="dependencias-utilitarios.md"/>
        <a href="versoes-premium.md"/>
        <a href="criacao-items.md"/>
        <a href="conditions.md"/>
    </category>
</seealso>