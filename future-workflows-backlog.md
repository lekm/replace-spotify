# Future Workflows Backlog
## Research Areas for Later Exploration

---

## Overview

This document captures workflows and research areas identified for future investigation. These are **not yet researched** but represent potential expansions of the Spotify replacement project.

**Status**: 📋 Backlog - No investigation completed
**Last Updated**: October 2024

---

## Workflow 1: Spotify Playlist Export & Ethical Purchase Mapping

### Objective
Enable users to export Spotify playlists and discover where to **purchase** (not stream) the music from ethical sources, prioritizing direct artist support.

### Current State
- Spotify playlists locked in platform
- Users want to maintain music taste data
- Need pathway from streaming → ownership

### Desired Future State
**Public-facing website** that allows anyone to:
1. Export Spotify playlists (all songs, metadata, play counts)
2. Analyze their listening history and patterns
3. Receive recommendations on **where to purchase** digital downloads and physical media
4. Prioritize ethical sources that maximize artist compensation
5. Support transition from streaming subscriptions to music ownership

### Key Research Questions

#### Technical Questions
- **Spotify API access**:
  - What data can be exported via Spotify API?
  - Authentication methods for user data access
  - Rate limits and restrictions
  - Historical listening data availability

- **Playlist data structure**:
  - Track metadata available (ISRC, artist IDs, album IDs)
  - Playlist organization preservation
  - Play count and timestamp data
  - User-generated metadata (custom playlists, folders)

- **Matching algorithms**:
  - How to match Spotify tracks to purchase sources?
  - Handling multiple editions (remaster, deluxe, etc.)
  - Dealing with unavailable/out-of-print releases
  - Fuzzy matching for tracks not found exactly

#### Ethical Purchase Source Research
- **Digital download platforms**:
  - Bandcamp (direct artist support, DRM-free)
  - Qobuz (hi-res purchases, artist compensation)
  - 7digital (independent, DRM-free)
  - HDtracks (audiophile quality)
  - Bleep (electronic music focus)
  - Artist websites (direct sales)

- **Physical media sources**:
  - Independent record stores (local + online)
  - Artist merch stores (maximum artist revenue)
  - Discogs marketplace (used/rare)
  - Bandcamp (physical + digital bundles)
  - Label direct sales

- **Artist compensation comparison**:
  - Revenue split percentages by platform
  - Direct vs intermediary sales
  - Regional availability
  - DRM and format options

#### Website/Tool Requirements
- **User flow**:
  - Spotify authentication (OAuth)
  - Playlist selection interface
  - Export processing (background job)
  - Results presentation (sortable, filterable)
  - Purchase link generation

- **Features**:
  - Batch export (all playlists at once)
  - Cost estimation (total to own vs annual streaming)
  - Priority ranking (most-played tracks first)
  - Ethical scoring (artist compensation transparency)
  - Format preferences (FLAC, vinyl, CD)
  - Regional availability filtering

- **Technical stack considerations**:
  - Frontend: React/Next.js for user interface
  - Backend: API to handle Spotify OAuth and data processing
  - Database: Store mappings, cache results
  - Matching service: Track → Purchase source mapping
  - Privacy: No long-term user data storage

#### Privacy & Ethics Considerations
- **User data handling**:
  - Minimal data collection (only playlist metadata)
  - No permanent storage of listening history
  - Transparent data usage policy
  - GDPR compliance (if serving EU users)
  - Option to process entirely client-side

- **Platform neutrality**:
  - Not favoring specific vendors for kickbacks
  - Transparent methodology for recommendations
  - Open-source ranking algorithm
  - Community contributions welcome

- **Political alignment**:
  - Prioritize independent artists and labels
  - Highlight platforms with best labor practices
  - Avoid platforms with problematic corporate ties
  - Support small business/local record stores

### Success Metrics
- **User outcomes**:
  - % of playlist tracks available for purchase
  - Average cost to own most-played albums
  - User conversion from streaming to ownership

- **Ethical outcomes**:
  - Increased direct artist purchases
  - Revenue redirected from streaming to ownership
  - User awareness of artist compensation

### Implementation Phases
1. **Research Phase**: Investigate APIs, purchase platforms, matching algorithms
2. **Prototype Phase**: CLI tool for personal use
3. **MVP Phase**: Simple web interface for single playlist export
4. **Public Launch**: Full-featured website for community use
5. **Expansion Phase**: Additional streaming platforms (Apple Music, YouTube Music)

### Related Tools/Prior Art
- **Existing playlist exporters**:
  - Soundiiz (migration focus, not purchase-focused)
  - FreeYourMusic (platform transfers)
  - Exportify (CSV export only)

- **Gaps to fill**:
  - None focus on **purchasing** vs streaming
  - None provide ethical source recommendations
  - None calculate ownership cost vs subscription cost

### Questions to Answer
- [ ] What's the legal status of using Spotify API for this purpose?
- [ ] How to maintain up-to-date purchase source database?
- [ ] Business model: Free service? Donation-supported? Grant-funded?
- [ ] Hosting costs at scale (thousands of users)?
- [ ] Community moderation for purchase source quality?
- [ ] How to handle regional restrictions (Australia vs US vs EU)?

---

## Workflow 2: Alternative Music Discovery Platforms

### Objective
Evaluate non-mainstream platforms for music discovery that align with ethical values and support independent artists.

### Platforms to Investigate

#### Bandcamp
**Status**: Active and thriving

**Research Areas**:
- **Discovery features**:
  - Genre/tag browsing effectiveness
  - "Fans also like" algorithm quality
  - Editorial recommendations
  - Bandcamp Daily articles and features
  - New release notifications

- **Artist support model**:
  - Revenue splits (artist vs platform)
  - Bandcamp Fridays (100% to artists)
  - Direct fan-to-artist connection
  - Artist control over pricing/bundles

- **Integration possibilities**:
  - API availability
  - Collection export to Navidrome
  - Wish list → Lidarr automation
  - Streaming vs ownership model

- **Community features**:
  - Fan accounts and collections
  - Artist following
  - Curated lists
  - Social discovery

- **Limitations**:
  - Catalog gaps (major label music)
  - Discovery algorithm vs Spotify
  - Mobile app experience
  - Offline listening options

#### SoundCloud
**Status**: Active but evolving business model

**Research Areas**:
- **Discovery mechanisms**:
  - Algorithm quality for recommendations
  - Genre/mood browsing
  - Charts and trending
  - Repost culture and viral discovery

- **Artist ecosystem**:
  - Independent vs major label presence
  - Monetization options (SoundCloud Premier)
  - Direct artist engagement
  - Remix/bootleg culture

- **Unique features**:
  - Timed comments on tracks
  - DJ mixes and long-form content
  - Early releases and exclusives
  - Underground/emerging artist focus

- **Integration possibilities**:
  - Download options (for purchased tracks)
  - API access
  - Playlist export
  - Navidrome compatibility

- **Corporate ethics**:
  - Ownership structure
  - Artist compensation model
  - Recent controversies or labor issues
  - Data privacy practices

#### Last.fm
**Status**: Unknown - still active?

**Research Areas**:
- **Current state**:
  - Is platform still actively maintained?
  - User base size and activity
  - Feature development timeline
  - Ownership (sold to multiple companies)

- **Scrobbling functionality**:
  - Does it still work reliably?
  - Supported platforms (Spotify, Navidrome, etc.)
  - Historical data preservation
  - Analytics and insights

- **Discovery features**:
  - Recommendations based on listening history
  - Similar artist suggestions
  - Neighbor compatibility (find users with similar taste)
  - Tag-based exploration

- **Integration value**:
  - Track listening across all platforms
  - Long-term listening history preservation
  - Statistics and year-in-review
  - Social features (friends, groups)

- **Navidrome integration**:
  - Native Last.fm scrobbling support?
  - Third-party scrobbler compatibility
  - Data export options

#### Other Platforms to Consider
- **Mixcloud**: DJ mixes, radio shows, podcasts
- **Audiomack**: Hip-hop/R&B focus, emerging artists
- **Resonate**: Co-op streaming platform (stream-to-own model)
- **Faircamp**: Self-hosted alternative to Bandcamp
- **Funkwhale**: Federated audio platform (open-source)
- **Ampwall**: Artist-first streaming (if still exists)

### Key Research Questions

#### Discovery Quality
- How do algorithms compare to Spotify's (pre-2018 quality)?
- Balance of mainstream vs underground recommendations
- Genre diversity and niche coverage
- Serendipity vs echo chamber effects

#### Ethical Considerations
- Artist compensation models
- Platform ownership and corporate structure
- Labor practices and worker treatment
- Data privacy and user tracking
- Environmental impact (streaming bandwidth)

#### Technical Integration
- API access and documentation
- Export/import capabilities
- Navidrome compatibility
- Lidarr integration potential
- Mobile app quality

#### Community & Culture
- User base demographics and values
- Artist-fan interaction quality
- Curatorial vs algorithmic discovery
- DIY and independent music presence

### Workflow Documentation Needs
- **Account setup process** for each platform
- **Discovery workflow** (how to find new music effectively)
- **Collection management** (wish lists, favorites, follows)
- **Export methods** (if switching platforms later)
- **Integration guides** (Navidrome scrobbling, etc.)
- **Cost analysis** (free vs paid tiers)

### Success Criteria
- **Discovery quality**: At least as good as current Spotify
- **Ethical alignment**: Better artist compensation than streaming giants
- **Technical compatibility**: Works with Navidrome/play:Sub workflow
- **User experience**: Intuitive and enjoyable to use
- **Community**: Positive, supportive, diverse user base

### Questions to Answer
- [ ] Which platforms are still actively maintained in 2024?
- [ ] Can multiple platforms be used simultaneously for different genres?
- [ ] How to aggregate discovery across platforms?
- [ ] What's the learning curve for each platform?
- [ ] Are there mobile apps, and how good are they?
- [ ] Can listening history be preserved if platform shuts down?

---

## Workflow 3: Shared Navidrome Collections - Legal & Ethical Analysis

### Objective
Investigate the **legal status** and **ethical implications** of a small group of friends sharing their format-shifted music collections via a single Navidrome instance.

### Scenario Definition

**Setup**:
- Single VPS running Navidrome
- 3-10 friends contributing music collections
- All music is **legally owned** (CDs, vinyl, digital purchases)
- All music is **format-shifted** (personal rips, no piracy)
- **Non-commercial**: No fees charged, no profit motive
- **Private**: Closed group, no public access
- **Streaming only**: No redistribution, no downloads to third parties

**Use Case**:
- Pool vinyl collections (expensive to duplicate)
- Share CD rips (friends can't afford to re-buy everything)
- Collective library building (like borrowing CDs, but digital)
- Cost-sharing VPS expenses ($12-15/month split 5-10 ways)

### Legal Research Questions

#### Australian Copyright Law
- **Format Shifting Provisions** (Copyright Act 1968, Section 43C):
  - Does "private and domestic use" extend to close friends?
  - Is a small private group considered "domestic"?
  - What defines "private" vs "public" use?
  - Does streaming count differently than copying?

- **Personal Use Limitations**:
  - Can you stream your own format-shifted music to yourself remotely? (Yes, clearly legal)
  - Can you share with household members? (Likely yes)
  - Can you share with close friends? (Grey area)
  - Can you share with a private club/group? (Unclear)

- **Distribution vs Access**:
  - Is providing streaming access "distribution"?
  - Does user authentication matter (password-protected)?
  - Is there a difference between active sharing vs passive access?
  - Does number of users matter (5 vs 50 vs 500)?

- **Precedents and Case Law**:
  - Any Australian cases involving private music sharing?
  - Library lending vs private streaming
  - "Making available" provisions in copyright law
  - Digital vs physical sharing legal distinctions

#### International Comparisons
- **United States**:
  - Fair use doctrine applicability
  - Plex/Emby user case studies
  - RIAA stance on private streaming servers

- **European Union**:
  - Private copying levies
  - Platform liability directives
  - Member state variations

- **New Zealand**:
  - Similar common law jurisdiction
  - Format shifting provisions
  - Private use interpretations

#### Risk Assessment
- **Likelihood of legal action**:
  - Small private groups (low profile)
  - No commercial activity (lower priority)
  - Rights holder enforcement patterns
  - ISP/VPS provider policies

- **Potential consequences**:
  - Cease and desist letters
  - Account termination (VPS provider)
  - Civil liability (damages)
  - Criminal prosecution (highly unlikely for non-commercial)

- **Mitigating factors**:
  - Proof of ownership (receipts, Discogs collection)
  - No public access (invite-only, strong passwords)
  - No monetization (cost-sharing only)
  - Limited group size (friends, not strangers)

### Ethical Considerations

#### Artist Impact
- **Positive arguments**:
  - Friends might discover and purchase more music
  - Artists already compensated through original purchases
  - Equivalent to friends borrowing physical CDs
  - Enables music appreciation for lower-income friends
  - May increase concert attendance and merch sales

- **Negative arguments**:
  - Lost sales (friends don't buy duplicate copies)
  - Artists didn't consent to collective sharing
  - Scale matters (10 friends sharing = 10x the impact)
  - Streaming royalties foregone (if they'd use Spotify otherwise)
  - Slippery slope to larger-scale sharing

- **Neutral considerations**:
  - Would friends have bought the music anyway?
  - Is this functionally different from a well-curated Spotify playlist?
  - Does format-shifting ethics change with audience size?

#### Socialist/Leftist Values Alignment
- **Pro-sharing arguments**:
  - Collective ownership reduces consumption
  - Mutual aid and resource sharing
  - Resistance to artificial scarcity
  - Democratizing access to culture
  - Anti-capitalist critique of IP maximalism

- **Pro-artist arguments**:
  - Artists deserve fair compensation
  - Small independent artists need sales to survive
  - Bypassing artist consent is exploitative
  - Support direct purchases over "sharing economy"
  - Ethical consumption under capitalism

- **Reconciliation possibilities**:
  - Collective purchase fund (group buys new releases)
  - Prioritize sharing major label music (less artist harm)
  - Use shared library for discovery → buy favorites
  - Support artists via concerts, merch, Patreon
  - Transparent communication with artist community

#### Community Norms
- **Private sharing culture**:
  - Friends have shared music for decades (mixtapes, burned CDs)
  - Digital equivalent of lending physical media
  - Trust and reciprocity in friend groups
  - Non-commercial social activity

- **Boundary considerations**:
  - Where is the line between friends and public?
  - Facebook group of 50 people? Discord server of 100?
  - Does money change ethics (cost-sharing vs profit)?
  - Should there be a group size limit?

### Technical Implementation Considerations

#### Access Control
- **User authentication**:
  - Individual accounts with strong passwords
  - Two-factor authentication (2FA)
  - Account sharing restrictions
  - Activity logging and auditing

- **Privacy protections**:
  - VPN requirement for access?
  - Geoblocking to specific countries?
  - IP whitelisting (only known friends)
  - Encryption in transit (HTTPS/TLS)

#### Contribution Tracking
- **Library organization**:
  - Separate folders per contributor?
  - Metadata tagging (who owns what)
  - Proof of ownership documentation
  - Discogs integration (verify collection ownership)

- **Fair use monitoring**:
  - Who uploads how much?
  - Are contributions balanced?
  - Minimum contribution requirements?
  - Quality standards (FLAC preferred)

#### VPS Provider Policies
- **Terms of Service review**:
  - OVHcloud acceptable use policy
  - Linode content restrictions
  - DMCA takedown procedures
  - Account termination triggers

- **Risk mitigation**:
  - Encryption (whole disk encryption)
  - Encrypted backups (off-site)
  - Legal disclaimer on login page
  - Geographic server location (Australia vs US)

### Alternative Models to Research

#### Model 1: Personal Libraries Only
- Each friend runs their own Navidrome instance
- "Visit" each other's libraries (URLs shared privately)
- No centralized pooling
- Clearly personal use, minimal legal risk

#### Model 2: Time-Limited Borrowing
- Friend "checks out" an album (locks for others)
- Digital equivalent of borrowing a CD
- One copy, one listener at a time
- More defensible as non-distribution

#### Model 3: Collective Purchase Co-op
- Friends pool money to buy music collectively
- Shared ownership, shared access
- All purchases documented
- Transparent artist support model

#### Model 4: Hybrid Public/Private
- Personal collections stay private
- Shared discovery playlists only
- Use Qobuz/Bandcamp for actual streaming
- Navidrome for owned music only

### Research Methodology

#### Legal Research Steps
1. **Primary sources**:
   - Read Copyright Act 1968 (Australia) in full
   - Review case law on private copying
   - Check ACCC and copyright agency guidance
   - Review VPS provider ToS

2. **Expert consultation**:
   - IP lawyer consultation (paid, one-time)
   - Copyright advocacy groups (EFF, Digital Rights Watch Australia)
   - Academic papers on digital sharing
   - Community forums (Reddit /r/legaladvice, Whirlpool)

3. **Comparative analysis**:
   - How do other jurisdictions handle this?
   - Plex/Jellyfin user experiences
   - Private torrent tracker legal status
   - Family sharing features in commercial services

#### Ethical Deliberation Process
1. **Stakeholder perspectives**:
   - Artists (independent vs major label)
   - Friends (access to culture)
   - Society (copyright balance)
   - Own values (socialist principles)

2. **Thought experiments**:
   - What if everyone did this?
   - Would I tell an independent artist I'm doing this?
   - How is this different from Spotify (artist perspective)?
   - What would a fair system look like?

3. **Community input**:
   - Survey friends on ethics
   - Ask musician friends their perspective
   - Research artist co-op positions
   - Explore open culture movements

### Decision Framework

**Proceed if**:
- ✅ Legal risk is low (lawyer consultation confirms)
- ✅ Group is genuinely small and private (≤10 friends)
- ✅ All music is legitimately owned
- ✅ Non-commercial (only cost-sharing)
- ✅ Ethical comfort level is high
- ✅ Artists would be supported in other ways (concerts, direct purchases)

**Do not proceed if**:
- ❌ Legal risk is significant (lawyer advises against)
- ❌ Group is large or semi-public (>20 people)
- ❌ Any pirated content involved
- ❌ Commercial motive (profit from access)
- ❌ Ethical discomfort (feels wrong)
- ❌ Would harm independent artists without compensation

**Alternative approaches if uncomfortable**:
- Each friend runs their own server (personal use only)
- Use Qobuz/Spotify family plans (legal streaming)
- Collective purchase fund (buy music together)
- Library lending model (one listener at a time)

### Questions to Answer
- [ ] What does Australian copyright law actually say about private sharing?
- [ ] Has anyone been prosecuted for small-scale private music sharing in Australia?
- [ ] What do IP lawyers advise for this scenario?
- [ ] How do musicians/artists feel about friend-group sharing?
- [ ] What's the ethical line between 5 friends and 50?
- [ ] Are there existing co-op models that address this better?
- [ ] Would VPS providers terminate accounts for this?
- [ ] Is there insurance or legal protection available?
- [ ] How does this compare to Spotify family plans (legally and ethically)?
- [ ] Would transparent communication with artists change the ethics?

---

## Implementation Priority

**Priority Ranking**:
1. **Workflow 1** (Spotify Export → Purchase Mapping): High impact, clear value proposition, aligns with anti-streaming goals
2. **Workflow 2** (Discovery Platform Research): Medium impact, immediate personal use, informs current setup
3. **Workflow 3** (Shared Navidrome): Low priority, significant legal/ethical complexity, personal server sufficient for now

**Recommended Approach**:
- Start with Workflow 2 (discovery research) - immediate personal benefit
- Develop Workflow 1 as side project - potential public tool
- Defer Workflow 3 until personal setup is mature and need is clear

---

## Documentation Status

- **Workflow 1**: 📋 Documented, not researched
- **Workflow 2**: 📋 Documented, not researched
- **Workflow 3**: 📋 Documented, not researched

All workflows are **ready for future investigation** when time and interest permit.

---

*This is a living document. Add new workflows as they're identified. Update status as research progresses.*
