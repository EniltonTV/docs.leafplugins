# API para Desenvolvedores

Para utilizar a API de nossos plugins, é necessário que você tenha a ```.JAR``` do LeafPlugins.

Você pode baixar <a href="https://leafplugins.com/?download=LeafPlugins">aqui</a> o arquivo .JAR , nele estará todas as APIs de nossos plugins (Gratuitos e pagos). Além de também possuir sistemas importantes como por exemplo a classe User que é utilizada nos plugins que armazenam em banco de dados e muito mais. Onde fornece as informações como UUID, Nome do jogador, Data de criação e Último Login.

### Como usar a instância?
Para a facilidade, nossas APIs possuem um padrão. Observe exemplos:

<code-block lang="plain text">LeafPunishAPI.getApi() - LeafTagsAPI.getApi() - LeafCombatLogAPI.getApi()</code-block>

### Tutoriais

<p>Logo abaixo estaremos disponibilizandos alguns tutoriais para sanar dúvidas em relação ao conteúdo.</p>

<chapter title="Clique aqui" collapsible="true">
    <p>Abaixo você encontra um video demonstrativo de como usar adicionar a API <a href="https://www.leafplugins.com/">LeafPlugins</a> em seu projeto, você pode optar por adicionar via mavem através do arquivo <code>pom.xml</code> basta indicar o diretório onde o arquivo <code>.JAR</code> se encontra.</p><br>
    <p><br></p>
<request>
    <deflist>
        <def title="API LeafPlugins">
            <p>Como adicionar API LeafPlugins em seu projeto?</p>
            <video src="https://youtu.be/d7AkJLOGwBg"/>
        </def>
    </deflist>
        <sample lang="json" title="pom.xml">
            &lt;dependencies&gt;
                &lt;dependency&gt;
                    &lt;groupId&gt;www.leafplugins.com&lt;/groupId&gt;
                    &lt;artifactId&gt;leafplugins&lt;/artifactId&gt;
                    &lt;version&gt;lastest&lt;/version&gt;
                    &lt;scope&gt;system&lt;/scope&gt;
                    &lt;systemPath&gt;C:/Arquivos/LeafPlugins.jar&lt;/systemPath&gt;
                &lt;/dependency&gt;
            &lt;/dependencies&gt;
        </sample>
    </request>
</chapter>



                    