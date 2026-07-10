# Supplementary material

This repository accompanies the paper *"Parsimonious disturbance-aware
minimum-time planning with parametric uncertainty"* (Gulisano, Masoni,
Gabiccini, Guiggiani — Università di Pisa). It provides two artefacts for
reviewers and readers: the full vehicle parameter set used in the study, and
an interactive viewer for the closed-loop Monte Carlo results.

## `released_fsae_vehicle_data.json`

The complete parameter set of the Formula SAE single-track vehicle model
used throughout the paper: mass and inertia properties, geometry, tyre
(Magic Formula, pure lateral slip) coefficients, aerodynamic data, and the
uncertainty description (initial covariance `P0` and process noise `Q` on
the augmented state used for covariance propagation). Every entry carries
its symbol, value, unit, and a short description, so the file can be read
standalone or cross-referenced against the paper's notation.

## `index.html` — interactive MPC dashboard

A self-contained, offline interactive page (no server or internet
connection required) that visualises the closed-loop MPC Monte Carlo
campaign: 1000 perturbed runs per reference trajectory, for each of the
four planning strategies compared in the paper. 

Live at <https://martinogulisano.github.io/data-parsimonious-disturbance-aware/>.
