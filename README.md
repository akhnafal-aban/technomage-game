# TechnoMage — Platform Shooting Game

2D platform shooter built with Unity 6 (6000.0.22f1), C#, and the new Input System. Play a mage that runs, jumps, and shoots projectiles through a tiled map; hits apply knockback, and the player has a health/life system.

This is the finished version of the project — the gameplay loop, audio manager, and both the primitive mage ("PrimitifMage") and the animated "Zera" character sets (idle, walk, jump, melee, range, attack animations) are in `Assets/`.

## What's implemented

- **Player controller** — run/jump using `PlayerController.cs` + Input System action maps
- **Shooting** — `PlayerAttack.cs` fires `Projectile.cs` from a shooting point with a cooldown
- **Combat feel** — `Knockback.cs`, `PlayerLife.cs` (health/lives)
- **Audio** — `AudioManager.cs` with sound effects (`AudioFX/`)
- **Two character sets** — primitive mage and the animated Zera sprite set
- **Single scene** — `Assets/Scenes/Game.unity`

## Running it

1. Open the project folder in Unity 6 (6000.0.22f1 or compatible)
2. Open `Assets/Scenes/Game.unity`
3. Press Play

## Project layout

```
Assets/
  Script/        PlayerController, PlayerAttack, PlayerLife, Projectile, Knockback, AudioManager
  Scenes/        Game.unity
  Map/           tile map art
  Prefab/        projectile + circle prefabs
  PrimitifMage/  primitive character + animations (mageIdle, mageJump, mageFall, mageMelee)
  Modern/        Zera character animations (idle, walk, jump, attack)
  AudioFX/       sound effects
```

## Tech

Unity 6, C#, Input System.
