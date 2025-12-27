# 404Framework License Implementation Guide

**For maintainers, founders, and organizations ready to adopt transparent, sustainable open source.**

---

## Quick Start (15 minutes)

### Step 1: Choose Your Core License (5 min)

```
Do you want:

a) Maximum permissiveness + minimal complexity?
   → Use MIT (404-MIT-LICENSE.md)

b) Enterprise adoption + patent protection?
   → Use Apache 2.0 (404-APACHE2-LICENSE.md)

c) All derivatives must stay open source?
   → Use GPLv3 (not included here; use FSF's template)

d) Even SaaS wrapping must be open?
   → Use AGPLv3 (not included here; use FSF's template)
```

**Most projects should choose A or B.**

### Step 2: Create Governance (5 min)

Copy this file to your repo: [CONTRIBUTORS-TEMPLATE.md](./CONTRIBUTORS-TEMPLATE.md)

Customize:
- Replace `[PROJECT NAME]` everywhere
- Add your non-profit foundation name (or create one)
- Set voting rules (recommendation: 75% supermajority)

### Step 3: Announce Your Adoption (5 min)

Post in your README:

```markdown
## Licensing & Sustainability

[PROJECT] is licensed under [MIT/Apache 2.0].

Our licensing is designed around the **404Framework philosophy**:
- Core is always open (MIT/Apache)
- Paid features are optional services (hosting, support)
- All license changes require contributor vote
- You own your contributions; we receive a license

See [CONTRIBUTORS.md](./CONTRIBUTORS.md) for full details.

**Our Metrics** (updated quarterly):
- Active Users: [X]
- Churn Rate: [Y%]
- Project Valuation: $[Z]
- Max Acceptable Price: $[CAP]/user
- Our Actual Pricing: $[PRICE]/user

[View full metrics dashboard](LINK)
```

Done. You're now 404Framework-compliant.

---

## Detailed Implementation

### Phase 1: Pre-Announcement (1-2 weeks)

**Tasks**:

1. **Legal review**
   - Review license text with legal counsel
   - Confirm compatibility with your codebase
   - Identify any GPL dependencies (if using MIT/Apache)

2. **Create governance structure**
   - Decide: non-profit foundation or community trust?
   - Name the steward entity
   - Draft bylaws (if foundation)
   - Set voting rules (recommend 75% supermajority)

3. **Retroactive licensing**
   - If you have past contributors, reach out
   - Get written confirmation they grant the license
   - Or: re-license past contributions if you own them
   - Document in CONTRIBUTORS.md

4. **Define paid services**
   - What will you charge for? (hosting, support, custom features?)
   - Pricing tiers
   - Rollout timeline

5. **Set up metrics infrastructure**
   - Choose metrics platform (Google Sheets, Metabase, custom dashboard)
   - Define what you'll measure (users, churn, valuation)
   - Create tracking infrastructure

### Phase 2: Announcement (1 day)

**Announcement template**:

```markdown
# 404Framework Adoption: Open By Default, Sustainable By Design

We're excited to announce that [PROJECT] is adopting the 404Framework model.

## What's changing:

- **Licensing**: [PROJECT] is now [MIT/Apache 2.0] (unchanged if already open)
- **Sustainability**: New paid services: [SERVICES LIST]
- **Contributor Rights**: All contributors now have guaranteed rights (CONTRIBUTORS.md)
- **Transparency**: We're publishing quarterly metrics on users, churn, and valuation
- **Governance**: License changes require 75% contributor vote (protection against rug-pulls)

## What's staying the same:

- Your code is still free
- No paywalls for basic functionality
- You can still fork, modify, self-host, use commercially
- All past versions remain open

## Why we're doing this:

We believe open source should be sustainable without betraying community. 
See [Philosophy](https://404framework.org/Philosophy) for the full rationale.

## Questions?

Read [CONTRIBUTORS.md](./CONTRIBUTORS.md) for details, or ask us at [CONTACT].
```

### Phase 3: Rollout (2-4 weeks)

**What to do**:

1. **Merge licensing docs**
   - Add CONTRIBUTORS-TEMPLATE.md (renamed to CONTRIBUTORS.md)
   - Add LICENSE file (full text of MIT/Apache 2.0)
   - Add CONTRIBUTORS.md to README
   - Add metrics dashboard link to README

2. **Reach out to major contributors**
   - Explain the change
   - Answer questions
   - Ask for feedback

3. **Set up public metrics**
   - Create dashboard
   - Populate initial data
   - Schedule quarterly updates

4. **Begin paid services**
   - Launch pricing page
   - Announce service tiers
   - Start offering paid support

5. **Community engagement**
   - Host Q&A session
   - Write detailed blog post
   - Link to Philosophy.md
   - Answer concerns

### Phase 4: Maintenance (Ongoing)

**Quarterly tasks**:

1. **Update metrics** (by the 15th of every quarter)
   - Active user count
   - Churn rate (% users lost last quarter)
   - Project valuation (updated estimate)
   - Max acceptable price per formula
   - Actual pricing vs. cap

2. **Community check-in**
   - Post "State of the Framework" update
   - Highlight new contributors
   - Share major wins/learnings
   - Request feedback

3. **Governance review**
   - Are contributors happy with governance?
   - Any license change proposals?
   - Update voting records if applicable

4. **Pricing review**
   - Is pricing below the cap?
   - Is churn acceptable?
   - Do we need to adjust?

---

## Migration Paths from Other Models

### From Pure Open Source (MIT/Apache)

**Current state**: Open source, free, volunteer-run

**Migration**:
1. Keep the license (no change needed)
2. Add CONTRIBUTORS.md (governance)
3. Launch paid services (hosting, support, training)
4. Publish metrics
5. Ask for sponsorships

**Timeline**: 4 weeks  
**Difficulty**: Easy (least disruptive)

### From Dual Licensing (GPL + Proprietary)

**Current state**: Two licensing paths, confusing to contributors

**Migration**:
1. Choose one license:
   - Keep GPL if you want copyleft
   - Revert to MIT/Apache if you want permissive
2. Discontinue proprietary licensing (or transition customers)
3. Consolidate to single CONTRIBUTORS.md
4. Update governance
5. Simplify pricing (services, not licenses)

**Timeline**: 8-12 weeks  
**Difficulty**: Medium (requires customer migration)

### From Open Core (Crippled Free Tier)

**Current state**: Free tier artificially limited, paying for features

**Migration** (⚠️ Hard but necessary):

1. Unlock free tier features
   - Identify artificial limitations (user limits, API throttling, etc.)
   - Remove them from free version
   - This is a MAJOR trust-rebuilding move

2. Move to service-based pricing
   - Managed hosting (charge $X/month for convenience)
   - Priority support (charge $Y/month)
   - Custom features (charge $Z/engagement)
   - Professional services (charge T/hour)

3. Announce the change
   - Be explicit: "We heard you. Free tier is now complete."
   - Explain new pricing model (services, not licenses)
   - Make it a trust-rebuilding moment

4. Track churn carefully
   - Some customers may leave (that's fine)
   - Some may upgrade to services (that's better)
   - Monitor satisfaction

5. Revert any proprietary features to open source
   - Enterprise features → open source
   - Advanced plugins → open source
   - Only keep "convenience" services proprietary (hosting, support)

**Timeline**: 12-16 weeks  
**Difficulty**: Hard (requires rebuilding trust)  
**Risk**: High (customers may leave)  
**Reward**: High (community trust returns)

### From SSPL/BSL (Proprietary Pretense)

**Current state**: Fake open source, restrictive licenses, community distrust

**Migration** (⚠️ Very hard; fork likely):

1. Revert to MIT/Apache immediately
   - Choose one license
   - Apply retroactively to all past versions
   - This is a signal: "We're serious"

2. Apologize
   - Be honest about why you did it
   - Explain the economics (pressure to block cloud competitors, VC pressure, etc.)
   - Show how 404Framework solves the real problem

3. Open source everything
   - Remove all proprietary features
   - Open the "enterprise" tier
   - Move to service-based pricing only

4. Rebuild community
   - This will take time
   - Expect a fork (it may already exist)
   - Support the fork if it's better
   - Earn back trust through transparency

5. Implement full governance
   - License change voting
   - Transparent metrics
   - Contributor rights
   - Public roadmap

**Timeline**: 20+ weeks (ongoing)  
**Difficulty**: Very hard (significant trust erosion)  
**Risk**: Project fork is likely; you may lose leadership  
**Reward**: If successful, loyal community returns

---

## Metrics Dashboard: What to Measure

### Engagement Metrics

**Monthly Active Users (MAU)**
- Definition: Unique users who used the project at least once in the last month
- Calculation: COUNT(DISTINCT user_id WHERE last_active > 30 days ago)
- Why: Measures actual usage, not just downloads

**Churn Rate**
- Definition: % of users lost per month
- Calculation: (Users Lost This Month / Users Last Month) × 100%
- Why: Directly affects your max acceptable price

**Retention Curve**
- Definition: % of cohort still active after N months
- Calculation: Monthly (by cohort start date)
- Why: Reveals if users stick around

**Daily Active Users (DAU)**
- Definition: Users who actively use on any given day
- Calculation: AVERAGE(daily_unique_users)
- Why: Measures engagement depth

### Financial Metrics

**Revenue**
- Subscription revenue (monthly recurring)
- One-time revenue (custom work, training)
- Sponsorship revenue
- Donation revenue
- Total

**Expenses**
- Team salaries
- Infrastructure (hosting, CDN)
- Tools (CI/CD, monitoring)
- Marketing & community
- Total

**Profit/Loss**
- Revenue - Expenses
- Monthly and annual figures

### Product Metrics

**Issue Response Time**
- Median time from issue creation to first response
- Target: <48 hours for public projects

**Release Frequency**
- How often do you release (weekly, monthly, quarterly)?
- Tracks stability/velocity

**Open Issue Count**
- Count of open bugs, features, questions
- Trend over time
- Categorized by severity

**Test Coverage**
- % of code covered by tests
- Trend over time

### Pricing Metrics

**Max Acceptable Price (per formula)**
```
Max Price = (Valuation / Active Users) × (1 - Churn Rate)
```

**Actual Pricing**
- Cost per tier
- % of max acceptable price
- Examples:
  - Max: $50/user, Pricing: $29/user (58% of cap ✓)
  - Max: $40/user, Pricing: $79/user (198% of cap ✗ UNSUSTAINABLE)

**Customer Mix**
- % on free tier
- % on paid tier
- % on enterprise

**Pricing Justification**
- Why this price?
- How does it compare to competitors?
- What value are you adding?
- Is churn acceptable at this price?

### Governance Metrics

**Contributor Count**
- Total contributors (all-time)
- Active contributors (last 6 months)
- New contributors (this quarter)

**Contribution Distribution**
- Top 10 contributors (commit count)
- Median commits per contributor
- Shows if project is too dependent on one person

**License Change Votes** (if applicable)
- Proposals made
- Approved/rejected
- Voter turnout
- Vote distribution

---

## Template: Quarterly Metrics Report

```markdown
# [PROJECT] Quarterly Report Q[X] [YEAR]

**Reporting Period**: [DATE RANGE]  
**Report Date**: [TODAY]  
**Next Report**: [NEXT DATE]

## Engagement Metrics

| Metric | Q[X-1] | Q[X] | Change | Status |
|--------|--------|------|--------|--------|
| Monthly Active Users | [X] | [Y] | +[Z]% | ✓ On track |
| Churn Rate | [X%] | [Y%] | +[Z%] | ⚠ Rising |
| Daily Active Users (avg) | [X] | [Y] | +[Z]% | ✓ Healthy |
| New Users (cohort) | [X] | [Y] | +[Z]% | ✓ Growth |

## Financial Metrics

| Metric | Q[X-1] | Q[X] | Target |
|--------|--------|------|--------|
| Revenue | $[X] | $[Y] | $[Z] |
| Expenses | $[X] | $[Y] | $[Z] |
| Profit/Loss | $[X] | $[Y] | $[Z] |

## Product Metrics

| Metric | Target | Actual | Status |
|--------|--------|--------|--------|
| Issue Response Time | <48hr | [X]hr | ✓ On track |
| Release Frequency | Monthly | [X]/month | ✓ On track |
| Test Coverage | >80% | [X]% | ⚠ Below target |

## Pricing Analysis

```
Project Valuation: $[X]
Active Users: [Y]
Churn Rate: [Z%]

Max Acceptable Price = ($[X] / [Y]) × (1 - [Z%])
Max Acceptable Price = $[CAP]/user/month

Our Pricing:
- Free Tier: $0/user (production-ready core)
- Pro Tier: $[A]/user/month ([A/$CAP]% of cap)
- Enterprise: $[B]/user/month ([B/$CAP]% of cap)

Assessment: ✓ Sustainable / ⚠ Approaching limit / ✗ Unsustainable
```

## Key Wins This Quarter

- [MAJOR WIN 1]
- [MAJOR WIN 2]
- [CONTRIBUTION HIGHLIGHT]

## Challenges & Learning

- [CHALLENGE 1 & RESPONSE]
- [LEARNING 2]

## Community Highlights

- New contributors: [COUNT]
- Major contributions: [EXAMPLES]
- Events: [CONFERENCES, MEETUPS, HACKATHONS]

## Looking Ahead (Next Quarter)

- Roadmap priorities
- Known challenges
- Team changes
- Pricing adjustments (if any)

## Questions?

Ask us at [CONTACT] or [COMMUNITY LINK]

---

**[PROJECT] Team**
```

---

## Common Implementation Mistakes

### ❌ Mistake 1: "We'll publish metrics later"

**Problem**: Never publish. Transparency is deferred indefinitely.

**Solution**: Create the dashboard now, even if rough. Publish your first report within 30 days.

### ❌ Mistake 2: "The free tier is fine as-is"

**Problem**: If you're still artificially crippling free tier, you're still doing open core.

**Solution**: Audit free tier. Unlock all artificial restrictions. Paid tier = services, not features.

### ❌ Mistake 3: "Churn doesn't matter"

**Problem**: Churn drives your max acceptable price. Ignore it and you'll overprice.

**Solution**: Track churn monthly. If >25%, something is wrong. Fix it before scaling pricing.

### ❌ Mistake 4: "We'll do contributor governance eventually"

**Problem**: Without written governance, you're one decision away from a rug-pull accusation.

**Solution**: Write CONTRIBUTORS.md on day 1. Make license change voting binding.

### ❌ Mistake 5: "Our valuation is proprietary"

**Problem**: If you won't publish valuation, nobody believes your pricing formula.

**Solution**: Publish it. Be honest. "This is our best estimate given [ASSUMPTIONS]."

### ❌ Mistake 6: "We'll switch to VC funding later if needed"

**Problem**: VC funding changes economics. You'll need growth-at-all-costs eventually.

**Solution**: Stay bootstrapped or raise funds that align with 404Framework (impact investors, mission-driven funds).

---

## Success Metrics: How You Know It's Working

**You're succeeding if**:

✅ Contributors feel safe contributing (no rug-pull fear)  
✅ Users trust your pricing (it matches the formula)  
✅ Churn is stable or declining (<15%)  
✅ Paid services are profitable  
✅ Community is growing (more PRs, more users)  
✅ License change votes would pass (if held)  
✅ Forks are minimal (community trusts you)  

**You're failing if**:

❌ High churn (>40%)  
❌ Users leaving due to pricing concerns  
❌ License change proposals are rejected  
❌ Active forks or competing projects  
❌ Contributors worried about rug-pulls  
❌ Declining contributor count  
❌ Employees leaving (burnout, ethics)  

---

## Tools & Resources

### Free

- **Google Sheets**: Metrics tracking
- **GitHub Insights**: Usage data
- **Slack Bots**: Automated metrics collection
- **GitHub Discussions**: Community governance

### Paid

- **Metabase**: Custom dashboards
- **Amplitude/Mixpanel**: Advanced analytics
- **GitBook**: Documentation & legal docs
- **OpenCollective**: Sponsor management

### Consulting

- **Open Source Initiative (OSI)**: License guidance
- **Software Freedom Conservancy**: Legal & fiscal sponsorship
- **Open Collective**: Fiscal sponsorship
- **Local open source lawyers**: License review

---

## FAQ: Implementation

**Q: How long does this take?**  
A: 4-12 weeks depending on current state. Pure OSS → 4 weeks. SSPL → 12+ weeks.

**Q: Do I need a lawyer?**  
A: Recommended for license review, signature placement, and trademark registration. Budget $2-5K.

**Q: What if I have GPL dependencies?**  
A: MIT is compatible with GPL v3. Apache 2.0 is compatible with GPL v3 but not v2. Check your deps.

**Q: How do I incorporate the non-profit?**  
A: Depends on jurisdiction. Budget 2-8 weeks, $500-2K. Use legal services or a foundation like Software Freedom Conservancy (they offer fiscal sponsorship for $500/year).

**Q: What if contributors don't like the new model?**  
A: Listen. Maybe adjust. If they fork, support the fork if it's better. 404Framework is trustworthy by design—you'll earn them back.

**Q: How do I handle retroactive licensing?**  
A: If you own past code, you can relicense. If contributors own it, reach out and get written permission. If you can't reach them, seek legal advice.

**Q: What if someone sues about the license?**  
A: 404Framework's transparency makes lawsuits unlikely. If it happens, defend based on the written agreement.

---

## Final Checklist

Before you announce, verify:

- [ ] License text is included (full OSI-approved license)
- [ ] CONTRIBUTORS.md is written and signed off by maintainers
- [ ] Trademark is registered to non-profit (or foundation created)
- [ ] Voting rules are documented (75% supermajority recommended)
- [ ] Metrics dashboard is live
- [ ] Paid services are defined and priced
- [ ] FAQ is written
- [ ] Blog post is drafted
- [ ] Legal review is complete
- [ ] Core team has signed off
- [ ] Community is aware (soft launch)
- [ ] Major contributors are informed

Once all checked, announce to the world.

---

**You're ready. Build something people trust.**

*The 404Framework: Open by default. Sustainable by design. Never by deception.*
