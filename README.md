# Scripts
My own bash scripts, created to solve my personal issues.


##Salah script
This script is to get the current salah time according to your geolocation this uses salahtime

for Arch linux(AUR)
```bash 
  sudo yay -S salahtime
```
for more info on your operating system
```bash
  https://codeberg.org/unixdigest/salahtime.git
```

Additionally you can create an icon on statusbar as i did to display this
```bash
"custom/salah": {
	"exec": "~/.local/bin/salah(Your Script location)",
	"interval": 60,
	"format": "🕌: {}",
	"on-click": "notify-send 'Prayer Schedule' \"$(salahtime)\"",
	"tooltip": false
	
}
```
