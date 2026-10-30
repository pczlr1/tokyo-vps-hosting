# tokyo vps hosting: BandwagonHost's Tokyo plans compared — CN2 GIA pricing, real costs, and how to pick without overpaying

Shopping for a Tokyo VPS usually means one of two very different trips. If you just need a server physically in Japan and your visitors are in the US or Europe, budget providers start around $4 a month and you're done in five minutes. If your visitors are in mainland China and you care about stable evening routing, the picture changes completely: you're shopping for premium network quality, and BandwagonHost's Tokyo CN2 GIA line — starting at $89.99/month at Tokyo Equinix TY8 — is one of the few established options on that shelf.

This article walks through both sides: what BandwagonHost actually sells in Tokyo, what each plan really costs over a year, where cheaper Tokyo competitors make more sense, and the limits that only show up once you're already at checkout.

> **Quick picks**
> - Visitors in mainland China, want stable telecom/unicom/mobile routing: **Tokyo CN2 GIA 40G** — 2 vCPU, 2 GB RAM, 40 GB SSD, 500 GB traffic, $89.99/mo or $899.99/yr. 👉 [Check the Tokyo CN2 GIA 40G plan and current stock](https://bandwagonhost.com/aff.php?aff=74518&pid=108)
> - Audience mostly outside China: a budget Tokyo host from $4–21/mo will do the job; skip the CN2 GIA premium entirely.
> - Want Tokyo-level latency on a budget: BandwagonHost's Osaka CN2 GIA starts at $49.99/mo — same network family, lower price.

## The two Tokyo products BandwagonHost sells (they are not interchangeable)

BandwagonHost runs two separate Tokyo product lines, and mixing them up is the most common mistake in reviews of this host:

**1. Tokyo CN2 GIA (JPTYO_8, Equinix TY8 datacenter).** Return traffic from all three Chinese carriers — China Telecom, China Unicom, and China Mobile — rides China Telecom's CN2 GIA network (AS4809), with outbound traffic prioritized on the same network. Six plans, 1.2 Gbps port on every tier, launched in November 2021. This is the premium option.

**2. The Tokyo Plan series (DC39 / DC39v2).** Limited-edition plans routed over CMI, China Mobile International's direct network. The current v2 flagship gives you 2 AMD cores, 2 GB RAM, 40 GB NVMe SSD, 1 TB traffic, and a 5 Gbps port for **$99/year**. A smaller basic version (1 core, 1 GB, 20 GB SSD, 500 GB traffic, 2.5 Gbps) has appeared at $79/year. Stock comes and goes; when it's gone, it's gone.

The routing difference matters more than the spec sheets suggest. CN2 GIA is China Telecom's premium transit product — market pricing for raw CN2 GIA IP transit reportedly runs up to $120 per Mbps, which is why plans built on it cost six times more than comparable US-based plans. CMI routing on the Tokyo Plan is cheap and fast, but independent testing found its weak spot: during the 10–11 pm China evening peak, packet loss fluctuates noticeably. On the CN2 GIA side, third-party tests (AMD EPYC Genoa nodes) measured 60–80 ms from the Shanghai/Jiangsu-Zhejiang region, near-zero packet loss at midday, and only scattered losses on a few routes at 11 pm.

Translation: if absolute evening stability matters, pay for CN2 GIA. If you can tolerate some peak-hour jitter and want 5 Gbps of port for the price of a dinner, The Tokyo Plan v2 at $99/year is the better deal — when you can get it.

## Full Tokyo CN2 GIA plan and price table

All plans sit in Tokyo Equinix TY8, run KVM virtualization on BandwagonHost's in-house KiwiVM panel, and share the same **1.2 Gbps port speed**. Prices in USD:

| Plan | Specs (CPU / RAM / SSD) | Traffic /mo | Monthly | Annual | Order |
| --- | --- | --- | --- | --- | --- |
| Tokyo CN2 GIA 40G | 2 cores / 2 GB / 40 GB RAID-10 | 500 GB | $89.99 | $899.99 | [ Order the 40G plan](https://bandwagonhost.com/aff.php?aff=74518&pid=108) |
| Tokyo CN2 GIA 80G | 4 cores / 4 GB / 80 GB | 1 TB | $155.99 | $1,559.99 | [ Order the 80G plan](https://bandwagonhost.com/aff.php?aff=74518&pid=109) |
| Tokyo CN2 GIA 160G | 6 cores / 8 GB / 160 GB | 2 TB | $299.99 | $2,999.99 | [ Order the 160G plan](https://bandwagonhost.com/aff.php?aff=74518&pid=110) |
| Tokyo CN2 GIA 320G | 8 cores / 16 GB / 320 GB | 4 TB | $589.99 | $5,899.99 | [ Order the 320G plan](https://bandwagonhost.com/aff.php?aff=74518&pid=111) |
| Tokyo CN2 GIA 640G | 10 cores / 32 GB / 640 GB | 6 TB | $989.99 | $9,989.99 | [ Order the 640G plan](https://bandwagonhost.com/aff.php?aff=74518&pid=123) |
| Tokyo CN2 GIA 1280G | 12 cores / 64 GB / 1280 GB | 8 TB | $1,889.99 | $18,989.99 | [ Order the 1280G plan](https://bandwagonhost.com/aff.php?aff=74518&pid=125) |

Quarterly and semi-annual billing also exists — the 40G plan runs $249.99/quarter and $479.99/semi-annual — and you'll see every cycle's price on the order page before paying.

The limited-edition **The Tokyo Plan v2** (DC39v2, CMI routing, 2 AMD cores / 2 GB / 40 GB NVMe / 1 TB traffic / 5 Gbps, $99/year) is sold separately and frequently out of stock: [👉 check availability for The Tokyo Plan v2](https://bit.ly/BandwaGon).

One detail almost every comparison table skips: **the port speed never changes.** The $89.99 entry plan and the $1,889.99 top plan both cap at 1.2 Gbps. Paying more buys CPU, RAM, storage, and traffic — nothing else. If your goal is raw speed, the cheapest tier already has it.

## What a Tokyo plan actually costs over a year

Sticker price is only half the story. Two numbers decide your real cost.

**Annual vs monthly billing.** Monthly billing on the 40G plan runs $89.99 × 12 = $1,079.88. Annual billing is $899.99 — a **$179.89 difference, roughly 17% off**. If you're keeping the server longer than a few months, annual is the obvious call. The gap holds proportionally across every tier.

**The coupon.** The code **BWHCGLUKKB** applies a recurring discount of roughly 6.6% that, per multiple independent guides tracking it through mid-2026, also applies at renewal — on an $899.99 annual plan that's about $60 back, every year. You enter it in the cart's promotional code field and click Validate before checkout; the discount shows immediately. Two caveats: older codes like BWH26FXH4II were officially retired during the 2025 Double 11 event, so don't copy codes from two-year-old blog posts, and always confirm the code actually validates on the checkout page — availability of promo codes changes without notice. 👉 [Open the cart with the 40G plan pre-selected and test the code](https://bandwagonhost.com/aff.php?aff=74518&pid=108)

Renewal pricing matches your original purchase price on these plans — the annual rate doesn't jump after year one, which is worth confirming on the order page but is how BandwagonHost's recurring billing has behaved across its lineup.

## How BandwagonHost's Tokyo plans compare with cheaper Tokyo hosts

To be fair to the market: BandwagonHost is nowhere near the cheapest way to get a server in Tokyo. Here's what verified competitors currently list (information only):

| Host | Tokyo starting price | Entry config | Notes |
| --- | --- | --- | --- |
| OliveVPS | $3.99/mo | 1 vCPU, 1 GB RAM, 25 GB NVMe, 1 TB traffic, 1 Gbps | Tier III facility, 24/7 staffed |
| ExtraVM | $4.50/mo | 1 GB RAM KVM NVMe, scales to 64 GB | DDoS-protected Tokyo line |
| LightNode | $21.2/mo | 2 GB RAM, 1 dedicated vCPU, 50 GB NVMe | Hourly billing available, Windows & Linux support |
| BandwagonHost | $89.99/mo | 2 cores, 2 GB, 40 GB, 500 GB traffic | CN2 GIA routing to all three Chinese carriers |

That price gap is enormous, and for most use cases the cheap options are genuinely fine. A blog serving North American readers gains nothing from CN2 GIA. Where the comparison flips is routing: budget Tokyo hosts sell you a server in Japan, but the path your packets take back to China runs over congested public transit — on ordinary 163-routed lines, evening packet loss can climb past 30%. CN2 GIA is the dedicated express lane, and you pay express-lane prices for it. If China routing isn't your problem, the $4–21/month column is the rational choice and there's no shame in it.

Also worth knowing within BandwagonHost's own catalog: Osaka CN2 GIA starts at $49.99/mo ($499.99/yr) with a 1.5 Gbps port, and the Los Angeles CN2 GIA-E line offers 10+ datacenters, 2.5 Gbps, and 1 TB traffic from $169.99/year. Official guidance itself suggests the US E-Commerce plans when latency isn't critical.

## Who should (and shouldn't) buy a Tokyo CN2 GIA plan

Good fits, based on what the routing and specs actually deliver:

- Websites and lightweight apps serving mainland China visitors, where telecom, unicom, and mobile all need decent evening performance
- Cross-border development/testing environments, remote work nodes, code repositories, small databases, or APIs where a stable China path matters
- Anyone who needs full root access and self-managed infrastructure in Japan with serious network quality

Poor fits:

- Sites whose audience lives in North America or Europe — you're paying a 6–20x premium for routing you'll never use
- High-traffic media or large-file distribution on the 40G tier: 500 GB/month disappears fast, and CN2 GIA capacity isn't built for bulk delivery
- Anyone expecting managed hosting. Every BandwagonHost plan is strictly self-managed: OS updates, SSH hardening, backups of your application data, and traffic monitoring are all on you
- DDoS-exposed workloads. CN2 GIA's capacity is limited, and when a plan gets attacked, the IP is null-routed (blackholed) rather than filtered. If your project attracts attacks, this line will hurt

## Limits to know before you click order

These come from BandwagonHost's product structure and are easy to miss in marketing copy:

1. **Tokyo plans can't migrate.** The CN2 GIA Ultra line locks you into specific Asian datacenters — Tokyo stays Tokyo. Only the CN2 GIA-E plans allow free migration across 10+ locations. If you want to try Osaka versus Tokyo yourself, Tokyo won't let you switch after purchase; pick deliberately.
2. **Upgrades go up, never down.** You can move to a bigger plan, but a 160G can't become an 80G.
3. **Traffic is a soft cap.** Third-party guides describe overage as throttling or additional billing rather than an instant cutoff, but the exact handling lives in the current terms — check them at checkout if you expect to run close to your quota.
4. **Refunds.** Independent reviews report a 30-day money-back window for new accounts with no contract lock-in. Since this isn't spelled out on the plan page itself, treat it as likely-but-unconfirmed and verify on the order page before paying if it matters to your decision.
5. **Two Tokyo lines, zero interoperability.** A Tokyo CN2 GIA plan and The Tokyo Plan are entirely separate products with separate routing. Buying the cheap one expecting CN2 GIA later won't work.

## How to order, step by step

The process takes a few minutes and the VPS typically comes online shortly after payment:

1. Open the plan page and pick your billing cycle (annual saves ~17% versus monthly).
2. Click through to the cart.
3. Enter **BWHCGLUKKB** in the promo code field and hit Validate — confirm the discount appears before continuing.
4. Register with accurate account details; mismatched or fake information can get orders flagged as fraudulent and cancelled.
5. Pay — Alipay, UnionPay, PayPal, and credit cards are all accepted.
6. Manage the server from KiwiVM: OS reloads, snapshots, rDNS edits, console access, and an API are all included. Supported OS images cover AlmaLinux, RockyLinux, CentOS, Debian, Ubuntu, and Fedora, plus manual ISO installs on request.

Every plan includes one dedicated IPv4 address, a routed /64 IPv6 subnet, free automatic backups, free snapshots, and a 99.95% uptime guarantee.

## FAQ

**How fast is BandwagonHost's Tokyo CN2 GIA from China?** Third-party tests put it at 60–80 ms from the Shanghai/Jiangsu-Zhejiang region and roughly 80–100 ms from Guangdong, with near-zero packet loss at midday and only scattered losses during the evening peak. Guangdong users generally get lower latency from Hong Kong CN2 GIA; Yangtze Delta users often find Tokyo matches or beats it.

**Does a more expensive Tokyo plan mean faster bandwidth?** No. Every Tokyo CN2 GIA tier caps at 1.2 Gbps. Higher tiers add CPU, RAM, storage, and traffic only.

**Can I get Windows on these plans?** Not from official images — the catalog is Linux-focused, with manual ISO installation available if you bring your own licensing. Providers like LightNode offer Windows on their Tokyo VPS if that's a requirement.

**Is the annual price a first-year teaser?** No. These plans bill on a recurring cycle and renew at the purchased rate, and the recurring coupon continues to apply at renewal according to current guides.

## Picking your plan: the short version

- Audience in mainland China, small site or personal project → **Tokyo CN2 GIA 40G** at $899.99/year, coupon applied. 👉 [Order the 40G Tokyo CN2 GIA plan](https://bandwagonhost.com/aff.php?aff=74518&pid=108)
- Same routing need, more RAM or containers in play → 80G ($155.99/mo) is the natural step up; beyond that, buy from monitoring data, not optimism.
- Need Tokyo on a $100/year budget and can accept evening-peak jitter → The Tokyo Plan v2 at $99/year, if stock exists.
- Audience outside China → skip the premium entirely; budget Tokyo hosts at $4–21/month cover that job.
- Latency-tolerant but China-adjacent → BandwagonHost's own Osaka ($49.99/mo) or LA CN2 GIA-E ($169.99/yr) lines deliver most of the experience for a fraction of the price.

Before paying, two things worth thirty seconds: confirm the promo code validates in the cart, and double-check the traffic quota against what you actually served last month. Then order the smallest plan that fits — you can always upgrade, but never sideways to another datacenter.
