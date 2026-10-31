# Lastro — sprites pixel v2

Arte original construída em grade inteira por PixelCharacterArt.ts. Não usa a ilustração de concept como recorte nem sprites de jogos existentes. Não foi gerada por ImageGen: é arte raster definida em código, com quadros pré-renderizados em PNG + atlas JSON.

Protagonista, rusher e gunner: 91 entradas de animação por personagem. Algumas poses sustentadas compartilham o mesmo desenho. Células transparentes 112×112; pivô dos pés (48,80); 8 colunas; atlas 896×1344. A figura ocupa aproximadamente 44 pixels de altura em pé. Nenhum redimensionamento variável entre frames.

Clips: idle, run, walk, jump, fall, land, crouch, dash, aim, shoot, reload, hurt, defeat, guard, throw, wall, slow e preparação/corte/recuperação dos três golpes. Estados especiais reaproveitam o clip mais próximo. O híbrido usa o visual do rusher. Defensor, miniboss e boss conservam o renderer anterior.

Os tempos de ataque, controles, física, dano e colisões permanecem no código de gameplay existente. O renderer só seleciona os quadros e desenha rastros/clarões. Efeitos de impacto continuam nos sistemas existentes.

Gerar novamente: node --experimental-strip-types scripts/build-pixel-characters.mts

Prévia animada: /qa/character-preview.html

Validação automática: alpha binário, dimensões fixas, margem livre em todos os quadros e contato dos pés nos ciclos de corrida/caminhada. Revisão visual no navegador necessária ao mudar a arte.
