# Navidrome Complete Setup Guide

## What is Navidrome?

Navidrome is a lightweight, self-hosted music streaming server that transforms your personal music collection into your own private streaming service. Think of it as running your own Spotify, but with music you actually own, complete privacy, and no corporate tracking.

---

## Hardware Requirements & Hosting Options

### VPS Hosting (Recommended for Good Uptime)

**Yes, you can absolutely use Navidrome on a VPS!** This is actually recommended for reliable uptime and remote access.

#### Minimum VPS Specifications
- **RAM**: 1GB (minimum) - Navidrome uses ~130MB while idle
- **CPU**: 1 vCPU (sufficient for personal use)
- **Storage**: 20GB+ (10GB system + your music library)
- **Bandwidth**: 1TB/month (adequate for personal streaming)

#### Recommended VPS Specifications
- **RAM**: 2-4GB (better for multiple users and large libraries)
- **CPU**: 1-2 vCPU
- **Storage**: 50GB+ (depends on music collection size)
- **Bandwidth**: 2TB+/month

#### Essential Requirements
- **FFmpeg**: Required for audio transcoding
- **SSD Storage**: Much better performance than HDD
- **IPv4 Address**: For remote access

### VPS Cost Comparison (2025)

| Provider | RAM | CPU | Storage | Bandwidth | Cost/Month (AUD) | Ethics Score |
|----------|-----|-----|---------|-----------|------------------|-------------|
| **OVHcloud VPS-1** | 8GB | 4 vCPU | 75GB SSD NVMe | 400 Mbps | **$6.73** (inc GST) | 8/10 |
| **OVHcloud VPS-2** | 12GB | 6 vCPU | 100GB SSD NVMe | 1 Gbps | **$10.47** (inc GST) | 8/10 |
| Linode | 1GB | 1 vCPU | 25GB SSD | 1TB | $7.50 | 7/10 |
| DigitalOcean | 1GB | 1 vCPU | 25GB SSD | 1TB | $9 | 5/10 |
| Vultr | 1GB | 1 vCPU | 25GB SSD | 1TB | $9 | 6/10 |

---

## Ethical Analysis & Melbourne Latency Considerations

### Corporate Ethics Comparison (2024)

#### **Linode/Akamai - Mixed Record (Ethics Score: 7/10)**
- **Positive**: No major controversies found, stable service record
- **Concern**: Acquired by Akamai (large US tech company) in 2022
- **Tax**: Now charges Australian sales tax (compliance, not avoidance)
- **Labor**: No significant labor issues found

#### **DigitalOcean - Concerning Practices (Ethics Score: 5/10)**
- **Major Issues**: Laid off 200 employees (11% of workforce) in 2023
- **Problematic**: "Promises were made, but in the end not honored"
- **Labor Practices**: Moving hiring to lower-wage countries (Pakistan, Mexico)
- **Employee Feedback**: "Pure greed play, nothing more" - multiple negative reviews
- **Leadership**: Ongoing instability with executive departures

#### **Vultr - Recent Controversy (Ethics Score: 6/10)**
- **2024 Issue**: Controversial terms claiming "perpetual, irrevocable" rights to user content
- **Resolution**: Quickly removed after public outcry
- **Assessment**: Concerning initial overreach but responsive to feedback

### Latency from Melbourne Australia

#### **Asia-Pacific Server Locations**
- **Vultr**: 32 global regions including Sydney, Singapore, Tokyo
- **DigitalOcean**: 13 data centers including Singapore
- **Linode**: 11 data centers, limited APAC presence

#### **Performance from Melbourne (2024 Testing)**
- **Vultr**: 359-382ms average response time, largest APAC network
- **DigitalOcean**: 365-405ms average response time
- **Linode**: 368-400ms average response time

**Latency Verdict**: Only 10-20ms difference between providers - **negligible for music streaming**

### Australian VPS Alternatives (Data Sovereignty)

#### **Why Consider Australian Hosting?**
- **2024 Privacy Act Updates**: New government requirements for data sovereignty
- **US CLOUD Act Concerns**: American companies can be forced to hand over data
- **Local Compliance**: Easier adherence to Australian privacy laws

#### **Australian VPS Providers**

##### **OVHcloud Australia** (Recommended Australian Option)
- **Location**: Sydney datacenter
- **Data Sovereignty**: Meets local residency requirements
- **Cost**: $6.12-9.52/month ex GST ($6.73-10.47 inc GST)
- **Specs**: VPS-1: 8GB RAM, 4 vCPU, 75GB SSD | VPS-2: 12GB RAM, 6 vCPU, 100GB SSD
- **Ethics**: European company, no major controversies
- **Performance**: Excellent for Australian users

##### **Other Australian Options**
- **Swift Digital**: ISO 27001 accredited, Australian-owned
- **Servers Australia**: Local data sovereignty focus
- **Macquarie Data Centres**: Government-certified strategic provider

### Updated Recommendation Based on Ethics + Location

#### **For Maximum Ethics + Australian Data Sovereignty**
**Primary**: **OVHcloud Australia VPS-1** (~$6.73/month inc GST)
- Local data protection under Australian law
- European company with better privacy record
- Excellent latency for Melbourne users
- Meets 2024 data sovereignty requirements

#### **For Best Value + Acceptable Ethics**
**Primary**: **Linode** ($5/month)
- Cleanest record of the major US providers
- Adequate latency (only 20ms worse than local)
- Proven reliability and performance
- Most cost-effective option

#### **Avoid for Ethical Reasons**
- **DigitalOcean**: Poor treatment of employees, problematic labor practices
- **Vultr**: Content rights overreach (though resolved)

### Local Hardware Options

#### Budget Option: Raspberry Pi
- **Cost**: $50-100
- **Pros**: Very low power consumption, silent operation
- **Cons**: Limited by home internet uptime, requires port forwarding
- **Good for**: Testing, personal use only

#### Mid-Range: Intel NUC or Mini PC
- **Cost**: $200-500
- **Pros**: More powerful, can run multiple services
- **Cons**: Higher power consumption, still tied to home internet
- **Good for**: Home lab enthusiasts

#### High-End: Dedicated Server
- **Cost**: $500+
- **Pros**: Maximum control and performance
- **Cons**: Highest cost, requires technical knowledge
- **Good for**: Tech enthusiasts with large collections

---

## Multi-User Sharing & Family Accounts

### Multi-User Capabilities

**Yes, Navidrome supports multiple users!** Each user gets:
- Individual playlists and favorites
- Personal play counts and listening history
- Separate user accounts with different permissions
- Their own customized experience

### Multi-Library Support for Families

Navidrome's multi-library feature is perfect for family setups:

#### How It Works
- **Separate Libraries**: Create different music libraries for each family member
- **Access Control**: Admin controls which users can access which libraries
- **Library Switching**: Users can switch between accessible libraries in the UI
- **Privacy**: Users only see music from libraries they have permission to access

#### Example Family Setup
```
Family Navidrome Server
├── Dad's Rock Collection (Dad access only)
├── Mom's Jazz Library (Mom access only)
├── Kids' Music (Kids access only)
└── Shared Family Library (Everyone access)
```

### User Roles & Permissions

#### Admin Users
- Access to all libraries automatically
- Can create and manage other users
- Can assign library permissions
- Full system configuration access

#### Regular Users
- Must be explicitly granted library access
- Can only see their assigned libraries
- Cannot create other users
- Limited configuration access

### Current Limitations

**Sharing Feature**: If enabled, all users have equal sharing capabilities. There's currently no granular sharing permissions per user.

---

## Cost Analysis: VPS vs Local Hardware

### VPS Hosting Costs (Annual)

#### OVHcloud VPS-1 (Best Value - $6.73/month inc GST)
- **Year 1**: $81 + music purchases
- **Year 2**: $81 + music purchases
- **5 Years**: $405 + music purchases

#### Linode 1GB Plan ($7.50/month AUD)
- **Year 1**: $90 + music purchases
- **Year 2**: $90 + music purchases
- **5 Years**: $450 + music purchases

#### Benefits of VPS
- **99.9% uptime** (much better than home internet)
- **No electricity costs** (server power included)
- **No hardware maintenance** (provider handles this)
- **Professional internet** (fast, reliable connection)
- **Remote access built-in** (no port forwarding needed)
- **Automatic backups** (most providers offer this)

### Local Hardware Costs

#### Raspberry Pi Setup
- **Initial**: $80 (Pi + accessories)
- **Annual electricity**: $10-20
- **5 Years**: $130-180 + music purchases

#### Intel NUC Setup
- **Initial**: $350 (mid-range NUC)
- **Annual electricity**: $30-50
- **5 Years**: $500-600 + music purchases

### Winner: VPS for Reliability

For your use case (heavy CarPlay usage, need for good uptime), **VPS is recommended** because:
- Home internet outages won't affect your music
- No need to configure home router/firewall
- Better performance and reliability
- Professional-grade infrastructure

---

## Storage Considerations

### Music Library Size Planning

| Collection Size | Storage Needed | Recommended VPS |
|----------------|----------------|-----------------|
| Small (1,000 songs) | 5-10GB | 25GB VPS |
| Medium (5,000 songs) | 25-50GB | 80GB VPS |
| Large (20,000 songs) | 100-200GB | 320GB VPS |
| Audiophile (FLAC) | 2-5x above sizes | Custom storage |

### Music Format Recommendations

#### For VPS Storage Efficiency
- **MP3 320kbps**: Good quality, reasonable file sizes
- **MP3 V0**: Variable bitrate, excellent quality/size ratio
- **FLAC**: Best quality but large files (use for favorites only)

#### For Vinyl Rips
- **FLAC**: Preserve the full quality of your vinyl
- **Separate library**: Keep vinyl rips in dedicated library
- **Metadata**: Tag with pressing details, catalog numbers

---

## Setup Process Overview

### Phase 1: VPS Setup
1. **Choose Provider**: Linode recommended ($5/month)
2. **Deploy Server**: Ubuntu 22.04 LTS recommended
3. **Secure Server**: SSH keys, firewall, fail2ban
4. **Install Dependencies**: Docker, FFmpeg

### Phase 2: Navidrome Installation
1. **Docker Compose Setup**: Easiest installation method
2. **Configuration**: Set music folder, database location
3. **First Run**: Create admin account
4. **SSL Setup**: Use Let's Encrypt for HTTPS

### Phase 3: Music Library Setup
1. **Upload Music**: Transfer your collection to VPS
2. **Organize Libraries**: Create separate libraries for family
3. **User Management**: Create accounts for family members
4. **Permissions**: Assign library access per user

### Phase 4: Client Setup
1. **iOS Apps**: Install play:Sub or Amperfy
2. **CarPlay Configuration**: Set up for reliable car use
3. **Home Integration**: Configure for WiiM Pro Plus
4. **Backup Strategy**: Regular library backups

---

## Integration with Your Current Setup

### CarPlay Integration
- **play:Sub**: $10, excellent CarPlay support, more reliable than Qobuz
- **Amperfy**: Free, good but limited CarPlay navigation
- **Offline Mode**: Download songs for areas with poor cell coverage

### WiiM Pro Plus Integration
- **Subsonic API**: WiiM should support this directly
- **Full Hi-Res**: Maintain FLAC quality throughout
- **Control**: Use iPhone app to control WiiM playback

### Record Collection Integration
- **Vinyl Rips**: Add high-quality digital versions of your records
- **Metadata**: Tag with pressing info, catalog numbers, personal notes
- **Organization**: Mix digital purchases with vinyl rips
- **Discovery**: Rediscover forgotten albums in your collection

---

## Security & Privacy Considerations

### VPS Security
- **SSH Key Authentication**: Disable password login
- **Firewall**: Only open necessary ports (80, 443, SSH)
- **Fail2Ban**: Prevent brute force attacks
- **Regular Updates**: Keep system and Navidrome updated

### Privacy Benefits
- **No Tracking**: Your listening habits stay private
- **No Ads**: Commercial-free music experience
- **Data Control**: Your music, your server, your rules
- **No Censorship**: Music can't be removed by licensing changes

---

## Recommended Setup for Your Needs

### Optimal Configuration
- **VPS**: Linode 1GB ($5/month) to start
- **Storage**: Upgrade as collection grows
- **iOS App**: play:Sub for best CarPlay experience
- **Libraries**: Separate for your collection + shared family library
- **Backup**: Weekly automatic backups of music and database

### Migration Strategy
1. **Start Small**: Set up VPS with core collection
2. **Test CarPlay**: Ensure play:Sub works reliably in car
3. **Expand Gradually**: Add more music as you go
4. **Family Integration**: Add other users once system is stable

### Total First Year Cost
- **VPS Hosting**: $60 (Linode 1GB)
- **play:Sub App**: $10 (one-time)
- **Domain**: $15 (optional, for easy access)
- **Music Purchases**: Variable (your choice)
- **Total**: ~$85 + music purchases

This setup gives you professional-grade music streaming with complete privacy, excellent CarPlay integration, and alignment with your leftist values by reducing dependence on corporate streaming services.