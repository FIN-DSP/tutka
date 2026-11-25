# Tutka 1.1.3 - Modern CTP-EOS/Debian Build 🐉

2015 chiptune tracker fixed for 2026 Debian 13+ (GCC14/Qt5.15)  
**Free MIDI sequencer** for GNU/Linux (Mac OS X source available)

> **NOTE:** MIDI only - requires outboard hardware or external synth routing  
> **Devices:** Tutka outputs ALSA MIDI only.  
> **Connect:** Route MIDI to a hardware synth, or to a software synth via ALSA/JACK/PipeWire.
 
> **Compatible File Import/Export Formats**  
> Import Tutka songs (.tutka), OctaMED SoundStudio Songs (.med),  
> Export Tutka songs (.tutka), OctaMED SoundStudio Songs (.med), Standard MIDI Files (.mid)   

## 🚀 Ready-to-run Binary (Recommended)
```bash
wget https://github.com/FIN-DSP/tutka/releases/download/v1.1.3/tutka
chmod +x tutka
./tutka
```

**Runtime deps:** `sudo apt install libqt5widgets5 libqt5gui5 libqt5core5a libqt5sql5-sqlite`

## 🛠️ Build from Source
```bash
sudo apt install qtbase5-dev qt5-qmake libqt5sql5-sqlite build-essential
git clone https://github.com/FIN-DSP/tutka.git
cd tutka
qmake tutka.pro && make -j$(nproc)
./tutka
```

## Debian Package (Future)
```bash
# .deb packaging WIP
sudo apt install qt5-default libasound2-dev checkinstall
# make install → checkinstall → tutka_1.1.3-1_amd64.deb
```

![Tutka Screenshot](https://raw.githubusercontent.com/FIN-DSP/tutka/main/images/tutka_screenshot.png)

**Key fixes:**
- ✅ **Added BINARY install**  
- ✅ **Correct runtime deps** 
- ✅ **qt5-default → qtbase5-dev** (modern naming)
- ✅ **Both binary + source paths**
- ✅ **No duplication**
- ✅ **CTP-EOS Debian 13 trixie** confirmed
- ✅ **Linux Compatible Binary** should work on all Linux distributions.

