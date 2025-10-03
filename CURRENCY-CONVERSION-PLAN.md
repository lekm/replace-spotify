# Currency Conversion Plan - USD to AUD

**Date**: October 3, 2025
**Exchange Rate**: 1 USD = 1.51 AUD (as of Oct 2, 2025)

---

## Current Issues

1. VPS providers (Linode, DigitalOcean, Vultr) show **USD** prices
2. Documentation doesn't clearly indicate USD vs AUD
3. Some docs show "~$7.50 AUD" for Linode but this is approximate
4. Need consistent AUD presentation for Australian user

---

## Exchange Rate Context

**Current Rate** (Oct 2, 2025):
- 1 USD = 1.51 AUD
- AUD/USD = 0.6618

**2025 Range**:
- Best: 0.6683 (Sept 16) = 1 USD = 1.497 AUD
- Worst: 0.5955 (April 8) = 1 USD = 1.679 AUD
- Average: 0.641 = 1 USD = 1.560 AUD

**Implication**: USD prices can vary ±10% in AUD terms over a year

---

## VPS Pricing - USD to AUD Conversion

### Linode
**USD**: $5.00/month (Nanode 1GB)
**AUD**: ~$7.55/month (at current rate)
**Previous Docs**: Showed "$7.50 AUD" - close but slightly off

### DigitalOcean
**USD**: $6.00/month (Regular 1GB)
**AUD**: ~$9.06/month
**Previous Docs**: Showed "$9 AUD" - approximately correct

### Vultr
**USD**: $3.50-6.00/month (depending on tier)
**AUD**: ~$5.29-9.06/month
**Previous Docs**: Showed "$9 AUD" - only for high-frequency tier

### OVHcloud ✅
**Native AUD**: $6.12-9.52 ex GST ($6.73-10.47 inc GST)
**No conversion needed** - priced in A$ on Australian site

---

## Recommended Updates

### 1. VPS Comparison Tables

**Add currency conversion notes**:
```markdown
| Provider | Monthly (AUD) | Notes |
|----------|---------------|-------|
| OVHcloud VPS-1 | $6.73 (inc GST) | ✅ Native AUD pricing |
| Linode Nanode | ~$7.55 | USD $5 converted at Oct 2025 rate |
| DigitalOcean | ~$9.06 | USD $6 converted at Oct 2025 rate |
| Vultr Regular | ~$5.29-7.55 | USD $3.50-5 converted |
```

### 2. Add Exchange Rate Disclaimer

Add to all documents with VPS pricing:
```markdown
**Exchange Rate Note**: Linode, DigitalOcean, and Vultr prices are shown
in USD on their websites. AUD equivalents shown here are converted at the
October 2025 rate (1 USD = 1.51 AUD) and will fluctuate with exchange rates.
OVHcloud prices are native AUD and fixed.
```

### 3. Annual Cost Calculations

Update to show AUD:

**Current (Mixed Currencies)**:
- Linode: "$5/month" (ambiguous)
- OVHcloud: "$6.73/month" (AUD)

**Proposed (All AUD)**:
- Linode: ~$7.55 AUD/month = ~$90.60/year
- OVHcloud VPS-1: $6.73 AUD/month = $80.76/year

### 4. Recommendations Update

**Current Recommendation**:
> "OVHcloud or Linode for best value"

**Updated Recommendation**:
> "OVHcloud VPS-1 offers best value at $6.73 AUD/month (native pricing, no
> exchange rate risk). Linode at ~$7.55 AUD/month is competitive but prices
> vary with USD/AUD exchange rate."

---

## Files Requiring Updates

### High Priority (Public-Facing)
- [ ] README.md - VPS comparison
- [ ] index.html - Cost tables
- [ ] master-project-documentation.md - VPS analysis section
- [ ] navidrome-setup-guide.md - Cost comparison table
- [ ] navidrome-setup-guide.html - Cost tables

### Medium Priority
- [ ] lidarr-discogs-workflow.md - Annual cost comparisons
- [ ] spotify-alternatives-report.html - Any VPS mentions

### Updates Needed in sources.md
- [ ] Add note about exchange rate source
- [ ] Add disclaimer about USD conversion methodology

---

## Proposed Standard Format

For consistency across all docs:

### VPS Pricing Format
```
**OVHcloud VPS-1**: $6.73 AUD/month (inc GST)
- Native AUD pricing, no exchange rate risk
- Source: [OVHcloud Australia](https://www.ovhcloud.com/en-au/vps/)

**Linode Nanode 1GB**: ~$7.55 AUD/month*
- *USD $5/month, converted at Oct 2025 rate (1 USD = 1.51 AUD)
- Subject to exchange rate fluctuations
- Source: [Linode Pricing](https://www.linode.com/pricing/)
```

### Cost Comparison Format
```
| Provider | AUD/Month | AUD/Year | Currency Risk |
|----------|-----------|----------|---------------|
| OVHcloud VPS-1 | $6.73 | $80.76 | None (native AUD) |
| Linode Nanode | ~$7.55 | ~$90.60 | Yes (USD pricing) |
```

---

## Benefits of This Approach

1. **Transparency**: Clear about which prices are native vs converted
2. **Accuracy**: User knows exact AUD costs at time of documentation
3. **Risk Awareness**: User aware that USD prices may vary
4. **Consistency**: All costs in user's home currency (AUD)
5. **Decision Making**: Can make true apples-to-apples cost comparisons

---

## Exchange Rate Monitoring

Going forward:
- Check exchange rates **quarterly** when updating VPS pricing
- Note significant changes (>10% movement) in documentation
- Consider OVHcloud's fixed AUD pricing as an advantage in documentation

---

## Example Updates

### Before (Ambiguous)
```
- Linode: $7.50/month
- OVHcloud: $6.73/month
```

### After (Clear)
```
- OVHcloud VPS-1: $6.73 AUD/month (native pricing)
- Linode Nanode: ~$7.55 AUD/month (USD $5 at Oct 2025 rates)

*USD prices subject to exchange rate fluctuations*
```

---

## Decision Points

**Option A: Show USD with AUD Conversion**
```
Linode: $5 USD (~$7.55 AUD at Oct 2025 rates)
```
Pros: Shows original price, user can recalculate
Cons: More verbose

**Option B: Show AUD with Footnote** ⭐ RECOMMENDED
```
Linode: ~$7.55 AUD*
*USD pricing converted at Oct 2025 rate
```
Pros: Cleaner, user sees what they'll pay
Cons: May drift from reality over time

**Option C: Range for USD Prices**
```
Linode: $7-8 AUD (varies with exchange rates)
```
Pros: Accounts for variability
Cons: Less precise

**RECOMMENDATION: Option B** - Shows AUD equivalent clearly with footnote explaining conversion

---

Ready to proceed with these updates?
