# EE274, in motion

Interactive, animated demos of the core ideas in EE274 (Quantum Computing Architectures), organized into five chapters. Each demo pairs a short explanation with live controls and an animation.

Open `index.html` in any modern browser. There is no build step and nothing to install.

## Demos

| Chapter | Lectures | Demos |
|---|---|---|
| 1. Qubit math | 1–5 | Born-rule measurement · single-qubit interference (H·H vs. H·Z·H) · Bell state with H + CNOT |
| 2. Bloch sphere & noise | 5–9 | Gates as Bloch-sphere rotations · T1/T2 decay with a live density matrix · Ramsey decay and spin echo |
| 3. Driving spin qubits | 10–16 | Larmor precession (Z gate) · Rabi oscillation in rotating and lab frames · silicon spin-to-charge readout |
| 4. Superconducting qubits | 16–25 | LC oscillator vs. transmon anharmonicity (8-level driven simulation) · Cooper-pair box bands vs. gate charge with charge noise · dispersive readout in the I-Q plane |
| 5. Trapped ions | 27–28 | Doppler cooling of an ion chain · fluorescence readout with photon-count threshold |

## Notes on the physics

- Cooper-pair box bands are exact numerical eigenvalues of H = 4E_C(n − n_g)² − E_J cos φ in a truncated charge basis (n = −10…10).
- The transmon ladder uses E_n ≈ −E_J + √(8E_J E_C)(n + ½) − (E_C/12)(6n² + 6n + 3), with E_C/h = 250 MHz for the displayed frequencies.
- The anharmonicity demo integrates the driven Schrödinger equation (RK4, rotating frame, 8 levels).
- Animations run on scaled time so motion is visible. Readout panels give physical values where they apply. Photon counts (fluorescence) and velocity units (Doppler cooling) are illustrative.

## Hosting with GitHub Pages

Place this folder in the repository (for example under `docs/ee274-interactive/`), then enable Pages from the repository settings. The page will be served at `https://<user>.github.io/<repo>/ee274-interactive/`.

## Credits

Content follows the EE274 lecture sequence (Prof. Hiu-Yung Wong). The lecture slides themselves are not included in this repository.
