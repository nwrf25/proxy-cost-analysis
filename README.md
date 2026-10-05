# buy proxy: what a gigabyte really costs, which proxy type you need, and how to start with $5

Search "buy proxy" and you get a wall of identical landing pages, all claiming the biggest pool and the fastest speeds. Almost none of them tell you the two numbers that actually decide your bill: how much each successful request costs, and whether the traffic you paid for survives the month.

So the useful way to approach this is not "which provider ranks first" but "what am I paying per usable gigabyte, and does the plan match the job". DataImpulse is a decent case study for that question, because its whole pitch is the boring part of proxy buying: a flat per-GB rate, no subscription, and traffic that doesn't expire. Whether that's the right buy for you depends on what you're scraping.

## First, decide what kind of proxy you're actually buying

"Proxy" is four different products with four very different price points, and picking the wrong tier is the most common way people waste money. Paying residential rates for a target that datacenter IPs would walk straight into is pure overspend. The reverse error costs you blocked requests and retry overhead.

| Proxy type | What the IP actually is | Typical price band on the market | Best fit |
| --- | --- | --- | --- |
| Datacenter | Server-network IPs, fast, cheap | ~$0.50–3/GB, or per-IP monthly fees | Bulk crawls of unprotected sites, price checks, uptime monitoring |
| Residential | ISP-assigned IPs from real devices | ~$3–8/GB at mainstream providers | E-commerce, SERPs, anything behind Cloudflare-grade protection |
| Mobile | 4G/5G carrier IPs | ~$5–15/GB, or per-port pricing | Mobile-first apps, social platforms, the hardest anti-bot stacks |
| Premium residential | Higher-grade residential sub-pool | Above standard residential rates | Enterprise workloads where latency and block rates have budget consequences |

On DataImpulse the same four tiers are priced at **$1/GB residential**, **$0.50/GB datacenter**, **$2/GB mobile** and **$5/GB premium residential**, all pay-as-you-go. That puts its residential and mobile lines at the bottom of the published market range rather than the middle of it.

If you want to sanity-check those against what the dashboard shows on the day, 👉 [👉 Check current DataImpulse per-GB pricing](https://bit.ly/dataimPulse)

## The billing model matters more than the sticker price

Here's the trap. A provider advertising $2.50/GB with a monthly plan and 30-day traffic expiry can easily cost more per usable gigabyte than one charging $3/GB pay-as-you-go, if your crawl calendar is lumpy. Data teams rarely burn bandwidth at a constant rate. You spike during a project, then go quiet for three weeks while you clean data.

Subscription traffic dies on a timer regardless of whether you used it. Prepaid balances that don't expire keep working whenever you come back.

DataImpulse sits firmly in the second camp: no subscription, no monthly minimum, and purchased GB staying in your account until consumed. The minimum top-up is **$5**, which is the entire commitment to test whether the network works on your specific targets.

That last point is worth spelling out, because it changes how you should evaluate providers. A $5 floor means you can measure your own success rate and cost per successful request on the sites you actually care about, rather than trusting someone else's benchmark page. Ten dollars of testing beats a month of guessing.

One caveat on the free-trial question: there isn't one. Nothing runs without a payment. Intro purchases do carry a 7-day money-back guarantee, but it applies to card payments and crypto buys are excluded, so read the terms on the checkout page before assuming you can unwind a purchase.

## Every DataImpulse plan, side by side

Here's the full plan grid as published on the official product pages. Intro is the new-user entry pack. Basic is the standard top-up. Advanced is where the volume discount starts. Custom is the enterprise lane handled through sales.

| Proxy type | Plan | Traffic | Price | Per GB | Billing | Purchase |
| --- | --- | --- | --- | --- | --- | --- |
| Residential | Intro | 5 GB | $5 | $1.00 | PAYG, non-expiring | [ Start with the $5 residential intro pack](https://bit.ly/dataimPulse) |
| Residential | Basic | 50 GB | $50 | $1.00 | PAYG, non-expiring | [ Top up 50 GB of residential traffic](https://bit.ly/dataimPulse) |
| Residential | Advanced | 1 TB | $800 | $0.80 | PAYG, 20% volume discount | [ Buy the 1 TB residential tier at $0.80/GB](https://bit.ly/dataimPulse) |
| Residential | Custom+ | 5 TB+ | Quoted | Negotiated | Enterprise, dedicated account manager | [ Request residential volume pricing](https://bit.ly/dataimPulse) |
| Datacenter | Intro | 10 GB | $5 | $0.50 | PAYG, non-expiring | [ Get 10 GB of datacenter traffic for $5](https://dataimpulse.com/datacenter-proxies/?aff=86938) |
| Datacenter | Basic | 100 GB | $50 | $0.50 | PAYG, non-expiring | [ Take the $0.50/GB datacenter plan](https://dataimpulse.com/datacenter-proxies/?aff=86938) |
| Datacenter | Advanced | 1 TB | $450 | $0.45 | PAYG, 10% volume discount | [ Buy 1 TB of datacenter traffic at $0.45/GB](https://dataimpulse.com/datacenter-proxies/?aff=86938) |
| Datacenter | Custom | 5 TB+ | From $2,250 | ~$0.45 | Enterprise | [ Ask about datacenter volume pricing](https://dataimpulse.com/datacenter-proxies/?aff=86938) |
| Mobile | Intro | 2.5 GB | $5 | $2.00 | PAYG, non-expiring | [ Buy 2.5 GB of 4G/5G mobile traffic](https://bit.ly/dataimPulse) |
| Mobile | Basic | 25 GB | $50 | $2.00 | PAYG, non-expiring | [ Top up 25 GB of mobile proxies](https://bit.ly/dataimPulse) |
| Mobile | Advanced | 1 TB | $1,600 | $1.60 | PAYG, 20% volume discount | [ Take the 1 TB mobile tier at $1.60/GB](https://bit.ly/dataimPulse) |
| Mobile | Custom+ | 5 TB+ | Quoted | Negotiated | Enterprise | [ Request mobile proxy volume pricing](https://bit.ly/dataimPulse) |
| Premium residential | Intro | 1 GB | $5 | $5.00 | PAYG, non-expiring | [ Test the premium residential pool for $5](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |
| Premium residential | Basic | 10 GB | $50 | $5.00 | PAYG, non-expiring | [ Buy 10 GB of premium residential proxies](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |
| Premium residential | Custom | 1,000 GB+ | $4,000 | $4.00 | PAYG, enterprise terms | [ Look at premium residential volume terms](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |

Two footnotes. The Custom+ and Custom "from" figures are the figures third-party reviews report for the enterprise lane; those tiers are quoted individually, so treat them as a floor rather than a price. And the discount tiers are volume-gated on purpose: on residential and mobile the 20% break starts at 1 TB, which means small and mid-size buyers pay the flat rate no matter how often they top up.

## Running the math on a realistic workload

Numbers land better with a scenario. Suppose a price-monitoring setup that pulls 200 GB a month.

- At the flat residential rate, that's **$200/month**, with no contract and no expiry clock.

- Bought as a 1 TB pack, the effective rate drops to $0.80/GB, so the same 200 GB costs **$160/month equivalent** — but you've paid $800 up front, and those gigabytes sit in the balance until used.

- Split the workload properly and it gets cheaper still. Public listings, news archives and unguarded catalogues don't need residential IPs. Routing the trivially accessible half of a crawl through **$0.50/GB datacenter** traffic instead cuts the bill roughly in half for the same volume.

That routing discipline is the single biggest lever on proxy spend, and it has nothing to do with which provider you pick. Buy the tier the target actually requires, not the tier that sounds safest.

There's one billing detail to watch here. On standard residential, country-level targeting is included in the base rate, but DataImpulse's own pricing guide describes state, city and ZIP and ASN filtering as a paid add-on rather than a free extra, and at least one independent write-up puts that surcharge at twice the standard per-GB rate. On premium residential, full targeting is listed as included. Third-party listings disagree on this point, so if your workflow depends on city or ZIP-level precision, confirm the current treatment with support before you build a budget around it.

## What independent testing actually shows

DataImpulse's published network stats are 90M+ ethically sourced IPs across 195 countries, with a first-party pool built through its own bandwidth-sharing app rather than resold from another vendor's network. It's a 2022-launch product out of the Softoria group, so younger than the decade-old names.

The more useful data points come from outside testing. Proxyway's April 2025 benchmark recorded a **99.51% overall success rate** and an average global response time of **1.22 seconds**, with Amazon at **93.66%** and Instagram at **65.30%**. That spread is the honest picture of any general-purpose residential network: fine on retail and search, visibly weaker on hard social targets. Proxyway also named the company Newcomer of the Year in 2024 and flagged it for greatest progress the following year.

One thing worth keeping in perspective: that same benchmark counted roughly 700,000 unique residential IPs in the network at the time, well below the 90M+ headline. Every provider in this market markets its pool at its theoretical maximum, so compare pools with a healthy amount of skepticism rather than treating any of these numbers as a like-for-like spec.

On the review side, G2 currently shows 28 reviews averaging about **4.7 out of 5**, and the company publicly claims 500,000+ customers. Trustpilot sentiment in provider roundups is broadly positive, particularly about response times. Those are vendor-sourced or platform-hosted numbers, so weigh them accordingly.

## Where DataImpulse is the wrong buy

A $1/GB rate has to come from somewhere, and the trade-offs are visible if you look.

- **No managed scraping API.** This is a developer-first, bring-your-own-code service. You handle requests, parsing, retries and CAPTCHA logic yourself. If you want a turnkey scraper, you're shopping for a different product.

- **No free trial.** The $5 floor is low, but it's still a payment.

- **Thin coverage in harder geographies.** Multiple reviewers note the network is shallower in parts of Sub-Saharan Africa and Central Asia than Bright Data or Oxylabs. US, UK, DE, JP and BR pull their weight; long-tail countries may disappoint.

- **Sticky session caps.** Residential sticky sessions are configurable up to 120 minutes with a 30-minute default, and the datacenter product caps sticky sessions around 30 minutes. Providers offering 24-hour session persistence exist if long-lived logins are core to your workflow.

- **No published SOC 2 or ISO 27001 certification.** If your procurement process is gated on compliance paperwork, that's a blocker regardless of price.

- **Softer hard-target performance.** The Instagram figure above says it plainly. For aggressive social platforms, a specialist may be worth the premium.

## How to buy and get running

The setup is short, which is itself a signal about what this service is.

1. **Create an account** and choose a plan type — residential, datacenter, mobile or premium residential.

2. **Top up the traffic volume** you want. $5 gets you 5 GB residential, 10 GB datacenter, 2.5 GB mobile or 1 GB premium. Nothing activates until you add funds.

3. **Configure in the dashboard.** Pick target country, rotation mode, session length, and authentication by username/password or IP whitelist. Sub-user accounts with their own quotas are available if you're splitting budget across a team.

4. **Point your code at the gateway.** HTTP/HTTPS on port 823, SOCKS5 on port 824. Sticky sessions run on the 10000–20000 port range.

5. **Test against real targets before scaling.** This is what the $5 pack is for. Measure your success rate on the sites you actually need, then decide whether 200 GB is a $200 line item or a mistake.

6. **Scale into the volume tier only when the usage is proven.** Buying 1 TB to chase a 20% discount, then burning 60 GB in a quarter, is a worse deal than paying the flat rate.

Integrations and code snippets cover Python, Node.js, PHP, C#, Go, Ruby and cURL, with guides for Scrapy, Selenium, Playwright, Puppeteer and the main anti-detect browsers. Documentation is decent enough that you likely won't need support to get a first request through.

## A six-point checklist before you pay any proxy vendor

1. Is the price per GB, or per IP per month? The two are not comparable without doing the math on your volume.

2. Does purchased traffic expire? If yes, what's the realistic waste rate for your team's schedule?

3. Is there a monthly minimum, and is a subscription required to get a sane per-GB rate?

4. Is geo-targeting included, or is city and ZIP precision a surcharge? This can quietly double a bill.

5. What's the entry price for a real test? Anything above roughly $10 makes honest evaluation expensive.

6. Does the provider's pool come from its own network or resold from aggregators? First-party pools tend to have less accumulated abuse history against the same IPs.

## Short answers to the usual questions

### Is $1 per GB real, or a promotional rate that disappears?

It's the published residential rate on the official site, not a limited-time discount, and country targeting is included. The volume discount at 1 TB is a separate, permanent tier structure.

### Do I need a subscription?

No. There's no subscription and no monthly minimum. The trade-off is that nothing is free either — the $5 intro pack is the smallest possible entry.

### What's the cheapest legitimate way to start?

Buy the smallest intro pack in the type that matches your target, run your own workload for a few days, and compute cost per successful request. On protected targets that means residential at $1/GB; on open sites, datacenter at $0.50/GB will usually do the job for half the money.

### Can I use one balance across proxy types?

Yes. Residential, datacenter, mobile and premium residential are all managed from a single account and dashboard.

---

The short version of buying a proxy in 2026: ignore the headline pool size, check whether your traffic expires, and buy the cheapest tier your targets will tolerate. Then test it on your own sites before committing real budget.

If you want to run that test on a first-party residential pool without signing up for anything recurring, the entry point is small enough to be worth an afternoon.

👉 [👉 Start with $5 and test DataImpulse on your own targets](https://bit.ly/dataimPulse)
