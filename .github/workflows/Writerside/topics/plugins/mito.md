# LeafMito
<secondary-label ref="gratuita"/>
<secondary-label ref="premium"/>

<p>Torne as disputas de pvp mais competitivas com nosso incrível sistema de mito.</p>

## Compatibilidades

<list>
    <li>
        Decent Holograms/Holographics Displays - crie hologramas para visualização o mito;
    </li>
    <li>
        Citzens2, zNPCSplus e FancyNpcs - crie npcs para visualização do mito.
    </li>
</list>

## Premium

<p>Ao adquirir uma versão aprimorada de nossos serviços você estará apoiando nosso projeto e adquirindo vantagens exclusivas.</p>

<procedure title="Quais sãos as vantagens?">
    <list>
        <li>
            <p>Sistema em menu para o /mito;</p>
        </li>
        <li>
            <p>Sistema de toplist, visualize os jogadores que mais vezes se tornarão mito.</p>
        </li>
    </list>
</procedure>

## Utilitários

<tabs>
    <tab title="Placeholders">
        <procedure title="Placeholders">
            <p><control>PlaceholderAPI</control></p>
            <p><code>%leafmito_tag%</code> - Retornar tag caso o jogador seja o mito;<br>
            <code>%leafmito_atual%</code> - Retorna um valor bolean caso o jogador seja o mito atual;<br>
            <code>%leafmito_vezes%</code> - Retorna quantas vezes o jogador se tornou mito;<br>
            <code>%leafmito_mito%</code> - Retorna o nickname do mito atual;<br>
            <code>%leafmito_mito_uuid% </code> - Retorna uuid do mito;<br>
            <code>%leafmito_mito_vezes%</code> - Retorna quantas vezes o mito atual se tornou mito;<br>
            <code>%leafmito_tem_mito%</code> - Retorna se há algum mito.</p>
            <p><control>nChat ou LegendChat</control></p>
            <p><code>{mito}</code> - Retornar a tag mito.</p>
        </procedure>
    </tab>
    <tab title="Permissões">
        <procedure title="Permissões">
            <p>Abaixo você pode visualizar as permissões disponíveis para este plugin.</p>
            <p><code>mito.gerenciar</code> - Permissão para gerenciar sistema /mito.</p>
        </procedure>
    </tab>
    <tab title="Comandos">
        <procedure title="Comandos">
            <p>Abaixo você pode visualizar os comandos disponíveis para este plugin.</p>
            <p><code>/mito</code> - Gerenciar o mito (caso não possua permissão, falará quem é o mito atual ou abrirá o menu).<br>
            <code>/mito menu</code> - Abrir o meu do mito;<br>
            <code>/mito atual</code> - Consultar quem é o atual mito;<br>
            <code>/mito npc</code> - Setar o npc do mito atual;<br>
            <code>/mito remover;</code> - Remover o mito atual;<br>
            <code>/mito setar random</code> - Setar aleatoriamente um novo mito;<br>
            <code>/mito setar [Jogador]</code> - Setar o mito para um jogador específico;<br>
            <code>/mito pausar</code> - Pausar/Reativar a tranferência do mito por morte.</p>
        </procedure>
    </tab>
</tabs>

## Arquivos de Configuração

Abaixo você poderá consultar os arquivos de configuração que este plugin disponibiliza.

<include from="arquivos-mito.md" element-id="arquivos-mito"></include>

## Tutoriais

<p>Logo abaixo estaremos disponibilizandos alguns tutoriais para sanar dúvidas em relação ao plugin.</p>

<chapter title="Clique aqui" collapsible="true">
    <deflist>
        <def title="Configurando aplicações webhooks">
            <p>Abaixo você aprenderá a como configurar aplicações webhooks para o LeafMito.</p>
            <video src="https://youtu.be/Ae0m8Yp-ULY"/>
        </def>
    </deflist>
</chapter>

<seealso title="Veja mais sobre">
    <category ref="wrs">
        <a href="dependencias-ultilitarios.md"/>
        <a href="versoes-premium.md"/>
        <a href="criacao-items.md"/>
        <a href="conditions.md"/>
    </category>
</seealso>