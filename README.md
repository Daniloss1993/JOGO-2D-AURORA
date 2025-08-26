# Aurora Steps — Plataforma 2D (Unity)

## Visão Geral

Plataforma 2D com movimento fluido (andar, correr, pular, escalar) em 3 a 5 fases curtas e progressivas. Colete cristais, evite perigos e alcance o portal final em cada nível. Arte estilizada com parallax, HUD minimalista e feedback audiovisual claro.

## Objetivo

Desenvolver um jogo de plataforma em 2D na Unity como peça de portfólio, demonstrando domínio da engine, programação em C#, design de níveis, feedback ao jogador, animação, áudio e empacotamento.

## Mecânicas

* Movimento: andar, correr, pular com coyote time e jump buffer.
* Escalada: ladders/escadas com gravidade desativada.
* Coletáveis: cristais com feedback sonoro e visual.
* Inimigos: patrulha com dano.
* Plataformas móveis e checkpoints.

## Conteúdo

* **Nível 1:** fundamentos (movimento, pulo, coleta).
* **Nível 2:** plataformas móveis e primeiros inimigos.
* **Nível 3:** verticalidade com escadas e perigos.
* **Nível 4 (opcional):** combinação de mecânicas.
* **Nível 5 (opcional):** desafio final.

## HUD

* Contador de vidas e cristais.
* Nome do nível.
* Mensagens rápidas (checkpoint, game over).

## Arte e Áudio

* Sprites autorais ou gratuitos (Kenney, Itch.io, OpenGameArt).
* Animações: Idle, Run, Jump, Fall, Climb, Hurt.
* SFX: pulo, coleta, dano, portal.
* BGM leve por nível.

## Estrutura do Projeto

```
Assets/
  Art/
  Audio/
  Materials/
  Prefabs/
  Scenes/
    Level_01.unity
    Level_02.unity
    Level_03.unity
  Scripts/
    PlayerController2D.cs
    EnemyPatrol.cs
    Collectible.cs
    GameManager.cs
    HUDController.cs
```

## Scripts Base

* **PlayerController2D.cs:** movimentação (andar, correr, pulo com coyote time e jump buffer, escada).
* **Collectible.cs:** coleta de cristais.
* **Damageable.cs:** sistema de vidas.
* **EnemyPatrol.cs:** inimigos patrulheiros.
* **PlatformMover.cs:** plataformas móveis.
* **HUDController.cs:** interface de vidas e cristais.
* **GameManager.cs:** lógica geral (vidas, níveis).
* **LevelExit.cs:** portal de saída.
* **AudioManager.cs:** efeitos sonoros globais.
* **Checkpoint.cs / PlayerRespawn.cs:** pontos de respawn.

## Controles

* **Mover:** A/D ou ←/→
* **Correr:** Shift
* **Pular:** Espaço
* **Subir/Descer:** W/S

## Build e Entrega

1. **Adicionar cenas** no Build Settings (Menu, Level\_01, Level\_02, Level\_03, GameOver).
2. **Exportar Build** para Windows x64 ou WebGL.
3. Compactar pasta Build e subir no GitHub.

## Estrutura do Repositório

```
/ (root)
  ├─ Assets/
  ├─ Packages/
  ├─ ProjectSettings/
  ├─ .gitignore
  ├─ README.md
  └─ LICENSE
```

**.gitignore essencial:**

```
[Ll]ibrary/
[Tt]emp/
[Bb]uilds?/
[Ll]ogs/
[Oo]bj/
[Mm]emoryCaptures/
UserSettings/
```

## Links Úteis

* [Unity Learn](https://unity.com/pt/learn/get-started)
* [YouTube: Plataforma 2D Unity](https://www.youtube.com/watch?v=dwcT-Dch0bA&t)
* [Tutorial Unity (Sentry)](https://blog.sentry.io/unity-tutorial-developing-your-first-unity-game-part-1/)

## Licença

MIT (pode adaptar conforme necessidade).
