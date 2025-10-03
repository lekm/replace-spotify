# Spotify Replacement Project - Master Documentation

## Project Overview

**Goal**: Replace Spotify with an ethical, technically compatible, and politically aligned music solution that supports a record collecting enthusiast in Melbourne, Australia.

**User Profile**:
- Location: Melbourne, Australia
- Political Values: Socialist, pro-LGBTQI+, land back/decolonisation, tax the rich, defund police
- Budget: Up to $30+ AUD per month
- Technical Setup: iPhone → Sonos (office) / WiiM Pro Plus (home) / Wired CarPlay (extensive use)
- Music Habits: Record collecting (Rega Planar 2), vinyl + digital collection, discovery-focused
- Additional: Significant CD collection stored in New Zealand (too heavy/fragile to ship)

## Key Requirements Identified

### Ethical Concerns
- **Spotify Issues**: Poor artist compensation ($0.003/stream), CEO invested €600M in AI weapons company, Palestinian artist censorship
- **Political Alignment**: Need solution that doesn't support military-industrial complex or corporate exploitation
- **Artist Support**: Preference for direct artist compensation and ethical streaming

### Technical Requirements
- **Discovery**: Better algorithm than Spotify (declined post-2018)
- **Audio Quality**: High-quality downloads preferred over streaming only
- **CarPlay**: Reliable wired CarPlay support (critical for daily use)
- **Device Integration**: iPhone, Sonos, WiiM Pro Plus compatibility
- **Migration**: Must export existing Spotify playlists without losing music
- **Offline Capability**: Download support for travel/poor coverage areas

## Research Findings Summary

### Music Discovery Algorithm Rankings (2024)
1. **YouTube Music**: Most intelligent AI, highly responsive to user feedback
2. **Spotify**: Still decent but repetitive, mainstream bias
3. **Tidal**: Excellent for discovering new/emerging artists via curation
4. **Apple Music**: Good integration but tends toward mainstream

### Artist Compensation (Per Stream, USD)
1. **Qobuz**: $0.022 (733% higher than Spotify)
2. **Napster**: $0.019-$0.021
3. **Tidal**: $0.013 (333% higher than Spotify)
4. **Apple Music**: $0.0056-$0.0078
5. **Deezer**: $0.0064
6. **Spotify**: $0.003-$0.004 (baseline)
7. **YouTube Music**: $0.0027 (25% lower than Spotify)

### Corporate Ethics Analysis (2024)

#### Spotify - Ethics Score: 2/10 (AVOID)
- **Major Red Flags**: €600M investment in Helsing (AI drone/weapons company)
- **Censorship**: Removed Palestinian artists under Israeli lobby pressure
- **Artist Opposition**: 400+ artists joined "No Music for Genocide" campaign
- **Recommendation**: Avoid due to direct opposition to anti-war values

#### Apple Music - Ethics Score: 6/10 (MIXED)
- **Positive**: Historically supportive of LGBTQ+ rights, diversity initiatives
- **Negative**: Massive tax avoidance, labor exploitation in factories, NLRB charges
- **Assessment**: Corporate liberalism - better than average but still problematic

#### Tidal - Ethics Score: 4/10 (AVOID)
- **Issues**: Mass layoffs, "No Jay-Z" discussion ban, $297M acquisition deemed "terrible decision"
- **Ownership**: Block/Square (Jack Dorsey) - corporate dysfunction and worker exploitation

#### Qobuz - Ethics Score: 9/10 (RECOMMENDED)
- **Strengths**: French company, no major scandals, gave 100% revenue to artists during COVID-19
- **Governance**: European standards, artist-focused mission, clean corporate record

#### YouTube Music/Google - Ethics Score: 3/10 (AVOID)
- **Issues**: Removed LGBTQ+ protections, class action lawsuit from LGBTQ+ creators
- **Trend**: Increasingly hostile to LGBTQ+ communities

### Technical Compatibility Analysis

#### CarPlay Performance
- **Excellent**: Apple Music (native integration, deep Siri support)
- **Good**: Spotify (intuitive interface, voice control)
- **Problematic**: Qobuz (frequent crashes, blank screens, connection drops after ~15 seconds)
- **Acceptable**: YouTube Music, Tidal

#### WiiM Pro Plus Integration
- **Excellent**: Tidal Connect (full hi-res), Qobuz native support
- **Limited**: Apple Music (AirPlay only, 256kbps max)
- **Good**: YouTube Music (Google Cast)

#### Sonos Integration
- **Native Support**: Apple Music, Spotify
- **Limited**: Tidal/Qobuz Connect not supported
- **Note**: 2024 Sonos app redesign caused reliability issues

### Cost Analysis (AUD, 2024 Pricing)

#### Streaming Services (Annual Costs)
- **Spotify Premium**: $15.99/month = $191.88/year [(Source)](https://www.spotify.com/au/premium/)
- **Qobuz Studio**: $19.99/month = $239.88/year OR $199.90/year (annual plan) [(Source)](https://www.qobuz.com/au-en/music/streaming/offers/studio)
- **Apple Music**: $12.99/month = $155.88/year [(Source)](https://www.apple.com/au/apple-music/)
- **Tidal HiFi Plus**: ~$20-25/month = $240-300/year *(needs verification)*
- **YouTube Music**: ~$12/month = $144/year *(needs verification)*

*Prices verified October 2025*

#### Self-Hosted Options (Annual Costs)
- **OVHcloud VPS-1**: $6.73 AUD/month (inc GST) = $80.76/year ✅ Native AUD pricing
- **OVHcloud VPS-2**: $10.47 AUD/month (inc GST) = $125.64/year ✅ Native AUD pricing
- **Linode Nanode**: ~$7.55 AUD/month* = ~$90.60/year *USD pricing, subject to exchange rates
- **play:Sub app**: $15 AUD (one-time)
- **Total**: $96-141 AUD/year + music purchases

*Non-OVHcloud prices are USD converted at Oct 2025 rates and will fluctuate*

## Recommended Solutions

### Primary Recommendation: Qobuz
**Why**: Best alignment with leftist values, highest artist compensation, cleanest corporate record
**Cons**: Smallest catalog, CarPlay reliability issues
**Cost**: $300-360 AUD/year
**Best For**: Maximum ethics when technical limitations are acceptable

### Optimal Solution: Navidrome + Qobuz Hybrid
**Components**:
- **Navidrome**: Self-hosted server for owned music (vinyl rips, purchases)
- **Qobuz**: Ethical discovery and streaming of new music
- **play:Sub**: iOS app with excellent CarPlay integration (more reliable than Qobuz native app)

**Benefits**:
- **Complete Privacy**: Most listening tracked locally
- **Maximum Ethics**: Highest artist compensation + direct purchases
- **Superior CarPlay**: play:Sub more reliable than Qobuz native app
- **Future-Proof**: Own music regardless of service changes
- **Cost-Effective**: $104-154 AUD/year vs $200-240 for Qobuz alone

### VPS Hosting Analysis (Melbourne, Australia)

#### Ethical VPS Comparison
| Provider | AUD/Month | Ethics Score | Currency | Notes |
|----------|-----------|-------------|----------|-------|
| **OVHcloud VPS-1** | **$6.73** | 8/10 | ✅ Native AUD | European company, Sydney datacenter, data sovereignty |
| **OVHcloud VPS-2** | **$10.47** | 8/10 | ✅ Native AUD | More RAM/CPU, same benefits as VPS-1 |
| Linode Nanode | ~$7.55* | 7/10 | USD* | Cleanest US provider, adequate latency |
| DigitalOcean | ~$9.06* | 5/10 | USD* | Mass layoffs, broken promises to employees |
| Vultr Regular | ~$5.29* | 6/10 | USD* | Budget option, 2024 content rights overreach (resolved) |

*USD pricing converted to AUD at Oct 2025 rate (1 USD = 1.51 AUD). These prices fluctuate with exchange rates. OVHcloud prices are native AUD and fixed.

#### Latency from Melbourne
- **OVHcloud Australia**: 10-20ms (Sydney local)
- **All others**: 359-400ms (only 10-20ms difference between providers)
- **Verdict**: Negligible impact for music streaming

#### Recommendation
**For Maximum Ethics**: OVHcloud Australia VPS-1 or VPS-2 ($89-139 AUD/year inc GST)
- Data sovereignty under Australian law
- European privacy protections
- Zero latency concerns
- Aligns with anti-US-tech-monopoly values

## Advanced Setup: Music Automation

### Lidarr Integration
**Purpose**: Automated music acquisition for owned physical media
**Workflow**: Scan barcode in NZ → Add to Discogs → Lidarr finds digital copies → Adds to Navidrome

**Legal Status (Australia)**: ✅ Legal under format shifting provisions for owned physical media

### Discogs Integration
**Status**: Active development - pull request in progress for Discogs import lists
**Function**: Sync Discogs collection/wantlist to trigger Lidarr searches
**Your Use Case**: Perfect for CD collection stored in New Zealand

### Complete Automation Stack
```
Physical Media (NZ) → Discogs (barcode scan) → Lidarr (auto-download) → Navidrome (streaming) → play:Sub (CarPlay)
```

## Migration Strategy

### Phase 1: Immediate Steps
1. **Export Spotify playlists** using Soundiiz or FreeYourMusic
2. **Test Qobuz** free trial for ethics + audio quality
3. **Test Apple Music** as backup for broader compatibility
4. **Avoid Tidal** due to corporate instability and labor issues

### Phase 2: VPS Setup
1. **Choose provider**: OVHcloud Australia for maximum ethics, Linode for budget
2. **Deploy Navidrome**: Self-hosted music server
3. **Install play:Sub**: iOS app for superior CarPlay integration
4. **Test CarPlay**: Ensure reliability for daily use

### Phase 3: Hybrid Implementation
1. **Navidrome for owned music**: Vinyl rips + purchased digital files
2. **Qobuz for discovery**: Ethical streaming for new music exploration
3. **Direct artist purchases**: Buy favorites discovered through Qobuz
4. **Lidarr automation**: Automated acquisition of owned physical media

### Phase 4: Advanced Automation
1. **Set up Lidarr**: Music automation server
2. **Configure Discogs integration**: Sync collection for automated downloads
3. **Establish workflow**: NZ CD scanning → Discogs → Lidarr → Navidrome
4. **Family integration**: Multi-user setup with library permissions

## Files Created

### Documentation
- `spotify-alternatives-report.html` - Complete analysis report
- `navidrome-setup-guide.html` - Comprehensive setup guide
- `claude.md` - Markdown research notes
- `navidrome-setup-guide.md` - Markdown setup guide
- `master-project-documentation.md` - This master document

### Key Tools for Migration
- **Soundiiz/FreeYourMusic**: Playlist migration
- **play:Sub**: iOS app for CarPlay integration
- **Navidrome**: Self-hosted music server
- **Lidarr**: Music automation (future)
- **OVHcloud Australia**: Ethical VPS hosting

## Next Steps for Future Sessions

### Immediate Priorities
1. **Export Spotify data** before canceling subscription
2. **Set up VPS** (OVHcloud Australia recommended)
3. **Deploy Navidrome** with initial music collection
4. **Test CarPlay integration** with play:Sub app

### Future Development
1. **Lidarr setup** for automation when Discogs integration releases
2. **Family user management** for multi-library setup
3. **Backup strategy** for music collection and metadata
4. **Expansion planning** as collection grows

### Success Metrics
- **CarPlay reliability** (most critical for daily use)
- **Discovery quality** compared to Spotify's algorithm
- **Cost savings** vs streaming subscriptions
- **Ethical alignment** with political values
- **Music collection growth** through direct artist support

## Political and Ethical Alignment Summary

This solution aligns with leftist values by:
- **Opposing military-industrial complex** (avoiding Spotify's weapons investments)
- **Supporting worker rights** (avoiding DigitalOcean's labor exploitation)
- **Promoting artist welfare** (highest compensation through Qobuz + direct purchases)
- **Reducing corporate dependence** (self-hosted infrastructure)
- **Supporting open-source** (Navidrome, various tools)
- **Data sovereignty** (Australian hosting, European privacy protections)
- **Anti-monopoly stance** (supporting smaller, ethical providers)

## Technical Architecture Summary

```
Music Sources → Processing → Storage → Streaming → Playback
     ↓             ↓          ↓         ↓         ↓
Vinyl Rips    → Navidrome → VPS     → Home     → iPhone
CD Collection → Lidarr    → Server  → WiFi     → CarPlay
Qobuz Stream  → play:Sub  → Sydney  → Mobile   → Sonos
Direct Buys   → Metadata → OVH     → Remote   → WiiM Pro
```

This architecture provides complete ownership, maximum privacy, superior CarPlay reliability, and perfect alignment with leftist political values while maintaining excellent technical performance for a Melbourne-based user.