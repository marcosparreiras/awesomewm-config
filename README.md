# AwesomeWM Configuration

## Funcionalidades

- Layouts principais: tile e tile.left
- Widgets:
  - Volume (`pactl`)
  - Rede (`vicious.widgets.net`)
  - Bateria (`vicious.widgets.bat`)
  - CPU (`vicious.widgets.cpu`)
  - Memória RAM (`vicious.widgets.mem`)
  - Relógio com calendário pop-up
  - Indicador de layout e teclado
- Hotkeys para navegação entre tags, manipulação de janelas, volume e execução de comandos
- Autostart: `picom`, `nm-applet`

## Dependências

### AwesomeWM
- awesome (>= 4.3)

### Aplicativos
- `alacritty` (terminal)
- `nvim` ou outro editor de sua preferência
- `flameshot` (captura de tela)
- `pactl` (controle de áudio)
- `nm-applet` (gerenciamento de rede)
- `picom` (compositor para transparência e sombras)

### Debian/Ubuntu
```bash
sudo apt install awesome alacritty flameshot pulseaudio-utils network-manager-gnome picom
```

## Instalação

1. Clone o repositório para o diretório de configuração do AwesomeWM: `~/.config/awesome/`

2. Recarregue o AwesomeWM: `Ctrl+Super+r`

3. Ajuste o sink do áudio, interfaces de rede e bateria e o dispositivo de disco no `rc.lua` conforme seu sistema:

```lua
local sink = "alsa_output.pci-0000_00_1f.3-platform-skl_hda_dsp_generic.HiFi__hw_sofhdadsp__sink"
local wifi_iface = "wlp0s20f3"
local eth_iface = "enp1s0"
local disk_device = "nvme0n1"
```
