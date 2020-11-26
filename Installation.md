### Automatic

You can install Omega automatically on our website [here](https://getomega.web.app/) in the "install" page.

<a href="https://getomega.web.app"><p align="center"><img alt="Omega Banner Discord" src="https://user-images.githubusercontent.com/12123721/86352956-e9000480-bc66-11ea-82b7-79fd7e56fa27.png" /></p></a>

### Manual

First of all, follow **step 1** [here](https://www.numworks.com/resources/engineering/software/build/). Then:

<details>
  <summary><b>Model n0100</b></summary>

```bash
git clone --recursive https://github.com/Omega-Numworks/Omega.git
cd Omega
git checkout omega-master
make MODEL=n0100 clean
make MODEL=n0100 OMEGA_USERNAME="{Your name, max 15 characters}" -j4
make MODEL=n0100 epsilon_flash
```

Important: Don't forget the `--recursive` tag, because Omega relies on submodules.
Also, you can change the number of processes that run in parallel during the build by changing the value of the `-j` flag.
  
</details>

<details>
  <summary><b>Model n0110</b></summary>

```bash
git clone --recursive https://github.com/Omega-Numworks/Omega.git
cd Omega
git checkout omega-master
make clean
make OMEGA_USERNAME="{Your name, max 15 characters}" -j4
make epsilon_flash
```

Important: Don't forget the `--recursive` tag, because Omega relies on submodules.
Also, you can change the number of processes that run in parallel during the build by changing the value of the `-j` flag.
  
</details>

<details>
  <summary><b>Bin files</b></summary>
  
These can be used to distribute Omega (so that it can be flashed by anyone with [Webdfu_Numworks](https://ti-planet.github.io/webdfu_numworks/)).

```bash
git clone --recursive https://github.com/Omega-Numworks/Omega.git
cd Omega
git checkout omega-master
make clean
make MODEL=n0100 OMEGA_USERNAME="" -j8
make MODEL=n0100 OMEGA_USERNAME="" binpack -j8
make OMEGA_USERNAME="" -j8
make OMEGA_USERNAME="" binpack -j8
```

Important: Don't forget the `--recursive` tag, because Omega relies on submodules.
Also, you can change the number of processes that run in parallel during the build by changing the value of the `-j` flag.
  
</details>

<details>
  <summary><b>Web simulator</b></summary>
  
First, install emsdk :

```bash
git clone https://github.com/emscripten-core/emsdk.git
cd emsdk
./emsdk install latest-fastcomp
./emsdk activate latest-fastcomp
source emsdk_env.sh
```

Then, compile Omega :

```bash
git clone --recursive https://github.com/Omega-Numworks/Omega.git
cd Omega
git checkout omega-master
make clean
make PLATFORM=simulator TARGET=web OMEGA_USERNAME="{Your name, max 15 characters}" -j4
```

The simulator is now in `output/release/simulator/web/simulator.zip`

Important: Don't forget the `--recursive` tag, because Omega relies on submodules.
Also, you can change the number of processes that run in parallel during the build by changing the value of the `-j` flag.

</details>

<details>
  <summary><b>3DS Simulator</b></summary>
  
You need devkitPro and devkitARM installed and in your path (instructions [here](https://devkitpro.org/wiki/Getting_Started))
```bash
git clone --recursive https://github.com/Omega-Numworks/Omega.git
cd Omega
git checkout --recursive omega-dev
make PLATFORM=simulator TARGET=3ds -j
```
You can then put epsilon.3dsx on a SD card to run it from the HBC or use 3dslink to launch it over the network:
```bash
3dslink output/release/simulator/3ds/epsilon.3dsx -a <3DS' IP ADDRESS>
```

</details>

If you need help, you can join our Discord server here : https://discord.gg/X2TWhh9

<a href="https://discord.gg/X2TWhh9"><p align="center"><img alt="Omega Banner Discord" src="https://user-images.githubusercontent.com/12123721/86287349-54ef5800-bbe8-11ea-80c1-34eb1f93eebd.png" /></p></a>
---