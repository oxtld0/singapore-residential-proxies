# singapore residential proxy: choosing real SG IPs for Shopee, Lazada and Google.sg, and when per-IP billing beats per-GB

You want Google to think you're in Singapore. A datacenter IP in Frankfurt gets you USD prices, a redirect, or a captcha wall, depending on the site. That's the whole problem in one sentence, and it's why people search for a Singapore residential proxy rather than "cheap proxy".

The trap is buying on headline price. A provider advertising 100M+ residential IPs across 195 countries can still have a thin Singapore pool, because Singapore is small — under six million people, four mobile operators, and a residential pool that is a rounding error next to the US or Brazil. If your target is Shopee, Lazada, Amazon.sg or Qoo10, the only number that matters is how many live SG IPs you can actually get at 10am Singapore time, and what you pay for them.

This is a working guide to that decision, with 9Proxy's current plans and prices laid out in full so you can compare the two billing models against your own workload.

## What a Singapore IP actually changes

Almost all the data worth collecting in Singapore is local and IP-gated. Shopee, Lazada, Amazon.sg and Qoo10 serve prices, stock levels, promotions and ad placements based on where the visitor appears to be, in Singapore dollars and in English. A price in SGD and a local delivery estimate only appear for an IP that looks Singaporean. Pull the same page from a Malaysian or American IP and you get wrong prices, a redirect, or nothing at all.

The same logic applies further out:

- Ad verification for campaigns bought on local publishers
- SERP and rank tracking on Google's Singapore results, which differ from the .com set you see abroad
- Travel and fintech pricing on Agoda-style aggregators that quote different fares per market
- Multi-account work on regional marketplaces and social platforms, where an IP that jumps between countries is the fastest way to get a seller account reviewed
- Content testing for services licensed per market in Southeast Asia

Singapore's own privacy law matters here too. The PDPA, enforced by the PDPC, governs personal data. Scraping public product and price data is defensible; personal data is the real risk regardless of which proxy you route through.

Anti-bot systems treat datacenter ranges as a signal and residential and mobile addresses from Singtel, StarHub, M1 and Simba as ordinary local shoppers. That's the technical reason a residential SG IP is not an optimisation but the entry condition for correct data.

## The five things worth checking before you pay

**Pool depth in Singapore specifically.** Ask for the SG IP count, not the global total. A provider with 90M IPs worldwide can still hand you the same few hundred Singapore addresses.

**Rotating versus sticky, and how long sticky lasts.** SERP sampling wants a fresh IP per request. Seller accounts, ad dashboards and cart sessions want the same IP held for 10 to 30 minutes. Confirm the session control is configurable to the minute, not just "sticky available".

**Targeting granularity inside the country.** Singapore is a city-state, so city targeting is effectively country targeting. What actually helps is postal-code and ISP filtering — useful when you need traffic that looks like it comes from a specific residential network rather than a flagged range.

**Protocol support.** HTTP/HTTPS and SOCKS5 both, because anti-detect browsers and automation stacks differ on which they want.

**Billing shape.** Per-gigabyte pricing punishes JavaScript-heavy pages; a product page that weighs 2 to 5 MB means your costs scale with page size you don't control. Per-IP pricing with unlimited bandwidth flattens that, but only pays off if you actually push volume through each IP.

## Where 9Proxy fits

9Proxy is a residential proxy provider that has been running for about three years, with a network it advertises as 20M+ residential IPs across 90+ countries. Singapore is on the country list, and country, state, city, ZIP code and ISP targeting are all supported. HTTP/HTTPS and SOCKS5 are both available.

It sells two residential models, and the difference explains most of the pricing:

**Residential by IPs.** You buy a block of IPs and pay per IP, not per gigabyte. Bandwidth is unlimited while an IP is active. Unused IPs never sit around expiring — they stay in your balance until you forward them. Each activated IP lives a few hours up to roughly 24 hours, which is normal for a residential network. You use this through the desktop app on Windows, macOS or Linux, forwarding an IP to a local port, with optional username-password authentication on top.

**Residential by GB.** You buy traffic and generate unlimited endpoints from the dashboard, no app needed. Rotating or sticky sessions, authenticated by username-password or by IP whitelisting. Purchased traffic is valid for 180 days, unlimited for Enterprise accounts. Targeting is embedded in the username string, so a Singapore session looks like:


country-sg
country-sg-city-singapore
country-sg-sst-20-ssid-device1


The `sst` value is the sticky session length in minutes; `ssid` lets you run several sticky IPs from the same configuration. Their own documentation warns against over-filtering — stacking state, city and ISP narrows the available pool, and in a small market like Singapore that warning bites faster than it does for the US.

One practical note for teams: on IP-based plans, one forwarded IP counts as one IP used, so you can't spin up unlimited concurrent sessions the way the GB plans allow. If your Singapore workflow is 40 parallel browser profiles, that's 40 IPs, and the arithmetic is straightforward.

## 9Proxy full plan list and prices

Prices are in USD as published, and reflect the pricing update that took effect on 1 June 2026 for IP-based and bundle packages. GB-based pricing was left unchanged in that update.

| Package | What you get | Price | Validity / notes | Purchase |
| --- | --- | --- | --- | --- |
| 100 IPs | 100 residential IPs, unlimited bandwidth | $24 | Unused IPs never expire | [Get the 100 IP package](https://bit.ly/9-Proxy) |
| 500 IPs | 500 residential IPs, unlimited bandwidth | $72 | Unused IPs never expire | [Get the 500 IP package](https://bit.ly/9-Proxy) |
| 1,000 IPs (+500 bonus) | 1,500 IPs total, unlimited bandwidth | $126 | Bonus IPs included | [Get the 1,000 + 500 IP package](https://bit.ly/9-Proxy) |
| 2,500 IPs | 2,500 residential IPs, unlimited bandwidth | $210 | Unused IPs never expire | [Get the 2,500 IP package](https://bit.ly/9-Proxy) |
| 5,000 IPs | 5,000 residential IPs, unlimited bandwidth | $360 | Unused IPs never expire | [Get the 5,000 IP package](https://bit.ly/9-Proxy) |
| 15,000 IPs | 15,000 residential IPs, unlimited bandwidth | $720 | Unused IPs never expire | [Get the 15,000 IP package](https://bit.ly/9-Proxy) |
| 25,000 IPs | 25,000 residential IPs, unlimited bandwidth | $863 | Unused IPs never expire | [Get the 25,000 IP package](https://bit.ly/9-Proxy) |
| 50,000 IPs | 50,000 residential IPs, unlimited bandwidth | $1,438 | Unused IPs never expire | [Get the 50,000 IP package](https://bit.ly/9-Proxy) |
| Business 100,000 IPs | High-volume IP block, unlimited bandwidth | $2,300 | Business tier | [Get the 100,000 IP business package](https://bit.ly/9-Proxy) |
| Business 200,000 IPs | High-volume IP block, unlimited bandwidth | $4,140 | Business tier | [Get the 200,000 IP business package](https://bit.ly/9-Proxy) |
| Business 500,000 IPs | High-volume IP block, unlimited bandwidth | $8,625 | Business tier | [Get the 500,000 IP business package](https://bit.ly/9-Proxy) |
| 5 GB | Traffic pack, unlimited endpoints | $15 | 180 days | [Get the 5 GB pack](https://bit.ly/9-Proxy) |
| 50 GB (+5 GB bonus) | Traffic pack, unlimited endpoints | $105 | 180 days, $2.10 per GB | [Get the 50 + 5 GB pack](https://bit.ly/9-Proxy) |
| 100 GB | Traffic pack, unlimited endpoints | $150 | 180 days, $1.50 per GB | [Get the 100 GB pack](https://bit.ly/9-Proxy) |
| 200 GB | Traffic pack, unlimited endpoints | $200 | 180 days, $1.00 per GB | [Get the 200 GB pack](https://bit.ly/9-Proxy) |
| 1,000 GB | Traffic pack, unlimited endpoints | $800 | 180 days, $0.80 per GB | [Get the 1,000 GB pack](https://bit.ly/9-Proxy) |
| 2,000 GB | Traffic pack, unlimited endpoints | $1,500 | 180 days, $0.75 per GB | [Get the 2,000 GB pack](https://bit.ly/9-Proxy) |
| 10,000 GB | Traffic pack, unlimited endpoints | $0.68 per GB at this tier | 180 days | [Get the 10,000 GB pack](https://bit.ly/9-Proxy) |
| Starter Bundle | 100 IPs + 5 GB | $30 | Bundled traffic valid 180 days | [Get the Starter Bundle](https://bit.ly/9-Proxy) |
| Popular Bundle | 1,500 IPs + 50 GB | $180 | Bundled traffic valid 180 days | [Get the Popular Bundle](https://bit.ly/9-Proxy) |
| Pro Bundle | 5,000 IPs + 500 GB | $720 | Bundled traffic valid 180 days | [Get the Pro Bundle](https://bit.ly/9-Proxy) |
| Enterprise | Unlimited traffic validity, team mode (1 owner + up to 5 members), per-member traffic controls, activity logs, VIP pricing, dedicated support | Quote on request | No expiration on shared traffic inside the team | [Open an account to request Enterprise pricing](https://bit.ly/9-Proxy) |

Two things stand out in that list. The entry point is $24, which is low enough that testing Singapore coverage before committing to a big plan costs less than lunch in Singapore. And the bonus structures — 1,000 + 500 IPs, 50 + 5 GB — are baked into the package itself rather than requiring a coupon code you have to hunt for.

If you're coming from an affiliate or referral link, note that 9Proxy's own affiliate FAQ states referred users get a 5% discount, which is applied through the invite code at sign-up. That's the reliable discount path; promo code aggregator pages for this brand are inconsistent, and several list codes that don't clearly correspond to a current offer.

## Per-IP or per-GB for a Singapore workflow?

This is the decision most people get wrong, and it comes down to what your job spends.

**Per-GB fits rotation-heavy, low-payload work.** SERP sampling across a few hundred Singapore queries, geo-checking, light monitoring, API polling. Each request carries maybe 40 to 80 KB, so a 50 + 5 GB pack at $105 covers a serious amount of sampling, and the 180-day window means an uneven project schedule doesn't burn your balance in a month. The dashboard-only setup also matters if you're running this from a cloud container where you can't install a desktop app.

**Per-IP fits sessions and heavy pages.** Seller account management, ad account work, cart and checkout flows, full catalogue scraping where images and scripts push each page into the megabytes. Unlimited bandwidth on an active IP means page weight stops being a cost variable. The 100-IP package at $24 works out to $0.24 per IP of balance — nothing, for a proof of concept.

The awkward middle is a project that needs both: a handful of long-lived sticky sessions plus a burst of high-volume rotation. That's what the bundles exist for, and the Popular Bundle at $180 for 1,500 IPs and 50 GB is the one most mixed workloads land on.

## Setting up Singapore targeting

1. Create an account through the invite link so any referral discount is attached to it.
2. Buy the package that matches your billing shape — IP-based if you need long sessions and heavy pages, GB-based if you're rotating a lot with small payloads.
3. **For GB plans:** open the dashboard, go to the proxy generator, pick Singapore as the country (and city, ZIP or ISP only if you need it), choose sticky or rotating, and export the endpoint list. No app is required.
4. **For IP-based plans:** install the desktop app, filter the proxy list to Singapore, then forward an IP to a local port and point your tool at `localhost:port`.
5. Verify before you trust it. Run a request through the endpoint against an IP-lookup service and confirm the country reads Singapore. Doing this once per new sticky session is cheaper than debugging why Shopee returned Malaysian prices.
6. If you're running IP-based plans in a workflow that breaks when an IP drops, turn on auto-refresh so offline IPs get replaced instead of stalling the job.

One account detail worth knowing: sub-users can log into the dashboard directly, and accounts can be shared via share codes or sub-accounts with per-member traffic controls. If you're handing Singapore work to a contractor, that's the cleaner route than passing around your main login.

## Limits and quirks, stated plainly

- On IP-based plans, an activated IP lives somewhere between a few hours and around 24 hours. That's the nature of a residential pool, not a bug, but it means you can't build a workflow that assumes one IP stays up all week.
- IP-based usage requires the desktop app for port forwarding. If your environment is a Linux container with no GUI, the GB model is the practical choice.
- GB traffic expires after 180 days unless you're on Enterprise. Plan purchases around project timelines rather than buying a year of traffic up front.
- Over-filtering hurts in small markets. Asking for one Singapore ZIP code plus one specific ISP shrinks your candidate pool a lot; start with country-level targeting and narrow only if you have a reason.
- The IP pool is advertised rather than independently audited, and no provider's advertised country count tells you how many of those IPs are live in Singapore at any given moment. Test it with your own targets.

## What third-party sources say

Geekflare's 2026 review treats 9Proxy as a budget option whose per-IP unlimited-bandwidth model suits sustained sessions and long scraping jobs, and notes the trade-off is that per-IP pricing is clumsy for projects that just need a little traffic. That matches the split described above.

ProxyLook's comparison pages list 9Proxy at a 97% success rate with roughly 1,300 ms average response time, against a 20M+ advertised residential pool — slower than the premium tier of the market, which is a fair description of what you're buying at this price point. A review on AlternativeTo describes the residential IPs as stable and notes they work with tools like Dolphin Anty and AdsPower, which is the multi-account use case in practice.

The brand also claims 99.95% uptime, and partner documentation mentions an instant credit for any IP that fails to connect within its first minute of use. Treat vendor figures as vendor figures and benchmark figures as starting points; the only number that matters is your success rate against your own target list.

## FAQ

**Does 9Proxy have Singapore residential IPs?**
Singapore is on the supported country list, and country-level targeting with city, ZIP and ISP filtering is available across the network. As with any provider, confirm live availability for your target sites before committing to a large package.

**What's the cheapest way to test Singapore IPs?**
The 100-IP package at $24, or the 5 GB pack at $15 if your test is request-volume based. Both are single purchases — there's no subscription to cancel. 9Proxy's vendor FAQ also mentions a limited free trial for new users, subject to availability.

**Can I hold the same Singapore IP for a long session?**
Yes, on GB plans via the `sst` parameter in the username, which sets session length in minutes; add `ssid` to run several sticky sessions from one configuration. On IP plans, persistence depends on the individual IP staying online.

**Do I need to install anything?**
Only for IP-based plans, which route through the desktop app on Windows, macOS or Linux. GB-based plans run entirely from the dashboard.

**Which payment methods are accepted?**
The vendor FAQ lists credit and bank cards, cryptocurrencies including USDT and BTC, Alipay, Apple Pay and Google Pay.

## Bottom line

If your target is Shopee, Lazada, Amazon.sg or Google's Singapore results, a residential SG IP is the only way to see correct prices in SGD, and pool depth in Singapore matters far more than a provider's global IP count. 9Proxy's two models map cleanly onto the two common Singapore workloads: buy per GB when you're rotating through sampling tasks with small payloads, and buy per IP when you're holding sessions and pushing heavy pages where per-gigabyte billing would punish you.

Start with the smallest package that covers your test, check your success rate against your real targets, and scale once the numbers hold up. 👉 [You can open a 9Proxy account and pick your Singapore package here](https://bit.ly/9-Proxy).
