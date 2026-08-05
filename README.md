# Arms of God — Weapon DPS Dataset

Reverse-engineered weapon DPS data from the Arms of God Early Access build (June 2026, Dark Jay Studio). Includes single-target boss DPS, AoE effective DPS, and sustained DPS metrics for 16 weapons.

## Data Format (`weapons-dps.json`)

Each weapon entry includes:
- `name` — Weapon name
- `tier` — S, A, or T3
- `type` — Damage type + melee/ranged
- `base_dmg` — Raw damage from stat card
- `attack_speed` — Attacks per second
- `raw_dps` — Base damage × attack speed
- `passive_multiplier` — Passive ability multiplier
- `effective_boss_dps` — Final DPS vs single target
- `effective_aoe_dps` — Final DPS vs 20 enemies (where applicable)

## Methodology

```
effective DPS = base_damage × attack_speed × passive_multiplier
```

Boss DPS assumes 60-second fight with optimal blessing setup. AoE DPS assumes 20 enemies on screen.

## Live Site

[armsofgodgame.com — Weapon DPS Comparison](https://armsofgodgame.com/guides/arms-of-god-weapon-dps-comparison)

## License

Data: CC BY 4.0 | Code: MIT
