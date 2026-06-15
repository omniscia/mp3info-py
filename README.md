# MP3Info — MP3 / MPEG audio metadata + ID3 tag extractor

**Used in 29+ public GitHub repositories.** ![GitHub](https://img.shields.io/badge/in%20use-29%2B%20repos-blue)

Extracts MPEG audio frame info and ID3 (v1/v2) tags from MP3 files — pure Python, no dependencies. Evolved 2002–2004 (RCS through v1.12); widely embedded in early-2000s media software.

By **Vivake Gupta** (2004). This repository keeps the full lineage in version
control: the original release and a faithful Python 3 modernization
(`git log MP3Info.py` walks the evolution).

## Used by (a sample)
- **freevo/kaa-metadata** — the Freevo media-center metadata library
- **aeridus/edna-MP3-Server-Redux** — edna streaming MP3 server
- **joerg-lehmann/PyTone** — PyTone music player
- **AvsPmod**, **camflan/mango**, **jamiew/rolldabeats-lookup**
- (historically: ECLipT Roaster, Xiph Positron, OpenNapster client, WiLM's MP3 Server)

## Usage
```python
from MP3Info import MP3Info
info = MP3Info(open('song.mp3','rb'))
print(info.mpeg.bitrate, info.id3.title)
```

## License
GPL-2.0-or-later, per the original header.
