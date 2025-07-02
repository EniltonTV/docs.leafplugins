# Usando as Conditions

<p>As conditions ou "condições" são valores atribuídos para checagens & formatação em nossos sistemas de mensagens.</p>

<tip>Vale ressaltar que este sistema está presente em apenas alguns plugins de nosso catálogo(Leaf Tags & Score).</tip>

## Center

<p>
    O <code>center</code> tem a função de centralizar o texto no chat.<br>
    Exemplo:  <code># &lt;center&gt;Mensagem centralizada!&lt;/center&gt;</code>
</p>

## When

<p>
    O <code>when</code> tem a função de verificar caso o texto seja equivalente(ignorando letras maiúsculas e minúsculas) ao <code>input</code>, caso seja, retornará o <code>output</code>. 
</p>

<tip>
    Os whens possui o input "empty" que checa se o texto está em branco/vazio.
    Você também poderá fazer que o output retorne alguma outra placeholder.
</tip>

<p>Exemplo: <code>&lt;when="empty"&gt;%simpleclans_clan_color_tag%&lt;/when="&cSem clan"&gt;</code></p>

<p>Esta checagem verifica se o texto que a placeholder <code>%simpleclans_clan_color_tag%</code> retornar está em branco. Caso seja, quer dizer que o jogador não possui um clan, com isso fará que apareça pro jogador a mensagem: &cSem clan"</p>

<p>Outro exemplo: <code>&lt;when="steve"&gt;%player_name%&lt;/when="&aVocê é o Steve!"&gt;</code></p>

<p>Esta checagem verifica se o texto que a placeholder <code>%player_name%</code> retornar é equivalente a "steve", ignorando letras maiúsculas e minúsculas.  Caso seja, quer dizer que o jogador possui o nome "Steve".</p>

## WhenNotEqual

<p>
    O <code>whennotequal</code> tem a função de verificar caso o texto NÃO seja EXATAMENTE IGUAL ao <code>input</code>, caso não seja, retornará o <code>output</code>. 
</p>

<tip>
    Os whens possui o <code>input</code> "empty" que checa se o texto está em branco/vazio.
    Você também poderá fazer que o <code>output</code> retorne alguma outra placeholder.
</tip>

<p>Exemplo: <code>&lt;whennotequal="AmenDoim"&gt;%player_name%&lt;/whennotequal="&cVocê não é AmenDoim!"&gt;</code></p>

<p>Esta checagem verifica se o texto que a placeholder <code>%player_name%</code> retornar não é exatamente igual a "AmenDoim". Caso não seja, quer dizer que o jogador não tem o nickname "AmenDoim".</p>

## WhenEqual

<p>O <code>whenequal</code> tem a função de verificar caso o texto seja EXATAMENTE IGUAL ao <code>input</code>, caso seja, retornará o <code>output</code>.</p>

<tip>
    Os whens possui o input "empty" que checa se o texto está em branco/vazio.
    Você também poderá fazer que o output retorne alguma outra placeholder.
</tip>

<p>Exemplo: <code>>&lt;whenequal="AmenDoim"&gt;%player_name%&lt;/whenequal="&aVocê é AmenDoim!"&gt;</code></p>

<p>Esta checagem verifica se o texto que a placeholder <code>%player_name%</code> retornar é exatamente igual a "AmenDoim". Caso seja, quer dizer que o jogador tem o nickname "AmenDoim".</p>

## hasPermission

<p>O <code>haspermission</code> tem a função de verificar caso o jogador possua a permissão <code>input.</code> Caso tenha, retornará o texto. Caso não tenha, retornará o <code>output</code>.</p>

<tip>
    Os hasPermission possui o input "op" que checa se o player tem OP.
    Você também poderá fazer que o output retorne alguma outra placeholder.
</tip>

<p>Exemplo: <code>&lt;haspermission="op"&gt;Você é OP!&lt;/haspermission="Sem perm"&gt;</code></p>

<p>Esta checagem verifica se o jogador possui OP, caso tenha aparecerá "Você é OP!". Caso o ao contrário, aparecerá: "Sem perm"</p>

<p>Outro exemplo: <code>&lt;haspermission="server.admin"&gt;Você é Admin!&lt;/haspermission="Sem perm"&gt;</code></p>

<p>Esta checagem verifica se o jogador possui permissão "server.admin", caso tenha aparecerá "Você é Admin!". Caso o ao contrário, aparecerá: "Sem perm"</p>

## hasPermission true/false

<tip>Os hasPermission possui o input "op" que checa se o player tem OP.</tip>

<p>Exemplo: <code>&lt;haspermission true="op"&gt;Você é OP!&lt;/haspermission&gt;</code></p>