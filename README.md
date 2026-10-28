# Quaternion · Quantum Computing

**▶ Open the course: [shanem73.github.io/Quaternion-Quantum-computing](https://shanem73.github.io/Quaternion-Quantum-computing/)**

Jump straight to a module: [I · Hamilton's Quaternions](https://shanem73.github.io/Quaternion-Quantum-computing/#quaternions) · [II · Qubits on the Sphere](https://shanem73.github.io/Quaternion-Quantum-computing/#qubits)

**Designer and main contributor:** Prof. Xin (Shane) Miao, Missouri State University ([@ShaneM73](https://github.com/ShaneM73))

A two-module interactive course that runs in the browser, with no build step and no dependencies beyond Google Fonts.

| Module | Folder | Steps | What it covers |
|---|---|---|---|
| I · Hamilton's Quaternions | [`quaternions/`](quaternions/) | 11 | Complex numbers as rotations, Hamilton's 1843 discovery, the rules of *i, j, k*, rotating space with *q v q⁻¹*, slerp, the vector war, and the link to qubits |
| II · Qubits on the Sphere | [`qubits/`](qubits/) | 14 | The qubit and the Bloch sphere, measurement, gates as quaternions, interference, noise, entanglement, phase kickback, teleportation, Grover search, gate synthesis, error correction |

The two modules share one dictionary: *i* ↔ −iσx, *j* ↔ −iσy, *k* ↔ −iσz, so unit quaternions are exactly the single-qubit gates in SU(2).

## Layout

```
index.html            Hub: course map, progress for both modules, tabbed switcher
quaternions/index.html  Module I (standalone page)
qubits/index.html       Module II (standalone page)
```

The hub opens each module in a full-height frame, so the modules stay separate items and each also works on its own. Direct links: `index.html#quaternions` and `index.html#qubits`. Progress is saved per module in the browser's localStorage.

## Run locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Publish

The site is plain static HTML and is served by GitHub Pages from the `main` branch root.
