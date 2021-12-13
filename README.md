# INSEL Block C++ programming demo

In this demo, we created a insel (C++) block for the nonlinear network solver 
[Hydraulic Network](https://github.com/leannejdong/HydraulicNetwork)


## Build/Run instruction

### Installation of INSEL 8.3

For winsows and Mac OS, please refer to [page3 INSEL Tutorial 1](https://insel.eu/files/public/inselTutorial_en_Module_1.pdf)

#### Linux

Debian-based distro: `sudo apt install ./insel_8.3.0.6b_x86_full.deb`

Arch-based: Instead of `apt` or `apt-get`, Arch users can install via `pacman` or though `AUR`.
Instructions will be supported later.

### Build and Run

We build insel block with [GNU Make](https://www.gnu.org/software/make/)

* make

* insel hydro.insel

## Future development 

The equations we solve requires plenty of inputs and parameters. Hence, creating insel blocks and getting output from it based on the whole code is somewhat difficult and impractical.
PhD students (Abolfazl Rezaei) will ve working on splitting the code into certain parts, and create multiple blocks outs of it.

### Small notes
Inputs: the demand data, network topology
Parameters: length, diameter, roughness, specific heat capacity, U-values (total heat transfer coefficients)

