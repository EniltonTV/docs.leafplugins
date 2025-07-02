# Criação de Items

<p xmlns="">A Leaf possui um sistema de criação de items prático similar aos demais plugins, você poderá usar o <control><emphasis>Minecraft ID/raw name</emphasis></control> para criação de seus items, será possível usar valores data dos itens, como por exemplo blocos com variações coloridas.</p>

<table width="600" style="header-row" border="false">
    <tr>
        <td width="1"></td>
        <td><control>Versões</control></td>
        <td><control>Suporta ID's</control></td>
        <td><control>Suporta Names</control></td>
    </tr>
    <tr>
        <td width="1"></td>
        <td><emphasis>1.8, 1.9, 1.10, 1.11, 1.12</emphasis></td>
        <td><icon src="../images/filled-checked-checkbox (2).png"/></td>
        <td><icon src="../images/filled-checked-checkbox (2).png"/></td>
    </tr>
    <tr>
        <td width="1"></td>
        <td><emphasis>1.13+</emphasis></td>
        <td></td>
        <td><icon src="../images/filled-checked-checkbox (2).png"/></td>
    </tr>
</table>

## Criando items

<p>Logo abaixo estaremos disponibilizando alguns breves exemplos de como criar items em nossos arquivos de configuração.</p>

<chapter title="Criação de items padrão" collapsible="true">
        <p>
            Para criar items por ID(Veja se sua versão é compatível com está opção) basta seguir este exemplo abaixo:
            <code-block lang="yaml">
                items:
                # Não altere o ID dos seguintes itens: mito-atual, mito-nenhum, top-list
                mito-atual:
                name: "&eMito Atual"
                item: "5:0"
                slot: 13
                lore:
                - ""
                - " &a%mitotimes%ª vez &fde &7%mitoname%"
                - ""
                - "&8Desde %mitodate%"
            </code-block>
            <br><br>
            O <code>id</code> de valor <code>5:0</code> é o item madeira de carvalho, o número logo após será sua <code>data</code>, items do mesmo tipo podem possuir variação destintas como blocos de lã que possuem variações de cores. Cada variação possuirá uma <code>data</code> destinta.
            <br><br>
            Para a criação de items por <code>raw name</code> você só precisará atribuir o nome do item que deseja e sua <code>data</code> um simples exemplo: <code>WOOD:0</code> bloco de madeira sem variações.
        </p>
</chapter>
<chapter title="Criação de heads(cabeças) personalizadas." collapsible="true">
        <p>Para encontrar heads personalizadas você pode acessar este site <a href="https://minecraft-heads.com/custom-heads">acessando aqui</a></p>
        <p>
            Introduza apenas o value da URL na opção <code>item</code>, seguindo este exemplo abaixo:<br>
            <code-block lang="yaml">
                items:
                # Não altere o ID dos seguintes itens: mito-atual, mito-nenhum, top-list
                mito-atual:
                name: "&eMito Atual"
                item: "head:2c45702c026252f9e03e6a5d3e2074f4e2a7ed0e742c5b381dda1e629078b5c"
                slot: 13
                lore:
                - ""
                - " &a%mitotimes%ª vez &fde &7%mitoname%"
                - ""
                - "&8Desde %mitodate%"
            </code-block>
            <br>
            Caso você deseje apenas puxar a head de um jogador específico você pode atribuir o valor <code>head:nickname</code> altere o valor <code>nickname</code> para o nome do jogador.
            <br><br>
            Você também poderá puxar a cabeça do jogador que abrir um menu de interação atribuindo o valor <code>head:player</code> (Não é preciso ultilizar nicknames apenas deixar deste modo).
        </p>
</chapter>
<chapter title="Criando items personalizados(Custom Model Data & Items Adders)" collapsible="true">
        <p>
            Para criação de items model data você pode optar por usar id ou name. Basta adicionar o <code>id</code> do custom model após a variação de item(Caso o item não possua variação ultilize o valor <code>0</code>)
            <br><br>
            Um breve exemplo abaixo:
            <code-block lang="yaml">
                items:
                # Não altere o ID dos seguintes itens: mito-atual, mito-nenhum, top-list
                mito-atual:
                name: "&eMito Atual"
                # Uma madeira sem variação sendo usada como custom model com id 1;
                item: "wood:0:1"
                slot: 13
                lore:
                - ""
                - " &a%mitotimes%ª vez &fde &7%mitoname%"
                - ""
                - "&8Desde %mitodate%"
            </code-block>
            <br><br>
            Para criação de items pelo Items Adders basta seguir o exemplo abaixo:
            <code-block lang="yaml">
                items:
                # Não altere o ID dos seguintes itens: mito-atual, mito-nenhum, top-list
                mito-atual:
                name: "&eMito Atual"
                item: "itemsadder:tag:estrela"
                slot: 13
                lore:
                - ""
                - " &a%mitotimes%ª vez &fde &7%mitoname%"
                - ""
                - "&8Desde %mitodate%"
            </code-block>
        </p>
</chapter>