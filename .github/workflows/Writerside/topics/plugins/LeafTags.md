# LeafTags
<secondary-label ref="gratuita"/>
<secondary-label ref="premium"/>

<p>Altere o ambiente visual de seu servidor adicionando tags exclusivas!</p>

## Compatibilidades

<list>
    <li>
        <p>Tags por textura(ItemsAdder, Oraxem e etc);</p>
    </li>
    <li>
        <p>LuckPerms/PermissionsEX - Altere tag sempre que mudar de cargo;</p>
    </li>
    <li>
        <p>LeafMedals - Definir medalhas automaticamente</p>
    </li>
    <li>
        <p>TAB - Caso esteja com problema para usar, clique aqui;</p>
    </li>
    <li>
        <p>Gradiente/Cores hex(ou RGB) - Apartir da versão 1.16+ será possível deixar sua tag mais style;</p>
    </li>
</list>

## Premium

<p>Ao adquirir uma versão aprimorada de nossos serviços você estará apoiando nosso projeto e adquirindo vantagens
exclusivas.</p>

<procedure title="Quais sãos as vantagens?">
    <step>
        <p>Suporte de caractéres ampliado nas versões 1.8 e 1.12 (Tags maiores);</p>
    </step>
    <step>
        <p>Nomes de usuário personalizados;</p>
    </step>
    <step>
        <p>Tags abovename e animadas;</p>
    </step>
</procedure>

## Ultilitários

<tabs>
    <tab title="Placeholders">
        <procedure title="Placeholders">
            <p>
                Caso queira pegar o cargo do jogador/maior tag do jogador, altere o tag das placeholders para maxtag. Exemplo: <code>{maxtag_prefix}</code> ou <code>%leaftags_maxtag_prefix%</code>
            </p>
            <p>
                <control>PlaceholderAPI</control>
            </p>
            <p>
                <code>%leaftags_tags_﹤id﹥_﹤informação﹥%</code> - Retornará a informação da tag.<br>
                <br><code>%leaftags_tag_﹤informação﹥%</code> - Retornará a informação da tag do jogador.
            </p>
            <p>
                Altere <control>﹤id﹥</control> para o id de alguma tag do servidor;<br>
                Altere <control>﹤informação﹥</control> para alguma destas:
            </p>
            <p>
                <code>id, name, color, icon, prefix, prefix_animated, suffix, preset, preview, abovename, description, tabprefix, tabsuffix, permission, position.</code>
            </p>
            <p>
                <code>%leaftags_suffix_﹤Informação﹥%</code> - Retornará a informação do sufixo customizado do jogador.<br>
                Altere <control>﹤informação﹥</control> para alguma destas:
            </p>
            <p>
                <code>id, name, suffix, preset, preview, permission.</code>
            </p>
        </procedure>
    </tab>
    <tab title="Permissões">
        <procedure title="Permissões">
            <p>Abaixo você pode visualizar as permissões disponíveis para este plugin.</p>
            <p>
                <code>leaftags.command.settag</code> - Permissão para setar uma tag para o jogador;<br>
                <code>leaftags.command.givetag</code> - Permissão para dar uma tag para o jogador;<br>
                <code>leaftags.command.removetag</code> - Permissão para remover uma tag do jogador
            </p>
        </procedure>
    </tab>
    <tab title="Comandos">
        <procedure title="Comandos">
            <p> Abaixo você pode visualizar os comandos disponíveis para este plugin.</p>
            <p>
                <code>/tags</code> - Selecionar uma tag;<br>
                <code>/suffix </code> - Selecionar uma tag suffixo;<br>
                <code>/settag </code> - Setar uma tag para o jogador;<br>
                <code>/givetag</code> - Adicionar uma tag para o jogador;<br>
                <code>/removetag</code> - Remover uma tag do jogador;
            </p>
        </procedure>
    </tab>
</tabs>

## Arquivos de Configuração

<p>Abaixo você poderá consultar os arquivos de configuração que este plugin disponibiliza.</p>

<include from="arquivos-tags.md" element-id="arquivos-tags"></include>

## Tutoriais

<p>Logo abaixo estaremos disponibilizandos alguns tutoriais para sanar dúvidas em relação ao plugin.</p>

<chapter title="Clique aqui" collapsible="true">
    <deflist>
        <def title="LeafTags + TAB como usar?">
            <p>Abaixo você aprenderá a como configurar o leaftags no plugin TAB.</p>
            <video src="https://youtu.be/OCjI5uqjLnY"/>
        </def>
    </deflist>
</chapter>