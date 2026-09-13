# Klaus — Codex Pet Superman

<p align="center">
  <img src="images/idle.gif" width="192" height="208" alt="Klaus idle animation">
</p>

<p align="center">
  <strong>Your Superman! 💪🏻</strong><br>
  Calm confidence, sharp focus, and a warm protective spirit.
</p>

Klaus is a custom animated pet for Codex. He stays calm while you think, gets moving when work begins, and brings a little superhero energy to every task.

## Costume collection

The same Klaus, with his black hair, beard, and powerful bodybuilder physique, in three additional outfits. Each outfit is a separate Codex Pet v2 package with nine animations and sixteen look directions.

<table align="center">
  <tr>
    <td align="center"><img src="pets/klaus-fitness/images/idle.gif" width="192" height="208" alt="Muscular shirtless Klaus in athletic shorts"><br><strong>健身休闲 · Fitness</strong><br>Bare chest, athletic shorts, and trainers.</td>
    <td align="center"><img src="pets/klaus-suit/images/idle.gif" width="192" height="208" alt="Muscular Klaus in a tailored navy suit"><br><strong>西装革履 · Suit</strong><br>Tailored navy suit, white shirt, and tie.</td>
    <td align="center"><img src="pets/klaus-beach/images/idle.gif" width="192" height="208" alt="Muscular Klaus wearing an open tropical shirt and beach shorts"><br><strong>海滩度假 · Beach</strong><br>Open tropical shirt, beach shorts, and sandals.</td>
  </tr>
</table>

Packages: [Fitness](pets/klaus-fitness/), [Suit](pets/klaus-suit/), [Beach](pets/klaus-beach/). Each includes animation previews and a labeled contact sheet for inspection.

## Animations

<table align="center">
  <tr>
    <td align="center"><img src="images/waving.gif" width="160" alt="Klaus waving"><br><strong>Waving</strong></td>
    <td align="center"><img src="images/jumping.gif" width="160" alt="Klaus jumping"><br><strong>Jumping</strong></td>
    <td align="center"><img src="images/waiting.gif" width="160" alt="Klaus waiting"><br><strong>Waiting</strong></td>
  </tr>
  <tr>
    <td align="center"><img src="images/running.gif" width="160" alt="Klaus standing and curling two dumbbells"><br><strong>Working</strong></td>
    <td align="center"><img src="images/review.gif" width="160" alt="Klaus wearing reading glasses and reading an open book"><br><strong>Reviewing</strong></td>
    <td align="center"><img src="images/failed.gif" width="160" alt="Klaus reacting to a failure"><br><strong>Oops!</strong></td>
  </tr>
</table>

### On the move

<p align="center">
  <img src="images/running-right.gif" width="192" alt="Klaus running right">
  <img src="images/running-left.gif" width="192" alt="Klaus running left">
</p>

## Install

Clone this repository into your Codex pets directory:

```bash
git clone git@github.com:Bosn/CodexPetSuperman.git ~/.codex/pets/klaus
```

If the directory already exists, update it instead:

```bash
cd ~/.codex/pets/klaus
git pull
```

Then restart Codex if Klaus does not appear immediately.

### Install the three additional outfits

From this repository, copy the three packages into your Codex pets directory:

```bash
mkdir -p ~/.codex/pets
for pet in klaus-fitness klaus-suit klaus-beach; do
  if [ -e "$HOME/.codex/pets/$pet" ]; then
    echo "Already installed; skipped: $pet"
  else
    cp -R "pets/$pet" "$HOME/.codex/pets/$pet"
  fi
done
```

Each appears separately in the pet picker under its Chinese outfit name. Restart Codex if the new entries do not appear immediately.

## Pet package

- `pet.json` — pet identity and Codex sprite configuration
- `spritesheet.webp` — complete v2 animation atlas
- `images/` — GIF previews used by this README
- `pets/klaus-{fitness,suit,beach}/` — additional outfits, each with its own manifest, atlas, previews, and QA artifacts

Klaus uses the Codex Pet v2 spritesheet format.
