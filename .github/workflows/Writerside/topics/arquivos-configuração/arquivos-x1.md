# arquivos-x1

<chapter id="arquivos-x1" title="Arquivos" collapsible="true">
    <chapter title="lang/" collapsible="true">
        <chapter title="messages_pt.yml" collapsible="true">
<code-block lang="yaml">
x1-empate-pvp: '&amp;eDuelo empatado!'
duelo-empatado-anuncio: '&amp;f%s &amp;eempatou contra &amp;f%s &amp;eno &amp;e&amp;lX1&amp;l&amp;e!'
duelo-vitoria-anuncio: '&amp;aO jogador &amp;f%s &amp;avenceu o jogador &amp;f%s &amp;ano &amp;a&amp;lX1&amp;a!'
x1-actionbar-pvp: '&amp;f%s &amp;c%sHP &amp;f- &amp;b%s'
x1-assistir-nenhum-encontrado: '&amp;cDuelo não encontrado.'
x1-assistir: '&amp;bVocê está assistindo o duelo entre &amp;f%s e &amp;f%s&amp;b!'
x1-anuncio-assistir: '&amp;eO jogador &amp;f%s &amp;eestá enfrentando &amp;f%s&amp;e! &amp;eClique &amp;faqui &amp;epara assistir.'
x1-iniciar: '&amp;aO duelo começará em &amp;f%s&amp;a...'
x1-arena-nao-existe: '&amp;cNão há arenas disponíveis no momento.'
x1-ja-convidou: '&amp;cVocê já convidou este jogador para um duelo.'
x1-convite-enviado: '&amp;aVocê convidou o jogador &amp;f%s &amp;apara um duelo.'
x1-convite-recebido: '&amp;f%s &amp;aconvidou você para um duelo. &amp;aClique &amp;faqui &amp;apara aceitar.'
x1-sem-money: '&amp;cVocê não possui dinheiro suficiente para apostar.'
apostas-desativadas: '&amp;cAs apostas estão desativadas.'
aposta-minima: '&amp;cA aposta mínima é de &amp;f%s.'
aposta-maxima: '&amp;cA aposta máxima é de &amp;f%s.'
x1-saindo-da-arena: '&amp;eSaindo da arena em &amp;f%s&amp;e...'
x1-vitoria-duelo: '&amp;aParabéns! Você derrotou o jogador &amp;f%s &amp;ae recebeu &amp;f%s&amp;a.'
x1-derrota-duelo: '&amp;cVocê foi derrotado para o jogador &amp;f%s &amp;ce perdeu &amp;f%s&amp;c.'
x1-toggle: '&amp;cVocê desabilitou os convites para novos duelos.'
x1-toggle-oponente: '&amp;cEste jogador desabilitou os convites para novos duelos.'
x1-aceito-oponente: '&amp;aVocê aceitou o desafio de &amp;f%s!'
x1-aceitar: '&amp;bUtilize /x1 aceitar &amp;f&lt;player&gt; &amp;bpara aceitar o convite de outra pessoa.'
x1-aceito: '&amp;f%s &amp;aaceitou o desafio!'
x1-recusar: '&amp;bUtilize /x1 recusar &amp;f&lt;player&gt; &amp;bpara recusar o convite de outra pessoa.'
x1-recusou: '&amp;cVocê recusou o desafio do jogador &amp;f%s&amp;c!'
x1-recusado: '&amp;cO jogador &amp;f%s &amp;crecusou o seu desafio!'
x1-animação: '&amp;aAnimação &amp;f%s &amp;aselecionada.'
x1-ajuda: '&amp;bUtilize /x1 &amp;f&lt;player&gt; &amp;bpara convidar outra pessoa para um duelo.'
x1-arena-selecionada: '&amp;aArena &amp;f%s &amp;aselecionada.'
x1-comandos-desativados: '&amp;cOs comandos estão desabilitados durante o duelo.'
x1-watch: '&amp;bUtilize /x1 watch &amp;f&lt;player&gt; &amp;bpara assistir o duelo de outro jogador.'
x1-nao-desafiado: '&amp;cVocê não foi desafiado por este jogador.'
x1-jogador-em-combate: '&amp;cEste jogador está em combate.'
x1-nao-esta-em-combate: '&amp;cVocê não está em combate.'
x1-convite-expirou: '&amp;cO convite de duelo contra &amp;f%s &amp;cexpirou.'
jogador-nao-encontrado: '&amp;cJogador não encontrado.'
sem-auto-desafio: '&amp;cVocê não pode se desafiar.'
impossivel-desafiar: '&amp;cVocê não pode desafiar um jogador enquanto estiver em combate.'
x1-arena-sem-kit: '&amp;cA arena selecionada não possui kit setado.'
</code-block>
        </chapter>
    </chapter>
    <chapter title="menus/" collapsible="true">
        <chapter title="menus.yml" collapsible="true">
<code-block lang="yaml">
invite-duel:
  title: "Desafiar %target%"
  slots: 54
  items:
    info:
      name: "&eInformações de %target%"
      item: "head:%target%"
      slot: 4
      lore:
        - ""
        - "&fElo: &b✦ %elo%"
        - "&fDuelos totais: &e%duels%"
        - ""
        - "&fAbates: &a%kills%"
        - "&fMortes: &c%deaths%"
        - "&fK/D: &9%kd%"
        - ""
    themes:
      name: "&eTema da arena"
      item: "item_frame"
      slot: 10
      lore:
        - "&7Clique para definir o tema da arena."
    animation:
      name: "&6Animação de vitória"
      item: "377"
      slot: 22
      lore:
        - "&7Clique para escolher a animação de vitória."
    ownitems:
      name: "&eUtilizar itens próprios &l%active%"
      item: "iron_sword"
      slot: 16
      lore:
        - "&7Clique para &f%enabled% &7seus itens próprios no combate."
    lowerbet:
      name: "&cDiminuir aposta"
      item: "ink_sack:1"
      slot: 29
      lore:
        - "&7Clique para diminuir a aposta."
    raisebet:
      name: "&aAumentar aposta"
      item: "ink_sack:10"
      slot: 33
      lore:
        - "&7Clique para aumentar a aposta."
    bet:
      name: "&eInformações da aposta"
      item: "gold_ingot"
      slot: 31
      lore:
        - ""
        - "&7Quantia da aposta: &2&l$ &a%bet%"
        - ""
    challenge:
      name: "&aDesafiar %target%"
      item: "wool:5"
      slot: 49
      lore:
        - "&7Clique para confirmar o desafio."
</code-block>
        </chapter>
    </chapter>
    <chapter title="settings/" collapsible="true">
        <chapter title="commands.yml" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração

x1:
name: x1
use-command: true
permission: ''
aliases:
- desafiar
- chamarx1
</code-block>
        </chapter>
    </chapter>
    <chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
# Agradecemos por escolher o LeafX1 ♥
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
host: 'localhost'
user: 'root'
password: ''
port: 3306
database: 'leaf'

# Configurações de pool da conexão MYSQL (AVANÇADO)
pool-settings:
enable: true
max-pool-size: 30
min-idle: 10
max-lifetime: 1800000 # 30 minutos
connection-timeout: 5000 # 5 segundos

# Configurações do plugin.

settings:
type: SIMPLE # SIMPLE

# Tempo máximo para o duelo, caso ultrapasse terminará empatado. (em minutos)
max-time-duel: 5

bet:
# Habilitar sistema de apostas.
enabled: true

    # Economia utilizada para apostas.
    economy: 'Vault'

    # Valor de aumento/diminuição de aposta.
    raise-bet: 1000

    # Valor mínimo de aposta.
    bet-min: 0

    # Valor máximo de aposta.
    bet-max: 100000

    # Valor de aposta padrão.
    bet-default: 0

# Valor de aumento/diminuição de elo ao vencer duelo (não é o valor fixo, pois conta com cálculos matemáticos baseado no KDR).
raise-elo: 10

# Valor de elo padrão.
default-elo: 1000

# Comando para executar quando resetar o ranking mensal nos top jogadores de elo.
ranking-monthly-command:
- '' #1
- '' #2
- '' #3

# Comando para executar quando resetar o ranking mensal nos top jogadores de elo.
ranking-weekly-command:
- '' #1
- '' #2
- '' #3

# Tempo de expiração dos convites de duelo (em minutos).
invite-expiration: 2

# Anúncio de duelos para todos os jogadores.
announce-duel: true

# Comandos permitidos em combate.
bypass-commands:
- '/gamemode'
- '/gm'
- '/fly'
- '/voar'
- '/tp'
- '/teleport'
- '/v'
- '/vanish'
- '/god'
- '/x1'
</code-block>
    </chapter>
</chapter>