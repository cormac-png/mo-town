# Mo Town

A small desktop browser game about Mo, a Bernese mountain dog with a cheese problem and a grudge against the post.

## Play

Play online at https://cormac-png.github.io/mo-town/

Or download the repo and double-click `index.html`. No install or build needed. Keep the `sounds` folder next to it. Opened straight from disk, some browsers will not load the recordings, and the game uses built-in synthesised sounds instead.

| Key | What it does |
| --- | --- |
| Arrow keys / WASD | Run about the park |
| Space | Bark (stuns postmen, scatters pigeons) |
| P | Pause |
| M, or the speaker button (bottom right) | Sound on / off |

On a phone or tablet: drag anywhere on the left half of the screen to run, tap anywhere on the right half to bark. Small buttons above the WOOF button pause the game and switch the sound on or off. It plays best with the phone held sideways.

## How it works

- **Postmen** walk in from the sides and try to reach a letterbox. Bark to stun one, then charge into him to bowl him over. Run into an un-stunned postman and you get a thwack from his newspaper. Five letters delivered and it is game over.
- **Cheese** fills the Gut-o-meter. The fifth wedge sets off the **Turbo Trots**: rocket speed, double points, and a trail that postmen slip on. Afterwards Mo is queasy for a few seconds: slow, no barking, no cheese. So choose your moment for that fifth wedge.
- **Pigeons** land in flocks and scoff your cheese. Chase them off for points; clear a whole flock quickly for a bonus. A pigeon taking off next to a postman stuns him.

## Tweaking

Everything is in `index.html`. The `CFG` block near the top holds the balance numbers (speeds, timings, how many cheeses trigger the trots, how many letters end the game).

## Sounds

Recordings live in `sounds/`. Each is optional; delete one and the game falls back to a synthesised version.

| File | Plays when |
| --- | --- |
| `bark.mp3` | Mo barks (Space) |
| `scream.mp3` | A postman is bowled over |
| `powerup.mp3` | The Turbo Trots start |
| `farts.mp3` | Six sounds in one file: the big one at the start of the Turbo Trots, the small ones while it lasts |

To swap one, replace the file and keep the name. If you replace `farts.mp3`, update the `FARTS` timings near the top of the sound code in `index.html`.

`farts.mp3` and `powerup.mp3` are from Epidemic Sound and are used under licence; they are not free to reuse.
