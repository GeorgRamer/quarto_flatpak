# QUARTO for flatpak SDK

These files create a flatpak SDK extension for [Quarto](https://quarto.org/), This allows you to use Quarto from flatpak IDEs like VS Codium without requiring to poke additional holes into flatpak. 

## How to run and install the SDK extension

1. Clone this repository to your machine
2.  Install the Builder flatpak

  flatpak install -y flathub org.flatpak.Builder

3. In the cloned repository run the following command to make the build.sh executable

  chmod +x build.sh
  
4. build and install the flatpak extension
  ./build.sh
  
## Enabling extension in other flatpaks

In order to enable the SDK extension. The easiest way to do this is to install the [Flatseal](https://flathub.org/apps/com.github.tchx84.Flatseal) flatpak and then adding the environmental variable `FLATPAK_ENABLE_SDK_EXT=quarto`

[Flatseal](pictures/flatseal.png)
