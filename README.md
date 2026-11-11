# Mo Town

A small desktop browser game about Mo, a Bernese mountain dog with a cheese problem and a grudge against the post.

## Play

Double-click `index.html`. No install, no build, no internet needed.

| Key | What it does |
| --- | --- |
| Arrow keys / WASD | Run about the park |
| Space | Bark (stuns postmen, scatters pigeons) |
| P | Pause |
| M, or the speaker button (bottom right) | Sound on / off |

## How it works

- **Postmen** walk in from the sides and try to reach a letterbox. Bark to stun one, then charge into him to bowl him over. Run into an un-stunned postman and you get a thwack from his newspaper. Five letters delivered and it is game over.
- **Cheese** fills the Gut-o-meter. The fifth wedge sets off the **Turbo Trots**: rocket speed, double points, and a trail that postmen slip on. Afterwards Mo is queasy for a few seconds: slow, no barking, no cheese. So choose your moment for that fifth wedge.
- **Pigeons** land in flocks and scoff your cheese. Chase them off for points; clear a whole flock quickly for a bonus. A pigeon taking off next to a postman stuns him.

## Tweaking

Everything is in `index.html`. The `CFG` block near the top holds the balance numbers (speeds, timings, how many cheeses trigger the trots, how many letters end the game).
