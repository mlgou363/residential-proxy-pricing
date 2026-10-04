# Residential proxy provider: how to compare per-IP and per-GB pricing, targeting depth, and trial terms before you commit

Search for a residential proxy provider and you get a wall of pages claiming six-figure IP pools and prices you will never actually be charged. The advertised floor is usually the top rung of a volume ladder, or a coupon that expires in three months. What you pay depends on two things almost nobody puts in the headline: how you are billed, and how much you actually consume.

So this is a buying guide, not a ranking. It walks through the decisions that change your invoice, the features that change your success rate, and where a provider like 9Proxy fits — including its full current plan list, since that is the part most comparison posts cut down to three rows.

## The billing model decides your cost before the provider does

Residential bandwidth is sold two ways, and they punish opposite workloads.

**Per-GB** is the industry default. You buy a bucket of traffic, requests rotate across the provider's pool, and every request burns bandwidth. It is cheap when each request pulls a small payload. It gets expensive fast when you are loading full pages with images, retrying blocked requests, or holding sessions that re-authenticate.

**Per-IP** flips it. You buy a number of residential IPs and run unlimited traffic through each one for as long as it stays alive. Predictable, and painful only when your job is small and bursty, because you paid for IPs you barely used.

Most vendors pick one and expect you to plan around it. 9Proxy sells both, plus bundles that mix IPs and gigabytes in one package, which is worth knowing if you run a steady multi-account workload and a bursty scraping job at the same time. You can [👉 compare the current 9Proxy packages and pricing](https://bit.ly/9-Proxy) directly rather than guessing from a blog's summary.

One caveat on numbers here: 9Proxy raised IP-based and bundle prices on 1 June 2026, the first adjustment in its history, and left GB-based pricing untouched. Older reviews still quote the pre-June rates, so expect to see $0.015/IP and $20 for 100 IPs on pages that have not been updated. The tables below use the post-adjustment figures.

## What actually separates one provider from another

Price is the easy part. These are the items that decide whether a provider survives contact with your workload.

**Targeting depth.** Country-level targeting is table stakes. City, state, ZIP, and ISP targeting is what tells you whether a geo-check reflects what a real local user sees. It also matters for account work, where two profiles on the same ISP in the same city look related.

**Session control.** You need sticky sessions for logins and checkout flows, and per-request rotation for high-volume collection. If a provider only offers one, half your use cases are broken before you start.

**IP lifetime, stated honestly.** Residential IPs belong to real devices, so they go offline when someone unplugs a router. Any provider promising fixed multi-day sessions on residential is either selling ISP proxies or being loose with definitions. A lifespan measured in hours, up to about a day, is normal.

**Invalid-IP policy.** What happens when an IP refuses connections in the first minute? A written replacement or credit policy is worth more than a slightly lower per-IP price.

**Tooling.** API access, a proxy generator, and configuration you can automate. If you are managing 200 endpoints by hand in a spreadsheet, you are paying in time instead of money.

**Protocol support.** HTTP and HTTPS cover browsers and most scraping libraries. SOCKS5 covers everything else, including anti-detect browsers and tools that do not speak HTTP proxies.

A quick gut check on any provider: ask what you pay at 5 GB and at 500 GB. If the answer is only ever "from $X/GB," the number is marketing.

## Where 9Proxy sits in that picture

9Proxy is a residential-only provider running a pool of 20M+ IPs across 90+ countries, with targeting down to country, state, city, ZIP, and ISP level. It supports HTTP, HTTPS, and SOCKS5, and reports 99.95% uptime.

The pool is smaller than the enterprise networks. Bright Data advertises 72M+ residential IPs, Oxylabs 100M+, Decodo 115M+ or more depending on which page you read. If your project needs genuine long-tail coverage in a specific small market, that gap can matter. If you are working the US, UK, Germany, Brazil, India and similar mainstream targets, it usually does not.

What 9Proxy leans on instead is a per-IP model with unlimited bandwidth per IP, unused IP balance that does not expire until activated, and a set of automation features aimed at reducing manual babysitting:

- **Today List** — any IP you forwarded in the last 24 hours can be reused at no cost if it is still online. Useful for daily recurring jobs on the same targets.
- **Auto-Refresh Proxy** — swaps IPs on a port when they drop, cutting down on connection-refused cascades in long runs.
- **Auto-Rotation Proxy** — rotates IPs on a schedule you set, per port.
- **Port configuration** — bind ports to a country, city, ZIP, or ISP, and split ports by project.
- **Proxy2Web** — web access to IP-based proxies, so you are not tied to the desktop app. The client runs on Windows and macOS.
- **API access** — programmatic endpoint creation and usage stats for pipelines.

For teams, the Enterprise GB tier adds a team mode with one owner plus up to five members, shared bandwidth with no expiry inside the team, per-member traffic limits, activity logs, and unlimited share codes.

On independent testing, a ProxyBros review published in December 2025 reported roughly 99.5% average success rate across US, DE, UK, BR, and IN routes, about 99.4% uptime on key routes measured over a week, and 0.6-second average response time on heavier pages. Those are one reviewer's numbers on one workload, not a guarantee, and residential success rates move with the target site. Reviewers also flag limits: iTWire noted that major streaming platforms frequently block 9Proxy IPs, and that the IP-based flow leans on the desktop app. If streaming unblocking is your use case, this is the wrong tool.

## Every current 9Proxy plan

Prices below are the post-June-2026 structure. IP-based and bundle pricing reflects the adjustment; GB-based pricing is unchanged.

### Residential proxy by IPs — unlimited bandwidth per IP

| Package | Price per IP | Total | Notes | Buy |
| --- | --- | --- | --- | --- |
| 100 IPs | $0.24 | $24 | Small projects, proof of concept | [ start with 100 IPs](https://bit.ly/9-Proxy) |
| 500 IPs | $0.144 | $72 | Solo operators, light scraping | [ get 500 IPs](https://bit.ly/9-Proxy) |
| 1,000 IPs + 500 bonus | $0.084 | $126 | Bonus IPs included | [ 1,000 IPs plus 500 bonus](https://bit.ly/9-Proxy) |
| 2,500 IPs | $0.084 | $210 | Several verticals running at once | [ compare 2,500 IPs](https://bit.ly/9-Proxy) |
| 5,000 IPs | $0.072 | $360 | Agencies and mid-scale SEO stacks | [ 5,000 IP packages](https://bit.ly/9-Proxy) |
| 15,000 IPs | $0.048 | $720 | Regional teams | [ 15,000 IP tier](https://bit.ly/9-Proxy) |
| 25,000 IPs | $0.035 | $863 | Heavy automation | [ 25,000 IP tier](https://bit.ly/9-Proxy) |
| 50,000 IPs | $0.029 | $1,438 | High-volume operations | [ 50,000 IP tier](https://bit.ly/9-Proxy) |
| 100,000 IPs | $0.023 | $2,300 | Business tier | [ 100,000 IP business tier](https://bit.ly/9-Proxy) |
| 200,000 IPs | $0.021 | $4,140 | Business tier | [ 200,000 IP business tier](https://bit.ly/9-Proxy) |
| 500,000 IPs | $0.018 | $8,625 | Business tier, lowest per-IP rate | [ 500,000 IP business tier](https://bit.ly/9-Proxy) |

Billing is prepaid balance, not a subscription. Unused IPs stay in your account until you activate them, and each IP runs until it naturally drops.

### Residential proxy by GB

| Package | Price per GB | Total | Validity | Buy |
| --- | --- | --- | --- | --- |
| 5 GB | $3.00 | $15 | 180 days | [ 5 GB starter pack](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | $2.10 | $105 | 180 days | [ 50 GB pack](https://bit.ly/9-Proxy) |
| 100 GB | $1.50 | $150 | 180 days | [ 100 GB pack](https://bit.ly/9-Proxy) |
| 200 GB | $1.00 | $200 | 180 days | [ 200 GB pack](https://bit.ly/9-Proxy) |
| 1,000 GB | $0.80 | $800 | 180 days | [ 1,000 GB pack](https://bit.ly/9-Proxy) |
| 2,000 GB | $0.75 | $1,500 | 180 days | [ 2,000 GB pack](https://bit.ly/9-Proxy) |
| 3,000 GB (Enterprise) | $0.72 | $2,160 | No expiry | [ Enterprise 3,000 GB](https://bit.ly/9-Proxy) |
| 6,000 GB (Enterprise) | $0.70 | $4,200 | No expiry | [ Enterprise 6,000 GB](https://bit.ly/9-Proxy) |
| 10,000 GB (Enterprise) | $0.68 | $6,800 | No expiry | [ Enterprise 10,000 GB](https://bit.ly/9-Proxy) |

On GB plans you generate unlimited endpoints and only the traffic is metered. The 180-day clock is the thing to watch for project-based work; it is generous compared to monthly commitments that reset, but it is not unlimited. Enterprise removes the deadline entirely and unlocks the team features.

### Bundle packages — IPs plus traffic

| Bundle | Contents | Price | Traffic validity | Buy |
| --- | --- | --- | --- | --- |
| Starter | 100 IPs + 5 GB | $30 | 180 days | [ Starter bundle](https://bit.ly/9-Proxy) |
| Popular | 1,500 IPs + 50 GB | $180 | 180 days | [ Popular bundle](https://bit.ly/9-Proxy) |
| Pro | 5,000 IPs + 500 GB | $720 | 180 days | [ Pro bundle](https://bit.ly/9-Proxy) |

The bundles are the cheapest way in if you are not sure which model you need. Note that both halves are discounted relative to buying them separately, which is the point.

Also worth checking before you pay: some payment methods carry an extra 5% discount or a 5% product bonus, so the effective price depends on how you check out. Free trials show up periodically but are limited and usually require asking support for a code — they are not a permanent self-serve option.

## Which model should you actually buy

Skip the tier table and think about your workload shape.

If your jobs are **long and steady** — logged-in sessions, account management, continuous collection where you would otherwise watch a bandwidth counter with dread — buy IPs. 100 IPs at $24 is the cheapest honest way to test the model, and unused IPs do not evaporate, so scaling up later costs you nothing extra.

If your jobs are **bursty or rotation-heavy** — ad verification, geo-checks, lightweight scraping where each request is small but you want a fresh IP constantly, API polling — buy GB. A 5 GB pack at $15 tells you more about IP quality in an afternoon than any review.

If you genuinely run **both kinds of work**, the Pro bundle at $720 beats sourcing the same volumes separately, but it is a real commitment. Most teams should spend a month on a small package first and let the usage data pick their model. There is no prize for guessing right on day one.

One number to sanity check against the rest of the market: at the low end, 9Proxy's $3.00/GB on a 5 GB pack is competitive with pay-as-you-go rates from established names, and its per-IP pricing at volume ($0.018 at 500,000 IPs) is low by industry standards. But per-GB rates from larger networks drop below $1/GB at high volume, so if you are a pure bandwidth buyer pushing terabytes, the smaller pool is not automatically the cheaper choice.

## Practical notes before you commit

A short list of things that trip people up, in no particular order.

Residential IPs die. Plan for it with auto-refresh rather than reacting to it. IP-based plans require the desktop app for most workflows, though Proxy2Web covers browser-based retrieval. GB plans run entirely from the dashboard with username/password or IP whitelisting, which is easier on cloud servers. Pair the service with an anti-detect browser for multi-account work; 9Proxy's own partner material points at Multilogin, AdsPower, and Dolphin Anty, and user reviews specifically mention those tools working with it.

Support is 24/7 with human agents, and third-party reviewers have generally reported quick, technically substantive replies. That is a claim from people who tested it, not a promise you can hold them to.

## FAQ

**How much does a residential proxy provider cost?**
Anywhere from under $1/GB to $12/GB depending on volume and provider tier. Per-IP pricing commonly lands between $0.02 and $0.30 per IP. 9Proxy's entry point is $15 for 5 GB or $24 for 100 IPs with unlimited bandwidth on each.

**Is per-IP or per-GB better for web scraping?**
It depends on payload size. Heavy pages and full browser rendering burn bandwidth quickly, which favours per-IP with unlimited traffic. Small API responses with frequent rotation favour per-GB, where you only pay for what you consume.

**How long do residential IPs last?**
Hours to roughly 24 hours on 9Proxy's IP-based plans, depending on the real device behind the IP. GB-based traffic uses rotating IPs with no fixed lifetime.

**Do unused proxies expire?**
On 9Proxy, unused IP balance stays until activated. GB packages carry 180-day validity, except Enterprise tiers, which have no expiry.

**Can I test before buying?**
Yes, in a limited way. Small packages are the practical route, and promotional free trials appear from time to time but need a request to support. There is also a 60-second policy that replaces or credits IPs that fail to connect immediately.

The honest summary: 9Proxy is a reasonable pick when your workload is data-heavy and you would rather pay for IP access than count gigabytes, and a poor pick if you need the largest possible pool or streaming unblocking. Check what you would pay at your actual volume before you commit either way — [👉 see the live 9Proxy plans and pick a package](https://bit.ly/9-Proxy) is the only number that matters in the end.
