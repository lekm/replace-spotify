# Replace Spotify: Ethical Music Streaming Research

Research and documentation for replacing Spotify with ethical, artist-friendly alternatives that align with leftist values.

## 🎯 Project Goal

Find and implement music streaming/ownership solutions that:
- **Support artists fairly** (better compensation than Spotify's $0.003/stream)
- **Align with socialist values** (anti-war, pro-LGBTQI+, anti-corporate exploitation)
- **Provide technical compatibility** (iPhone, CarPlay, Sonos, WiiM Pro Plus)
- **Enable music ownership** (downloads, self-hosting, format shifting)

## 📊 Key Findings

### Ethical Rankings (2024)

| Service | Ethics Score | Artist Pay/Stream | Notes |
|---------|--------------|-------------------|-------|
| **Qobuz** | 9/10 ✅ | $0.022 | French company, cleanest record |
| **Navidrome** | 10/10 ✅ | N/A | Self-hosted, complete control |
| **Apple Music** | 6/10 ⚠️ | $0.0056-$0.0078 | Mixed: LGBTQ+ support but tax avoidance |
| **Tidal** | 4/10 ⚠️ | $0.013 | Corporate instability, mass layoffs |
| **YouTube Music** | 3/10 ❌ | $0.0027 | Removed LGBTQ+ protections (2025) |
| **Spotify** | 2/10 ❌ | $0.003-$0.004 | CEO invested €600M in weapons company |

### Why Not Spotify?

- **Military investment**: CEO Daniel Ek invested €600M in Helsing (AI drone/weapons company)
- **Censorship**: Removed Palestinian artists under Israeli lobby pressure
- **Artist boycotts**: 400+ artists joined "No Music for Genocide" campaign
- **Lowest compensation**: Among the worst for artist payments

## 🏆 Recommended Solutions

### Option 1: Qobuz (Pure Streaming)
- **Cost**: $19.99 AUD/month (or $16.66/month on annual plan)
- **Ethics**: 9/10 - Best commercial option
- **Quality**: Hi-res FLAC up to 24-bit/192kHz
- **Cons**: Smallest catalog, CarPlay reliability issues

### Option 2: Navidrome Self-Hosted (Recommended)
- **Cost**: $6.73-10.47 AUD/month (VPS, native AUD pricing) + music purchases
- **Ethics**: 10/10 - Complete control, support artists directly
- **Quality**: Lossless (FLAC) from your own collection
- **Pros**: Future-proof, privacy, superior CarPlay with play:Sub app

### Option 3: Hybrid (Optimal)
- **Navidrome** for owned music (vinyl rips, purchases)
- **Qobuz** for discovery and new music
- **Best of both worlds**: Ethics + discovery + ownership

## 📚 Documentation

### Core Research
- **[claude.md](./claude.md)** - Original research notes and requirements
- **[master-project-documentation.md](./master-project-documentation.md)** - Complete project overview
- **[spotify-alternatives-report.html](./spotify-alternatives-report.html)** - Full analysis report

### Setup Guides
- **[navidrome-setup-guide.md](./navidrome-setup-guide.md)** - Self-hosting instructions
- **[lidarr-discogs-workflow.md](./lidarr-discogs-workflow.md)** - Automated CD collection digitization

### Future Research
- **[future-workflows-backlog.md](./future-workflows-backlog.md)** - Planned investigations:
  - Spotify playlist export → ethical purchase mapping
  - Alternative discovery platforms (Bandcamp, SoundCloud, Last.fm)
  - Shared Navidrome legal/ethical analysis

## 🛠️ Technical Setup

### Navidrome + Lidarr Automation Stack

```
Physical Media → Discogs → Lidarr → Navidrome → play:Sub → CarPlay
(CDs/Vinyl)    (Catalog) (Auto)   (Stream)    (iOS App)  (Playback)
```

**Components**:
- **Navidrome**: Self-hosted music server (open source)
- **Lidarr**: Automated music acquisition for owned physical media
- **Discogs**: Collection management and barcode scanning
- **play:Sub**: iOS app with excellent CarPlay integration ($15)
- **OVHcloud VPS**: Ethical hosting (Sydney datacenter, $6.73-10.47 AUD/month native pricing)

**Legal Status**: ✅ Format shifting is legal in Australia for owned physical media (Copyright Act 1968, Section 43C)

## 💰 Cost Comparison

| Solution | Annual Cost (AUD) | Ethics Score |
|----------|-------------------|--------------|
| Spotify Premium | $191.88 | 2/10 ❌ |
| Qobuz Studio (monthly) | $239.88 | 9/10 ✅ |
| Qobuz Studio (annual) | $199.90 | 9/10 ✅ |
| Navidrome + VPS | $96-141 | 10/10 ✅ |
| Hybrid (Navidrome + Qobuz annual) | $296-341 | 10/10 ✅ |

**Savings**: Navidrome-only saves $59-104/year vs Qobuz (monthly) or $104/year vs Qobuz (annual plan), $96/year vs Spotify

*Prices verified October 2025 - [Sources](sources.md)*

## 🎵 Device Compatibility

### WiiM Pro Plus (Home)
- ✅ **Excellent**: Tidal Connect, Qobuz native, Navidrome (Subsonic)
- ⚠️ **Limited**: Apple Music (AirPlay only, 256kbps max)

### CarPlay (Daily Use - Most Critical)
- ✅ **Excellent**: Apple Music (native), play:Sub + Navidrome (more reliable than Qobuz)
- ✅ **Good**: Spotify
- ❌ **Problematic**: Qobuz native app (crashes, blank screens, connection drops)

### Sonos (Office)
- ✅ **Native**: Apple Music, Spotify
- ⚠️ **Limited**: Tidal/Qobuz Connect not supported (use AirPlay)

## 🚀 Getting Started

### Immediate Steps (This Week)
1. **Export Spotify playlists** using Soundiiz or FreeYourMusic
2. **Test Qobuz** free trial for audio quality and catalog
3. **Read setup guides** to understand Navidrome workflow

### Implementation (Next Month)
1. **Deploy VPS** (OVHcloud Australia recommended)
2. **Install Navidrome** via Docker
3. **Purchase play:Sub** iOS app
4. **Test CarPlay** reliability
5. **Migrate playlists** from Spotify

### Long-term (Ongoing)
1. **Digitize CD collection** using Lidarr + Discogs
2. **Use Qobuz for discovery** → buy favorites
3. **Support artists directly** (Bandcamp, concerts, merch)
4. **Cancel Spotify** once transition complete

## 📖 Background

This research was conducted for a Melbourne-based record collector seeking to replace Spotify due to:
- **Ethical concerns**: Military investments, artist censorship, poor compensation
- **Political values**: Socialist, pro-LGBTQI+, land back/decolonisation, anti-war
- **Technical needs**: Reliable CarPlay, high-quality audio, device compatibility
- **Music habits**: Vinyl/CD collector, discovery-focused, wants to own music

## 🤝 Contributing

This research is shared to help others make informed, ethical music streaming choices. Feel free to:
- Open issues with corrections or updates
- Share your own experiences with alternatives
- Suggest additional platforms to research
- Contribute to future workflow investigations

## 📜 License

Documentation released under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) - Share and adapt with attribution.

---

**Last Updated**: October 2025
**Status**: Active research, Navidrome setup in progress
**Contact**: Open an issue for questions or suggestions

---

*Built with leftist values: Support artists, resist corporate exploitation, own your culture.*
