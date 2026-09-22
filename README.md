# cricket-social (hop 3)

Social posts. **Three hops** from `cricket-protocol`. **One hop** from `cricket-highlights`.

```
protocol → scoring → highlights → social
```

Posts `WICKET` only when highlights says `{ clip: true, kind: "wicket" }`. Does not know `BallEvent` or `umpire_confirmed`.

A protocol default that makes scoring count an unconfirmed LBW becomes a public WICKET post in this repo without this file changing.

## Trap branch

`trap/post-appeals` — also post `WICKET` when `kind === "appeal"` so the timeline feels live. Tests stay green. Failed LBWs trend as wickets.

## Develop

```bash
npm test
```
