# arquivos-mysterybox

<chapter id="arquivos-mysterybox" title="Arquivos" collapsible="true">
    <chapter title="lang/" collapsible="true">
        <chapter title="messages_pt.yml" collapsible="true">
<code-block lang="yaml">
prize:
  - ''
  - '&7[&6%box_name%&7] &fParabéns, &7%opener_displayname%&f! Você ganhou:'
  - '&f- &a%prize_name% &fde raridade &a%rarity_displayname%'
  - ''

cant-open: '&cPara abrir &f%box_name% &cé necessário possuir uma caixa ou uma chave desta caixa em mãos.'
max-boxes-openning: '&cVocê já está abrindo o número máximo de caixas permitido (&f%max_boxes%&c). Aguarde terminar de abrir as caixas atuais.'
no-permission-instantly-open: '&cVocê não possui permissão para abrir caixas instantaneamente.'

actionBar:
opening: '&aAbrindo &f%box_name%'
already_opening: '&cVocê já está abrindo esta caixa'
someone_already_opening: '&cA &f%box_name% &cjá está sendo aberta por &f%player_displayname%'
</code-block>
        </chapter>
    </chapter>
    <chapter title="menus/" collapsible="true">
        <chapter title="inspect-menu.yml" collapsible="true">
<code-block lang="yaml">
main-menu:
  title: "%box_name% - Prêmios"
  slots: 54

list:
# Slots que os itens ocuparão
slots: [10, 11, 12, 13, 14, 15, 16, 19, 20, 21, 22, 23, 24, 25, 28, 29, 30, 31, 32, 33, 34, 37, 38, 39, 40, 41, 42, 43]

    # Formato dos itens dos prêmios
    format:
      name: "%prize_name%"
      item: "%prize_icon%"
      lore:
        - ""
        - " &fRaridade: &a%rarity_displayname%"
        - " &fProbabilidade: &b%prize_chance%%"
        - ""

# Altere como quiser (Adicionar, remover, editar itens)
items:
historic:
name: "&a%player_displayname%"
item: "head:player"
slot: 48
lore:
- ""
- " &fCaixas disponíveis: &a%boxes%"
- ""
- "&eClique para conferir seus ganhos"


    open:
      name: "&eAbrir caixa"
      item: "TRIPWIRE_HOOK"
      slot: 50
      lore:
        - ""
        - "&f Sair do menu"
        - ""

      closeInventory: true

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
    </chapter>
    <chapter title="prizes/" collapsible="true">
    <chapter title="caixa-avancada.yml" collapsible="true">
<code-block lang="yaml">
vip_rank:
  chance: 1.0
  rarity: legendary
  display:
    name: "&6VIP Rank"
    lore:
      - "&7Concede o rank VIP no servidor por tempo indeterminado."
      - "&7Inclui permissões e vantagens exclusivas."
      - "&7Comandos: ajuste conforme seu plugin de permissões."
    icon:
      item: "NAME_TAG"
      glow: true
  commands:
    - "lp user {player} parent add vip"
  broadcast:
    enable: true
    message:
      - ""
      - "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
      - "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
      - ""

5000_money:
chance: 12.0
rarity: rare
display:
name: "&aMoney &ex5000"
lore:
- "&7Um bom aporte de &a5000 &7para gastar no servidor."
- "&7Ideal para comprar equipamentos e começar upgrades."
icon:
item: "GOLD_NUGGET"
glow: false
commands:
- "money give {player} 5000"
broadcast:
enable: false
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

15000_money:
chance: 4.0
rarity: epic
display:
name: "&aMoney &ex15000"
lore:
- "&7Grande recompensa: &a15000 &7de moeda do servidor."
- "&7Perfeito para compras importantes e investimentos."
icon:
item: "GOLD_BLOCK"
glow: true
commands:
- "money give {player} 15000"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

diamond_bundle_x32:
chance: 10.0
rarity: rare
display:
name: "&bDiamantes x32"
lore:
- "&7Um pacote generoso de &b32 &7diamantes."
- "&7Perfeito para forjar ferramentas e armaduras de alto nível."
icon:
item: "DIAMOND"
glow: false
commands:
- "give {player} minecraft:diamond 32"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

diamond_bundle_x64:
chance: 3.0
rarity: epic
display:
name: "&bDiamantes x64"
lore:
- "&7Pacote: &b64 &7diamantes para grandes construções e trocas."
icon:
item: "DIAMOND"
glow: true
commands:
- "give {player} minecraft:diamond 64"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

netherite_set:
chance: 2.5
rarity: legendary
display:
name: "&6Conjunto Netherite"
lore:
- "&7Um conjunto completo de netherite (capacete, peitoral, calça, botas)."
icon:
item: "NETHERITE_HELMET"
glow: false
commands:
- "give {player} minecraft:netherite_helmet 1"
- "give {player} minecraft:netherite_chestplate 1"
- "give {player} minecraft:netherite_leggings 1"
- "give {player} minecraft:netherite_boots 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

elytra_plus_fireworks:
chance: 2.0
rarity: epic
display:
name: "&bElytra + Fogos"
lore:
- "&7Elytra para voar junto com um pacote de fogos."
- "&7Perfeito para viagens rápidas e shows aéreos."
icon:
item: "ELYTRA"
glow: true
commands:
- "give {player} minecraft:elytra 1"
- "give {player} minecraft:firework_rocket 16"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

enchanted_golden_apple_x2:
chance: 0.8
rarity: legendary
display:
name: "&5Maçã Dourada Encantada x16"
lore:
- "&7Duas maçãs encantadas — salve-se de batalhas críticas."
icon:
item: "ENCHANTED_GOLDEN_APPLE"
glow: true
commands:
- "give {player} minecraft:enchanted_golden_apple 16"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

beacon_plus_nether_star:
chance: 1.2
rarity: legendary
display:
name: "&bBeacon + Estrela do Nether"
lore:
- "&7Um beacon completo e a estrela necessária para montar."
icon:
item: "BEACON"
glow: true
commands:
- "give {player} minecraft:beacon 1"
- "give {player} minecraft:nether_star 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

shulker_box_purple_x4:
chance: 6.0
rarity: uncommon
display:
name: "&5Shulker Box Roxa x4"
lore:
- "&7Quatro Shulker Boxes para armazenamento móvel."
icon:
item: "PURPLE_SHULKER_BOX"
glow: false
commands:
- "give {player} minecraft:purple_shulker_box 4"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

iron_tools_set:
chance: 8.0
rarity: common
display:
name: "&7Kit Ferramentas de Ferro"
lore:
- "&7Conjunto básico: picareta, pá, machado e espada de ferro."
- "&7Ótimo para mineração e aventuras iniciais."
icon:
item: "IRON_PICKAXE"
glow: false
commands:
- "give {player} minecraft:iron_pickaxe 1"
- "give {player} minecraft:iron_shovel 1"
- "give {player} minecraft:iron_axe 1"
- "give {player} minecraft:iron_sword 1"
broadcast:
enable: false
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

golden_apple:
chance: 6.0
rarity: rare
display:
name: "&eMaçã Dourada x8"
lore:
- "&7Item de cura rápido — útil em combates ou situações perigosas."
- "&7Um clássico que nunca perde valor."
icon:
item: "GOLDEN_APPLE"
glow: false
commands:
- "give {player} minecraft:golden_apple 8"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

ender_pearl_x16:
chance: 12.0
rarity: common
display:
name: "&5Ender Pearls x16"
lore:
- "&7Pacote de 16 ender pearls para teletransporte e navegação pelo mapa."
- "&7Ótimo para explorar ilhas e fugir de perigos."
icon:
item: "ENDER_PEARL"
glow: false
commands:
- "give {player} minecraft:ender_pearl 16"
broadcast:
enable: false
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

obsidian_x32:
chance: 7.0
rarity: uncommon
display:
name: "&5Obsidiana x32"
lore:
- "&7Blocos resistentes para construções, portais ao Nether ou bastiões."
- "&7Perfeito para quem vai criar defesas sólidas."
icon:
item: "OBSIDIAN"
glow: false
commands:
- "give {player} minecraft:obsidian 32"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

pumpkin_head:
chance: 3.0
rarity: uncommon
display:
name: "&aCabeça de Abóbora"
lore:
- "&7Uma cabeça divertida para decoração ou para se proteger de Endermen."
- "&7Ótima para construções temáticas."
icon:
item: "CARVED_PUMPKIN"
glow: false
commands:
- "give {player} minecraft:carved_pumpkin 1"
broadcast:
enable: false
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

saddle:
chance: 4.0
rarity: rare
display:
name: "&6Sela"
lore:
- "&7Permite montar em porcos, cavalo e outros mobs montáveis."
- "&7Item raro e muito útil em exploração."
icon:
item: "SADDLE"
glow: false
commands:
- "give {player} minecraft:saddle 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

music_disc:
chance: 2.0
rarity: uncommon
display:
name: "&dDisco de Música"
lore:
- "&7Um disco raro para tocar nas jukeboxes do servidor."
- "&7Ótimo para colecionadores e decorações."
icon:
item: "MUSIC_DISC_11"
glow: false
commands:
- "give {player} minecraft:music_disc_11 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

cooked_beef_x32:
chance: 10.0
rarity: common
display:
name: "&cCarne Cozida x32"
lore:
- "&7Um bom suprimento de comida — mantém a barra de fome cheia."
- "&7Útil em longas jornadas e batalhas."
icon:
item: "COOKED_BEEF"
glow: false
commands:
- "give {player} minecraft:cooked_beef 32"
broadcast:
enable: false
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

fishing_rod:
chance: 9.0
rarity: common
display:
name: "&bVara de Pescar"
lore:
- "&7Vara de pesca para conseguir itens, comida e troféus."
- "&7Simples e eficaz — ideal para relaxar no servidor."
icon:
item: "FISHING_ROD"
glow: false
commands:
- "give {player} minecraft:fishing_rod 1"
broadcast:
enable: false
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

emerald_bundle_x16:
chance: 5.0
rarity: uncommon
display:
name: "&aEsmeraldas x16"
lore:
- "&7Moeda de troca para comerciantes do vilarejo."
- "&7Ótimo para trocas e negociações com NPCs."
icon:
item: "EMERALD"
glow: false
commands:
- "give {player} minecraft:emerald 16"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""
</code-block>
</chapter>
<chapter title="caixa-padrao.yml" collapsible="true">
<code-block lang="yaml">
creeper_head:
  # Chance de ganhar este prêmio (0.0 a 100.0) em porcentagem
  chance: 1.0
  # Raridade deste prêmio (deve existir em rarities.yml)
  rarity: legendary

# Visual do prêmio (no inventário da caixa, holograma, mensagem de broadcast, etc)
display:
# Nome do prêmio
name: "&aCabeça de Creeper"
# Descrição do prêmio
lore:
- "&7Uma cabeça assustadora de creeper — um troféu sinistro."
- "&7Perfeita para decoração ou para intimidar visitantes."
- "&7Mostre suas conquistas: item raro e cheio de personalidade."
# Icone do prêmio
icon:
item: "CREEPER_HEAD"
glow: false

# Comandos que serão executados ao ganhar este prêmio
commands:
- "give {player} minecraft:creeper_head 1"

# Mensagem enviada para todos os jogadores
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

1000_money:
# Chance de ganhar esta prêmio (0.0 a 100.0) em porcentagem
chance: 5.0
# Raridade desta prêmio (deve existir em rarities.yml)
rarity: common

# Visual da prêmio (no inventário da caixa, holograma, mensagem de broadcast, etc)
display:
# Nome da prêmio
name: "&aMoney &ex1000"
# Descrição da prêmio
lore:
- "&71000 de money para gastar como quiser!"
# Icone da prêmio
icon:
item: "GOLD_NUGGET"
glow: false

# Comandos que serão executados ao ganhar esta prêmio
commands:
- "money give {player} 1000"

# Mensagem enviada para todos os jogadores
broadcast:
enable: false
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

netherite_ingot:
chance: 5.0
rarity: legendary
display:
name: "&6Lingote de Netherite"
lore:
- "&7Um material extremamente raro e resistente."
- "&7Perfeito para forjar equipamentos finais."
icon:
item: "NETHERITE_INGOT"
glow: false
commands:
- "give {player} minecraft:netherite_ingot 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

enchanted_golden_apple:
chance: 1.0
rarity: legendary
display:
name: "&5Maçã Dourada Encantada"
lore:
- "&7O item mais poderoso para emergências."
- "&7Proteção e regeneração instantâneas."
icon:
item: "ENCHANTED_GOLDEN_APPLE"
glow: true
commands:
- "give {player} minecraft:enchanted_golden_apple 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

elytra_wings:
chance: 3.0
rarity: epic
display:
name: "&bElytra"
lore:
- "&7Asas para voar pelos céus do mundo."
- "&7Use com cuidado — o céu é o limite."
icon:
item: "ELYTRA"
glow: false
commands:
- "give {player} minecraft:elytra 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

totem_of_undying:
chance: 4.0
rarity: epic
display:
name: "&eTotem da Imortalidade"
lore:
- "&7Salva o jogador de uma morte certa."
- "&7Um item heroico para momentos críticos."
icon:
item: "TOTEM_OF_UNDYING"
glow: true
commands:
- "give {player} minecraft:totem_of_undying 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

dragon_egg:
chance: 0.5
rarity: legendary
display:
name: "&cOvo do Ender Dragon"
lore:
- "&7Um troféu único — raríssimo."
- "&7Ótimo para quem quer ostentar no servidor."
icon:
item: "DRAGON_EGG"
glow: false
commands:
- "give {player} minecraft:dragon_egg 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

nether_star:
chance: 2.0
rarity: epic
display:
name: "&fEstrela do Nether"
lore:
- "&7Usada para construir beacons poderosos."
- "&7Perfeita para obras de alto nível."
icon:
item: "NETHER_STAR"
glow: true
commands:
- "give {player} minecraft:nether_star 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

beacon_block:
chance: 1.5
rarity: rare
display:
name: "&bBeacon"
lore:
- "&7Um bloco que concede efeitos mediante estrutura."
- "&7Ótimo para bases e áreas comunitárias."
icon:
item: "BEACON"
glow: false
commands:
- "give {player} minecraft:beacon 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

diamond_bundle:
chance: 10.0
rarity: rare
display:
name: "&bDiamantes x16"
lore:
- "&7Um bom pacote de diamantes para upgrade."
- "&716 unidades — ótimo para forjas e trocas."
icon:
item: "DIAMOND"
glow: false
commands:
- "give {player} minecraft:diamond 16"
broadcast:
enable: false
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""

shulker_box_purple:
chance: 6.0
rarity: uncommon
display:
name: "&5Shulker Box Roxa"
lore:
- "&7Caixa prática para armazenamento móvel."
- "&7Ótima para aventuras longas."
icon:
item: "PURPLE_SHULKER_BOX"
glow: false
commands:
- "give {player} minecraft:purple_shulker_box 1"
broadcast:
enable: true
message:
- ""
- "&7[&6%box_name%&7] &fO jogador &7%player_displayname% &facabou de ganhar:"
- "&f- &a%prize_name% &fde raridade &a%rarity_displayname%"
- ""
</code-block>
</chapter>
</chapter>
<chapter title="settings/" collapsible="true">
<chapter title="commands.yml" collapsible="true">
<code-block lang="yaml">
# É necessário reiniciar o servidor após a alteração
givebox:
  name: givebox
  use-command: true
  permission: leafmysterybox.command.givebox
  aliases:
    - darcaixa

removebox:
name: removebox
use-command: true
permission: leafmysterybox.command.removebox
aliases:
- removercaixa

givekey:
name: givekey
use-command: true
permission: leafmysterybox.command.givekey
aliases:
- darchave

editboxes:
name: editboxes
use-command: true
permission: leafmysterybox.admin
aliases:
- editarcaixas
</code-block>
</chapter>
</chapter>
<chapter title="boxes.yml" collapsible="true">
<code-block lang="yaml">
padrao:
  # Nome do tipo de caixa
  name: "&5&lCaixa Padrão"

# Arquivo de recompensas (/plugins/LeafMysteryBox/rewards/)
prizes: "caixa-padrao.yml"

# [Premium] Animação ao abrir a caixa
# Deixe '0' para não usar animação
# Confira a lista de animações em https://leafplugins.com/plugin/LeafMysteryBox
animation: 1

# Chave para abrir a caixa
key:
# Nome do item
name: "%box_name%"

    # Tipo do item (Material)
    item: "TRIPWIRE_HOOK"

    # Descrição do item
    lore:
      - ""
      - "&7Use esta chave para abrir"
      - "&7uma caixa misteriosa do tipo"
      - ""
      - "&eUse o botão direito na caixa"

# Usar holograma customizado ao em vez da config.yml
holograms:
prize:
height: 0.5
lines:
1:
# Caso haja mais de um nesta lista, fará uma linha animada
frames:
- '&f« &5&lCAIXA PADRÃO &f»'
- '&f« &f&lCAIXA PADRÃO &f»'
- '&f« &5&lC&f&lAIXA PADRÃO &f»'
- "&f« &5&lCA&f&lIXA PADRÃO &f»"
- "&f« &5&lCAI&f&lXA PADRÃO &f»"
- "&f« &5&lCAIX&f&lA PADRÃO &f»"
- "&f« &5&lCAIXA &f&lPADRÃO &f»"
- "&f« &5&lCAIXA P&f&lADRÃO &f»"
- "&f« &5&lCAIXA PA&f&lDRÃO &f»"
- "&f« &5&lCAIXA PAD&f&lRÃO &f»"
- "&f« &5&lCAIXA PADA&f&lRÃO &f»"
- "&f« &5&lCAIXA PADR&f&lÃO &f»"
- "&f« &5&lCAIXA PADRA&f&lO &f»"
- "&f« &5&lCAIXA PADRÃO &f»"
- "&f« &f&lCAIXA PADRÃO &f»"
# Intervalo para mudar de frame (0.1 minimo para animações)
interval: 0.1
2:
frames:
- '&a%player_displayname% &fɢᴀɴʜᴏᴜ ᴀʟɢᴏ &b%prize_rarity%'
interval: 0.1
3:
frames:
- '&fᴘʀêᴍɪᴏ: &a%prize_name%'
interval: 0.1
display:
height: 0.5
lines:
1:
# Caso haja mais de um nesta lista, fará uma linha animada
frames:
- '&f« &f&lCAIXA PADRÃO &f»'
- '&f« &f&lCAIXA PADRÃO &f»'
- '&f« &f&lCAIXA PADRÃO &f»'
- '&f« &e&lCAIXA PADRÃO &f»'
- '&f« &b&lCAIXA PADRÃO &f»'
- '&f« &a&lCAIXA PADRÃO &f»'
- '&f« &5&lCAIXA PADRÃO &f»'
- '&f« &f&lCAIXA PADRÃO &f»'
- '&f« &5&lC&f&lAIXA PADRÃO &f»'
- "&f« &5&lCA&f&lIXA PADRÃO &f»"
- "&f« &5&lCAI&f&lXA PADRÃO &f»"
- "&f« &5&lCAIX&f&lA PADRÃO &f»"
- "&f« &5&lCAIXA &f&lPADRÃO &f»"
- "&f« &5&lCAIXA P&f&lADRÃO &f»"
- "&f« &5&lCAIXA PA&f&lDRÃO &f»"
- "&f« &5&lCAIXA PAD&f&lRÃO &f»"
- "&f« &5&lCAIXA PAD&f&lRÃO &f»"
- "&f« &5&lCAIXA PADR&f&lÃO &f»"
- "&f« &5&lCAIXA PADRÃ&f&lO &f»"
- "&f« &5&lCAIXA PADRÃO &f»"
- "&f« &f&lCAIXA PADRÃO &f»"

            # Intervalo para mudar de frame (0.1 minimo para animações)
          interval: 0.2
        2:
          frames:
            - '<when var="%boxes%" equals="0" then="&c&lVOCÊ NÃO POSSUI CAIXAS" else="&fᴠᴏᴄê ᴘᴏꜱꜱᴜɪ &a%boxes% ᴄᴀɪxᴀꜱ &fᴅɪꜱᴘᴏɴíᴠᴇɪꜱ"></when>'
            - '<when var="%boxes%" equals="0" then="&c&lVOCÊ NÃO POSSUI CAIXAS" else="&fᴠᴏᴄê ᴘᴏꜱꜱᴜɪ &b%boxes% ᴄᴀɪxᴀꜱ &fᴅɪꜱᴘᴏɴíᴠᴇɪꜱ"></when>'
            - '<when var="%boxes%" equals="0" then="&c&lVOCÊ NÃO POSSUI CAIXAS" else="&fᴠᴏᴄê ᴘᴏꜱꜱᴜɪ &d%boxes% ᴄᴀɪxᴀꜱ &fᴅɪꜱᴘᴏɴíᴠᴇɪꜱ"></when>'
            - '<when var="%boxes%" equals="0" then="&c&lVOCÊ NÃO POSSUI CAIXAS" else="&fᴠᴏᴄê ᴘᴏꜱꜱᴜɪ &e%boxes% ᴄᴀɪxᴀꜱ &fᴅɪꜱᴘᴏɴíᴠᴇɪꜱ"></when>'
          interval: 0.1
        3:
          frames:
            - ''
          interval: 1
        4:
          frames:
            - '&eʙᴏᴛãᴏ ᴅɪʀᴇɪᴛᴏ &fᴘᴀʀᴀ &aᴀʙʀɪʀ'
            - '&eꜱʜɪꜰᴛ &f+ &eʙᴏᴛãᴏ ᴅɪʀᴇɪᴛᴏ &fᴘᴀʀᴀ &bᴀʙʀɪʀ ɪɴꜱᴛᴀɴᴛâɴᴇᴏ'
          interval: 5
        5:
          frames:
            - '&eʙᴏᴛãᴏ ᴇꜱꞯᴜᴇʀᴅᴏ &fᴘᴀʀᴀ &dɪɴꜱᴘᴇᴄɪᴏɴᴀʀ'
          interval: 1

avancada:
name: "&6&lCaixa Avançada"
prizes: "caixa-avancada.yml"
animation: 1
key:
name: "%box_name%"
item: "TRIPWIRE_HOOK"
lore:
- ""
- "&7Use esta chave para abrir"
- "&7uma caixa misteriosa do tipo"
- ""
- "&eUse o botão direito na caixa"
holograms:
prize:
height: 0.5
lines:
1:
# Caso haja mais de um nesta lista, fará uma linha animada
frames:
- "&f⚡ &6&lCAIXA AVANÇADA &f⚡"
- "&f⚡ &f&lCAIXA AVANÇADA &f⚡"
- "&f⚡ &6&lC&f&lAIXA AVANÇADA &f⚡"
- "&f⚡ &6&lCA&f&lIXA AVANÇADA &f⚡"
- "&f⚡ &6&lCAI&f&lXA AVANÇADA &f⚡"
- "&f⚡ &6&lCAIX&f&lA AVANÇADA &f⚡"
- "&f⚡ &6&lCAIXA &f&lAVANÇADA &f⚡"
- "&f⚡ &6&lCAIXA A&f&lVANÇADA &f⚡"
- "&f⚡ &6&lCAIXA AV&f&lANÇADA &f⚡"
- "&f⚡ &6&lCAIXA AVA&f&lNÇADA &f⚡"
- "&f⚡ &6&lCAIXA AVAN&f&lÇADA &f⚡"
- "&f⚡ &6&lCAIXA AVANÇ&f&lADA &f⚡"
- "&f⚡ &6&lCAIXA AVANÇA&f&lDA &f⚡"
- "&f⚡ &6&lCAIXA AVANÇAD&f&lA &f⚡"
- "&f⚡ &6&lCAIXA AVANÇADA &f⚡"
- "&f⚡ &f&lCAIXA AVANÇADA &f⚡"
interval: 0.1
2:
frames:
- '&a%player_displayname% &fɢᴀɴʜᴏᴜ ᴀʟɢᴏ &b%prize_rarity%'
interval: 0.1
3:
frames:
- '&fᴘʀêᴍɪᴏ: &a%prize_name%'
interval: 0.1
display:
height: 1
lines:
1:
# Caso haja mais de um nesta lista, fará uma linha animada
frames:
- "&f⚡ &6&lCAIXA AVANÇADA &f⚡"
- "&f⚡ &f&lCAIXA AVANÇADA &f⚡"
- "&f⚡ &6&lC&f&lAIXA AVANÇADA &f⚡"
- "&f⚡ &6&lCA&f&lIXA AVANÇADA &f⚡"
- "&f⚡ &6&lCAI&f&lXA AVANÇADA &f⚡"
- "&f⚡ &6&lCAIX&f&lA AVANÇADA &f⚡"
- "&f⚡ &6&lCAIXA &f&lAVANÇADA &f⚡"
- "&f⚡ &6&lCAIXA A&f&lVANÇADA &f⚡"
- "&f⚡ &6&lCAIXA AV&f&lANÇADA &f⚡"
- "&f⚡ &6&lCAIXA AVA&f&lNÇADA &f⚡"
- "&f⚡ &6&lCAIXA AVAN&f&lÇADA &f⚡"
- "&f⚡ &6&lCAIXA AVANÇ&f&lADA &f⚡"
- "&f⚡ &6&lCAIXA AVANÇA&f&lDA &f⚡"
- "&f⚡ &6&lCAIXA AVANÇAD&f&lA &f⚡"
- "&f⚡ &6&lCAIXA AVANÇADA &f⚡"
- "&f⚡ &f&lCAIXA AVANÇADA &f⚡"
interval: 0.2
2:
frames:
- '&e&lNOVOS PRÊMIOS TODA SEMANA!'
- '&b&lNOVOS PRÊMIOS TODA SEMANA!'
- '&a&lNOVOS PRÊMIOS TODA SEMANA!'
- '&d&lNOVOS PRÊMIOS TODA SEMANA!'
interval: 0.1
3:
frames:
- ''
interval: 1
4:
frames:
- '<when var="%boxes%" equals="0" then="&c&lVOCÊ NÃO POSSUI CAIXAS" else="&fᴠᴏᴄê ᴘᴏꜱꜱᴜɪ &a%boxes% ᴄᴀɪxᴀꜱ &fᴅɪꜱᴘᴏɴíᴠᴇɪꜱ"></when>'
- '<when var="%boxes%" equals="0" then="&c&lVOCÊ NÃO POSSUI CAIXAS" else="&fᴠᴏᴄê ᴘᴏꜱꜱᴜɪ &b%boxes% ᴄᴀɪxᴀꜱ &fᴅɪꜱᴘᴏɴíᴠᴇɪꜱ"></when>'
- '<when var="%boxes%" equals="0" then="&c&lVOCÊ NÃO POSSUI CAIXAS" else="&fᴠᴏᴄê ᴘᴏꜱꜱᴜɪ &d%boxes% ᴄᴀɪxᴀꜱ &fᴅɪꜱᴘᴏɴíᴠᴇɪꜱ"></when>'
- '<when var="%boxes%" equals="0" then="&c&lVOCÊ NÃO POSSUI CAIXAS" else="&fᴠᴏᴄê ᴘᴏꜱꜱᴜɪ &e%boxes% ᴄᴀɪxᴀꜱ &fᴅɪꜱᴘᴏɴíᴠᴇɪꜱ"></when>'
interval: 1
5:
frames:
- ''
interval: 1
6:
frames:
- '&eʙᴏᴛãᴏ ᴅɪʀᴇɪᴛᴏ &fᴘᴀʀᴀ &aᴀʙʀɪʀ'
- '&eꜱʜɪꜰᴛ &f+ &eʙᴏᴛãᴏ ᴅɪʀᴇɪᴛᴏ &fᴘᴀʀᴀ &bᴀʙʀɪʀ ɪɴꜱᴛᴀɴᴛâɴᴇᴏ'
interval: 5
7:
frames:
- '&eʙᴏᴛãᴏ ᴇꜱꞯᴜᴇʀᴅᴏ &fᴘᴀʀᴀ &dɪɴꜱᴘᴇᴄɪᴏɴᴀʀ'
interval: 1
</code-block>
</chapter>
<chapter title="config.yml" collapsible="true">
<code-block lang="yaml">
# Agradecemos por escolher o LeafMysteryBox ♥
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

options:
# Usará o sistema de chaves para abrir caixas
use-keys: true

# Anunciará prêmios com broadcast
# ==> 'true' Anunciará para todos os jogadores do servidor
# ==> 'false' Anunciará apenas para jogadores no mesmo mundo
broadcast-all: false

# Quantidade máxima de caixas que podem ser abertas ao mesmo tempo por um jogador
max-opening-boxes: 1

# Fará com que as animações sejam individuais para cada jogador
individual-opening: true

# Permitir que caixas sejam abertas instantaneamente (sem animação)
allow-open-instantly: true
</code-block>
</chapter>
<chapter title="rarities.yml" collapsible="true">
<code-block lang="yaml">
common:
  name: "Comum"
  color: "&7"
  displayName: "&7&lCOMUM"

rare:
name: "Raro"
color: "&9"
displayName: "&9&lRARO"

epic:
name: "Épico"
color: "&b"
displayName: "&b&lÉPICO"

legendary:
name: "Lendário"
color: "&6"
displayName: "&6&lLENDÁRIO"

uncommon:
name: "Incomum"
color: "&5&l"
displayName: "&f&l&kI &5&lINCOMUM &f&l&kI"
</code-block>
</chapter>
</chapter>