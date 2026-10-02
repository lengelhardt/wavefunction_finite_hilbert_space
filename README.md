# Wavefunction in a Finite Hilbert Space

An interactive, single-page simulation for teaching how a continuous wavefunction is represented by a finite set of coefficients, and how that representation approaches the wavefunction as the dimension of the Hilbert space grows.

**Run it in your browser:** https://lengelhardt.github.io/wavefunction_finite_hilbert_space/

Nothing to install. To run it offline, download `index.html` and open it in any modern browser.

## What it shows

A particle in a box of length L has eigenstates ψₙ(x) = √(2/L) sin(nπx/L). The box is divided into N equal cells of width Δx = L/N, and each cell gets one coefficient cᵢ, with |cᵢ|² = ∫ |ψ|² dx over that cell and the sign of ψ in the cell.

- **Wavefunction:** the exact ψ(x)·√L, with the cell boundaries marked.
- **Coefficients:** a histogram of cᵢ on a fixed −1 to 1 scale, so students can see the coefficients shrink as N grows. The sum of their squares, shown above the plots, is the total probability.
- **Density:** an optional overlay of cᵢ/√Δx on the wavefunction plot. Dividing by √Δx turns a probability amplitude into an amplitude per unit length, and the bars approach ψ(x) as N grows.

## Controls

- **Dimension of Hilbert space, N:** a number box and a slider.
- **Quantum number n.**
- **Display Density:** overlays cᵢ/√Δx on the wavefunction plot. Off by default.
- **Autoscale histogram:** zooms the coefficient axis in on the values. Off by default.
- **Calculate** and **Reset.** The plots also update as you type.

Hover over a plot to read values.

## Credits and license

Created by Larry Engelhardt, Francis Marion University, with Claude (Anthropic), 2026. It is a port of `WaveMechanicsApp`, a Java program written by Larry Engelhardt in 2010 with the Open Source Physics library.

This work is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). See [LICENSE](LICENSE).
