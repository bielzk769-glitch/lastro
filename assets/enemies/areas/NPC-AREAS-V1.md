# NPCs das cinco áreas — v1

Modo de criação: ferramenta integrada de geração de imagens. O protagonista preto, branco e vermelho foi usado apenas como referência de densidade de pixel, anatomia e acabamento; seus traços e sua paleta não foram copiados.

## Prompt comum

Folha de concepts em pixel art para jogo indie 2D de ação rápida. Grade exata 2×2, quatro personagens humanos completos em vista lateral, fundo alfa transparente, mesma escala e linha dos pés. Pixel clusters nítidos, anatomia com volume, streetwear cyberpunk ligado ao trabalho de cada área. Cada classe precisa diferir por silhueta, postura, arma e blocos de cor. Sem robôs, ternos sociais, soldados genéricos, logos, texto, cenário, cortes ou sobreposição entre células.

## Área 1 — Mercado de Chuva

Átrio corporativo convertido em mercado molhado. Paleta teal petróleo, prata, âmbar e grafite. Personagens: courier com cutelo elétrico, lookout de capa transparente e rifle, flanker com lâminas curvas e capitão com escudo dobrável.

## Área 2 — Trânsito da Fundição

Esteiras, guindastes, fornalhas e trilhos. Paleta fuligem, ferrugem, latão e aço. Personagens: brawler com martelo térmico, técnica com rifle de rebites, armadilheiro com mina triangular e capataz com bate-estaca.

## Área 3 — Laboratórios Bioglass

Contenção e cirurgia abandonadas. Paleta branco frio, menta, ultravioleta e grafite. Personagens: capturador com bastão bifurcado, pesquisadora com rifle de ampola, controladora com injetores por cabo e warden com pinça energética.

## Área 4 — Poço de Energia

Elevadores, turbinas, pontes e canais de wall-jump. Paleta azul-marinho, cobalto, amarelo de segurança e alumínio. Personagens: escaladora com lâminas-garra, sniper de arpão, perseguidor com boleadeiras elétricas e sentinela com lança e escudo.

## Área 5 — Reator da Coroa

Cobertura executiva em ruínas ao redor do reator. Paleta obsidiana, porcelana, ouro-champagne e pequenos núcleos carmesim. Personagens: duelista de sabre, railgunner com manto, caçador de lâminas crescentes e executor final com gunblade.

## Integração de gameplay

As cinco folhas são carregadas como spritesheets 2×2. Nos encontros comuns, a função determina a célula: rusher 0, gunner 1, hybrid 2 e defender 3. O miniboss usa a elite da Área 4 e o boss final usa o Executor da Área 5. O movimento é aplicado pelo `AreaNPCVisual` com inclinação, compressão, salto, recuo, queda, flashes e efeitos de ataque, preservando integralmente IA, hitboxes, dano e temporização do combate existente.
