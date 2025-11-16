# LeafMedals
<secondary-label ref="gratuita"/>
<secondary-label ref="premium"/>

<p>Recompense seus jogadores com nosso sistema de medalhas único!</p>

## Compatibilidades

<list>
  <li>
    <p>LeafTags - Definir medalhas automaticamente no suffixo;</p>
  </li>
  <li>
    <p>Gradiente/Cores hex(ou RGB) - Apartir da versão 1.16+ será possível deixar sua tag mais style.</p>
  </li>
</list>

## Premium

<p>Ao adquirir uma versão aprimorada de nossos serviços você estará apoiando nosso projeto e adquirindo vantagens
exclusivas.</p>

<procedure title="Quais sãos as vantagens?">
  <step>
    <p>Com a versão premium você pode equipar +3 e criar mais slots para medalhas.</p>
  </step>
</procedure>

## Utilitários

<tabs>
    <tab title="Placeholders">
        <procedure title="Placeholders">
          <p><control>PlaceholderAPI</control></p>
          <p>
            <code>%leafmedals_medals%</code> - Retornará o ícone das medalhas;<br>
            <code>%leafmedals_medals_space%</code> - Retornará o ícone das medalhas com espaçamento;<br>
            <code>%leafmedals_medal_﹤slot﹥_﹤informação﹥%</code> - Retornará a informação da medalha.
          </p>
          <p>
            Altere <control>﹤slot﹥</control> para o exibir informações sobre a medalha equipada nele;<br>
            Altere <control>﹤informação﹥</control> para alguma destas:
          </p>
          <p>
          <code>id, name, color, icon, prefix, suffix, preset, rarity, description, permission.</code>
          </p>
          <p>
            <control>LegendChat ou nChat</control>
          </p>
          <p>
            <code>{medals}</code> - Retornará o ícone das medalhas;<br>
            <code>{medals_space}</code> - Retornará o ícone das medalhas com espaçamento;<br>
            <code>{medal_﹤slot﹥_﹤informação﹥}</code> - Retornará a informação da medalha.
          </p>
          <p>
            Altere <control>﹤slot﹥</control> para o exibir informações sobre a medalha equipada nele;
          </p>
          <p>
            Altere <control>﹤informação﹥</control> para alguma destas:
          </p>
          <p>
            <code>id, name, color, icon, prefix, suffix, preset, rarity, description, permission.</code>
          </p>
        </procedure>
    </tab>
    <tab title="Permissões">
        <procedure title="Permissões">
          <p>Abaixo você pode visualizar as permissões disponíveis para este plugin.</p>
          <tip>As permissões das medalhas são definidas no arquivo <code>medals.yml</code></tip>
          <p>
            <code>leafmedals.slot.﹤slot﹥</code> - Permissão para liberar o slot para equipar a medalha;<br>
            <code>leafmedals.command.setmedal</code> - Permissão para dar uma medalha para o jogador.<br>
          </p>
        </procedure>
    </tab>
    <tab title="Comandos">
        <procedure title="Comandos">
          <p>Abaixo você pode visualizar os comandos disponíveis para este plugin.</p>
          <p>
            <code>/medals</code> - Selecionar uma medalha;<br>
            <code>/setmedal </code> - Setar uma medalha para um jogador.
          </p>
        </procedure>
    </tab>
</tabs>

## Arquivos de Configuração

<p>Abaixo você poderá consultar os arquivos de configuração que este plugin disponibiliza.</p>

<include from="arquivos-medals.md" element-id="arquivos-medals"></include>

## Tutoriais
<secondary-label ref="breve"/>

<p>Logo abaixo estaremos disponibilizandos alguns tutoriais para sanar dúvidas em relação ao plugin.</p>

<seealso title="Veja mais sobre">
    <category ref="wrs">
        <a href="dependencias-ultilitarios.md"/>
        <a href="versoes-premium.md"/>
        <a href="criacao-items.md"/>
        <a href="conditions.md"/>
    </category>
</seealso>