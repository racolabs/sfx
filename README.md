# Raco Labs SFX

Pacote de efeitos sonoros **CC0** (domínio público) da Raco Labs, nascido no jogo *Sobrecarga* e usado também em *Em Produção*.
169 arquivos `.ogg` (1,9 MB): tiros e recargas de 12 armas, faca por superfície, passos, quedas, explosões, fumaça, clarão,
habilidades, pings, interface (moedas, recusa), rádio e ambiente (gaivotas, apito de navio).

A Raco Labs's CC0 sound effects pack, born in the game *Sobrecarga* and also used in *Em Produção*.
169 `.ogg` files (1.9 MB): gunshots and reloads for 12 weapons, knife hits by surface, footsteps, falls, explosions, smoke,
flashbang, abilities, pings, UI (coins, deny), radio and ambience.

## Licença / License

Tudo aqui é **CC0 1.0**: use, mude e venda sem pedir licença e sem dar crédito. Os autores originais estão em
[CREDITS.md](CREDITS.md), por gentileza (não é obrigação).
Everything here is **CC0 1.0**: use, modify and sell with no permission and no attribution required. Original authors
are listed in [CREDITS.md](CREDITS.md) as a courtesy.

## Como usar / Usage

- `audio/<pasta>/<nome>.ogg`: mono, curtos, já cortados e com o volume igualado.
- Variações de um som se chamam `nome-0`, `nome-1`...; sorteie uma a cada vez para não soar repetido.
- `audio/sons.json` agrupa os sons por categoria (`tiro`, `info`, `nucleo`, `interface`, `habilidade`, `ambiente`) e diz o que baixar antes.
- Safari/iOS antigos não tocam OGG: converta com `ffmpeg -i in.ogg -ac 1 -c:a aac -b:a 64k out.m4a` (foi o que o Em Produção fez).

Variations of one sound are `name-0`, `name-1`...; pick one at random. `audio/sons.json` groups the sounds by category and lists what to preload. Older Safari/iOS cannot play OGG: convert with the `ffmpeg` line above.

## Pastas / Folders

| Pasta | O que tem |
|---|---|
| `armas/` | tiro de perto e de longe de 12 armas |
| `arma/<conjunto>/` | pente sai, pente entra, ferrolho, saque e clique sem bala |
| `recarga/`, `troca/` | recarga e troca de arma genéricas |
| `faca/` | corte no ar, acerto em corpo, madeira, metal, concreto e risca |
| `acerto/`, `dano/`, `impacto/` | acerto no corpo, levar tiro, arma e bala batendo |
| `passos-*`, `queda*`, `pouso-*`, `quique/` | passos, quedas e pousos, quique por material |
| `explosao/`, `hab/`, `spray/` | explosões, fumaça, clarão, vidro, fogo, muralha, lata de spray |
| `nucleo/` | pegar, travar, tampar, ferramenta, desarmar, explosão grande |
| `ping/`, `radio/`, `interface/` | pings por tipo, chiado de rádio, moedas e recusa |
| `amb/` | gaivotas, apito de navio |

Sons sintetizados (bipes de menu etc.) vivem no código dos jogos, não neste pacote.
