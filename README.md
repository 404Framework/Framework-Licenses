# 404Framework Licenses

A collection of licenses designed with the 404Framework philosophy in mind—built for **openness without collapse**, **fair pricing**, and **sustainable community-driven development**.

**Start here**: [INDEX.md](./INDEX.md) for navigation and quick decisions  
**Full philosophy**: [Philosophy](https://404framework.org/Philosophy)

---

## The 404Framework Philosophy

The 404Framework rejects both the false choice of unsustainable pure open source and proprietary rug-pulls. Instead, it advocates for:

- **Free access to production-ready cores** (MIT, Apache 2.0)
- **Value-based pricing** tied to measurable engagement and churn
- **Transparent economics** with public metrics and accountability
- **Rug-pull insurance** through contributor rights and license change governance
- **No tricks**: No SSPL, no BSL, no artificial crippling of free tiers

See [Philosophy](https://404framework.org/Philosophy) for the complete framework.

## Supported Licenses

Licenses in this collection are vetted against the 404Framework principles:

### Core Framework Licenses (Tier 1: Production-Ready, Freely Accessible)

These licenses are **OSI-approved**, **perpetual**, and **unrestricted** for all users. Use these for your framework core.

| License        | Use Case                                   | Key Terms                                                                          |
| -------------- | ------------------------------------------ | ---------------------------------------------------------------------------------- |
| **MIT**        | Maximally permissive                       | No restrictions; can be proprietary downstream                                     |
| **Apache 2.0** | Permissive with patents                    | Includes explicit patent grant; can be proprietary downstream                      |
| **GPL v3**     | Copyleft (everything must stay open)       | Derivative works must use GPL v3; no proprietary downstream                        |
| **AGPL v3**    | Network copyleft (all use is distribution) | Even SaaS users trigger copyleft; requires commercial license for proprietary SaaS |

**Decision Tree**:

- **No restrictions, maximum reusability?** → MIT
- **Need explicit patent protection?** → Apache 2.0
- **Derivatives must stay open, proprietary downstream not allowed?** → GPL v3
- **SaaS must also be open (no proprietary cloud wrappers)?** → AGPL v3

### Rejected Licenses (Tier 4: Fake Open Source)

These licenses **contradict the 404Framework** because they restrict usage or claim openness while imposing proprietary terms.

| License                     | Why Rejected                                                                                             |
| --------------------------- | -------------------------------------------------------------------------------------------------------- |
| **SSPL (Mongo)**            | Claims "open source" while blocking commercial use. Not OSI-approved.                                    |
| **BSL (Elastic/HashiCorp)** | Source-available trap: proprietary before release date, licensing afterward. Creates artificial lock-in. |
| **RSAL (Redis)**            | Restricts cloud provider use. Proprietary in all but name.                                               |
| **Commons Clause**          | Prohibits selling software (permits donations). Artificial revenue gatekeeping.                          |
| **Custom Proprietary**      | Invented licenses with no community backing. No legal certainty.                                         |

**Why they fail**: They all share the same structure: "we promise openness, but we reserve the right to block your use case." This replicates the exact dynamics that lead to rug-pulls.

---

## License Design Principles for 404Framework Projects

When building a framework under 404Framework principles, follow these rules:

### 1. Core License = OSI-Approved Open Source

- Your core product must use MIT, Apache 2.0, GPL v3, or AGPL v3
- No invented licenses
- No "source available" variants (BSL, SSPL, RSAL)
- License cannot change without 75% contributor vote

### 2. Paid Features ≠ License Restrictions

- Monetization happens through **services**, not license restrictions
- Free tier = production-ready, complete core
- Paid tier = convenience (managed hosting, support, integrations)
- Never artificially cripple free features to force paid upgrades (that's open core)

### 3. Dual Licensing Only If Necessary, Single License Preferred

If you use dual licensing (e.g., AGPL free + proprietary paid):

- Be explicit: clearly communicate which users need commercial licenses
- Make the free license genuinely open (AGPL or stronger copyleft)
- Document the exact commercial restrictions
- Provide a clear path to commercial licensing (no gatekeeping)

**Note**: Single-license projects (MIT/Apache) are strongly preferred. Dual licensing creates contributor confusion and legal ambiguity.

### 4. Contributor Rights Must Be Guaranteed

Every 404Framework project must document:

- **Copyright**: Contributors retain copyright; you receive a license grant, not ownership transfer
- **No CLA**: Optional contributor agreements that don't sign away rights
- **License change voting**: Any core license change requires 75% contributor approval
- **Fork rights**: Contributors can always fork under the original license
- **Public transparency**: License text, voting records, and changes are public

Create a `CONTRIBUTORS.md` outlining these rights. Make it legally binding.

### 5. Trademark Protection (Not Corporate Ownership)

- Trademark held by a **non-profit foundation** or **community trust**, not a for-profit entity
- Prevents hostile takeovers (Redis-style)
- Prevents "community edition" vs "enterprise edition" splitting
- Cannot be used to force commercial licensing

### 6. Transparency Requirements

Every 404Framework project must publish quarterly:

- Active user count
- Churn rate (% of users lost per period)
- Current project valuation
- Max acceptable price per the formula: `(Valuation / Users) × (1 - Churn Rate)`
- Actual pricing vs. the calculated cap
- Reasoning for any pricing changes

This prevents the "we need to be sustainable" excuse from triggering rug-pulls.

---

## Creating a 404Framework License

Follow this template when designing a license under 404Framework principles:

```markdown
# [Project Name] License

## Core Terms

This [Project] is made available under the [LICENSE NAME] (full text below).

The [PROJECT] core is freely available to:

- Individuals and organizations
- For-profit and non-profit use
- Derivative works and modifications
- Commercial deployment

With the following requirements:

- [License obligations: e.g., attribution, source availability]

## Paid Services

The [PROJECT] team offers paid services, separate from the license:

- Managed hosting
- Priority support
- Training and consulting
- Custom feature development

Using the core framework does not require purchasing paid services.
Paid services are optional enhancements.

## License Change Governance

Changes to this license require:

1. Public proposal with 30-day comment period
2. Contributor vote (weighted by contribution volume)
3. 75% supermajority approval
4. If approved, the new license applies only to future versions
5. All past versions remain under the original license

Contributors have the right to fork under the original license if the change is rejected.

## Trademark

[PROJECT] trademark is held by [NON-PROFIT FOUNDATION/COMMUNITY TRUST].

The trademark cannot be used to:

- Force commercial licensing
- Block derivative projects
- Create false "official" vs "community" editions

## Full License Text

[Include full OSI-approved license text: MIT, Apache 2.0, GPL v3, or AGPL v3]
```

---

## Comparison: Industry License Approaches

| Model            | Example          | Sustainability   | Community Trust | Legal Clarity          |
| ---------------- | ---------------- | ---------------- | --------------- | ---------------------- |
| **Pure OSS**     | Linux kernel     | ❌ Burnout risk  | ✅ High         | ✅ Clear               |
| **404Framework** | To be built      | ✅ Fair pricing  | ✅ High         | ✅ Clear               |
| **Dual-license** | MySQL, Grafana   | ⚠️ Possible      | ⚠️ Confused     | ⚠️ Ambiguous           |
| **Open Core**    | Elastic, Datadog | ⚠️ Artificial    | ⚠️ Eroded       | ⚠️ Deceptive           |
| **SSPL/BSL**     | MongoDB, Redis   | ❌ Drives forks  | ❌ Destroyed    | ❌ Pretends to be open |
| **Freemium**     | Most SaaS        | ✅ Maximized     | ❌ Exploited    | ✅ Clear               |
| **VC-backed OS** | Most startups    | ❌ Rug-pull risk | ❌ Exit-driven  | ❌ No guarantees       |

---

## Using These Licenses

### If You're Starting a New Project

1. **Choose your core license**: MIT (simplest), Apache 2.0 (with patents), GPL v3 (copyleft), or AGPL v3 (network copyleft)
2. **Define your paid services**: What adds value without restricting the free tier?
3. **Document contributor rights**: Use the template in `CONTRIBUTORS.md`
4. **Publish your economics**: Valuation, users, churn, pricing cap, actual pricing
5. **Set up governance**: License change voting, trademark protection, fork rights

### If You're Migrating From Another Model

- **SSPL/BSL to 404Framework**: Revert core to MIT/Apache; keep paid services the same
- **Proprietary to 404Framework**: Open-source the core; maintain paid services for SaaS hosting/support
- **Confusing dual-license to 404Framework**: Unify to one OSI-approved license; make commercial licensing optional and transparent

### If You're Evaluating a Framework

Ask:

1. Is the core OSI-approved open source? (MIT, Apache, GPL, AGPL only)
2. Does it have a complete, production-ready free tier?
3. Are contributor rights documented and protected?
4. Do they publish metrics on users, churn, and pricing?
5. Is the license changeable without community vote?

If the answer is "no" to any of these, it's not truly 404Framework compliant.

---

## Resources

- **[Philosophy](https://404framework.org/Philosophy)**: Complete 404Framework philosophy and economic model
- **About Us**: Organization details and governance
- **OSI Licenses**: https://opensource.org/licenses/
- **Contributor License Agreements**: https://www.apache.org/licenses/individual-cla.pdf

---

## Contributing

Have a 404Framework-aligned license to add? Or identified a gap in this framework?

1. Create a pull request with your proposal
2. Include reasoning for why the license aligns with 404Framework principles
3. Ensure it's OSI-approved or explain why custom terms are necessary
4. Cite real-world projects using the license

---

**The 404Framework: Building what couldn't be found.**

_Because the best licenses are the ones that never betray you._
