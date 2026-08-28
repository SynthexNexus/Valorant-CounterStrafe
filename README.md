## 📖 Overview

In tactical first-person shooters like **VALORANT**, gun accuracy is heavily tied to player movement. Firing while moving introduces severe bullet inaccuracy (Movement Error). To achieve instant first-bullet accuracy, players must **Counter-Strafe**—pressing the opposite direction key the exact microsecond they release the primary movement key to instantly halt momentum.

**Valorant-CounterStrafe** is an input-optimization utility that monitors directional key states (`W`, `A`, `S`, `D`) and intelligently executes instantaneous counter-pulses upon key release. This drastically cuts down deceleration frames and ensures your crosshair transitions to zero spread in the shortest physical timeframe possible.

🎯 In-Game Calibration (The Range)

To find the sweet spot for your hardware and ping:

Launch VALORANT and enter The Range (靶場).

Open Settings > Video > Stats and set Shooting Error to Both (Graph + Text).

Walk sideways using A or D, then let go and immediately click your primary fire (Mouse 1).

Check the Shooting Error graph:

🔵 Blue / Cyan Bar: Means movement inaccuracy was detected (counter-strafe was too slow or duration too short).

🟠 Orange / Yellow Bar: Perfect standstill shot! Accuracy reset instantly.

Fine-tune CounterTapDurationMs in config.json until your shots consistently register orange error markers right after key release.

🛡️ Anti-Cheat & Fair Play Disclaimer [!WARNING]

Please read carefully before using this software.

Educational & Accessibility Purpose: This software is developed solely as an open-source technical proof-of-concept for input event interception and SOCD algorithms.

Riot Vanguard Compliance: Riot Games' proprietary anti-cheat (Vanguard) strictly regulates automated macro inputs, software hooks, and synthetic input injections. While hardware-level SOCD (such as Razer Snap Tap or Wooting Rappy Snappy) operates on the keyboard firmware level, software-level input automation carries inherent risks.

Risk of Account Penalties: Using external automation tools in competitive matchmaking may violate Riot Games' Terms of Service (ToS) regarding third-party automation software. The developers of this repository assume no liability for any in-game disciplinary actions, suspensions, or permanent bans resulting from the use of this code.

Recommended Use: We strongly advise utilizing this tool only in offline custom games, testing environments, or local sandboxes.

🤝 Contributing
Contributions, bug reports, and feature requests are welcome!

Fork the Project.

Create your Feature Branch (git checkout -b feature/OptimizedHook).

Commit your Changes (git commit -m 'Add low-overhead raw input listener').

Push to the Branch (git push origin feature/OptimizedHook).

Open a Pull Request.

📄 License
Distributed under the MIT License. See LICENSE for more information.
