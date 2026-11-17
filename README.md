# RackNerd Amsterdam: What $21.99/Year Buys You, Can You Actually Pick Amsterdam at Checkout, and Does Renewal Cost More? (Plans, Test IP, Refund Rules)

RackNerd's cheapest Amsterdam VPS is **$21.99/year** for 1 GB RAM, 20 GB SSD and 3 TB of monthly transfer, deployed in Equinix AM5 on a 1 Gbps port. A separate Amsterdam-only store page has also listed a 2 GB plan at **$22.38/year**. Treat that second figure as something to confirm in the cart rather than a published fact: it appears in several third-party walkthroughs, but no public RackNerd page can be re-checked for it right now.

Two other things decide whether this is a good buy: whether Amsterdam appears in the location dropdown for the plan you pick, and the fact that the annual price is not refundable. Both are covered below, along with three-year cost, the facility itself, and which tier fits a VPN versus a Docker stack.

> **Quick pick:** For a European exit node running a VPN, a small site or a couple of containers, take the **1 GB plan at $21.99/year**. If the Amsterdam store page shows the 2 GB plan at $22.38 at checkout, buy that instead, since it doubles the RAM for about 39 cents more. 👉 [Check current RackNerd Amsterdam VPS pricing](https://my.racknerd.com/aff.php?aff=11397&rp=/store/amsterdam-kvm-vps-specials)

## The full plan lineup, and which tiers reach Amsterdam

These are the annual KVM specials RackNerd sells across its locations. All of them include full root access, one dedicated IPv4, a 1 Gbps port and a KVM panel.

| Plan | vCPU / RAM / SSD | Monthly transfer | Annual price | Order |
| --- | --- | --- | --- | --- |
| 1 GB KVM Special | 1 / 1 GB / 20 GB | 3 TB | $21.99/yr | [Order the 1 GB plan](https://my.racknerd.com/aff.php?aff=11397&rp=/store/special-promos) |
| 2 GB KVM Special | 2 / 2 GB / 35 GB | 5 TB | $35.99/yr | [Order the 2 GB plan](https://my.racknerd.com/aff.php?aff=11397&rp=/store/special-promos) |
| 4 GB KVM Special | 3 / 4 GB / 60 GB | 7 TB | $59.99/yr | [Order the 4 GB plan](https://my.racknerd.com/aff.php?aff=11397&rp=/store/special-promos) |
| 6 GB KVM Special | 6 / 6 GB / 100 GB | 12 TB | $89.99/yr | [Order the 6 GB plan](https://my.racknerd.com/aff.php?aff=11397&rp=/store/special-promos) |
| 8 GB KVM Special | 7 / 8 GB / 150 GB | 20 TB | $119.99/yr | [Order the 8 GB plan](https://my.racknerd.com/aff.php?aff=11397&rp=/store/special-promos) |

Storage is RAID-10 SSD on every tier, and the panel is RackNerd's `ctrl` (older writeups still describe SolusVM; `ctrl` adds an HTML5 VNC console, root password reset, one-click apps and inbound firewall rules).

Where the sources disagree is Amsterdam availability. One review states the whole 1/2/4/6/8 GB ladder can be deployed to Amsterdam; another states Amsterdam currently carries a single special and that the 4, 6 and 8 GB tiers are multi-location only. Neither could be verified against an official product page. The practical rule is blunt: **the location dropdown at checkout is the only authority.** Open the general specials page, pick your plan, and look at the location field before you type card details. The general specials page does not pre-select Amsterdam for you.

Amsterdam-only stock does exist in batches. RackNerd has run a flash sale of a 4 GB / 50 GB / 10 TB Amsterdam plan at $22.33/year limited to 10 units, and an earlier pooled promotion listed Amsterdam alongside San Jose, Chicago, Dallas and Atlanta. Those batches sell out and the next one can carry a different price, so a plan you saw last month is not a plan you can buy today.

## What the Amsterdam location actually is

The hardware sits in **Equinix AM5** at Schepenbergweg 42, 1105 AT Amsterdam, a 64,583 sq ft carrier-neutral building. RackNerd has used it since December 2020, when it extended its KVM VPS line to Europe for the first time and the CEO cited Amsterdam's position as Europe's second-largest data center market.

Verified facility specs:

- **Transit:** Cogent and Arelion
- **Power:** N+1 redundant; **cooling:** N+2 redundant
- **Certifications:** ISO 50001:2011, ISO 9001:2015, ISO 14001:2015, SOC 2 Type II
- **Security:** electronic monitoring and secure entry
- **Services on site:** VPS, dedicated servers, colocation, DRaaS, private cloud

One line on RackNerd's own page deserves a careful read: the **100% uptime guarantee covers power**, backed by the redundant plant. It is not a network SLA, and there is no credit regime published for packet loss or transit flaps.

Before ordering, ping the test IP **23.94.101.88** from wherever your users are. RackNerd runs a Looking Glass for the Amsterdam node with ping, traceroute and MTR plus 10 MB, 100 MB and 1 GB test files, so you can measure your own route in about ten seconds. That beats any benchmark screenshot, including the ones in this article.

The peering argument is real: AMS-IX broke the 6 Tbps barrier and peaked at 6.3 Tbps in 2019 according to RackNerd's own copy, which keeps routes to Germany, the UK, France and the Nordics short. One review measured under 1 ms inside Amsterdam and roughly 6–8 ms to Frankfurt, London and Paris. A separate reviewer's working threshold is under 30 ms to major European cities and under 100 ms to the US East Coast.

## What one, two and three years actually cost

Renewal is the question that decides these deals, and RackNerd answers it in its own specials FAQ: *"These RackNerd VPS specials are lifetime recurring. You can renew at the same rate for as long as you decide to keep the service."*

So the 1 GB plan costs **$43.98 over two years and $65.97 over three**, with the monthly equivalent frozen at about $1.83. There is no second-year jump on the SKU you bought. What can change is the price of a *new* batch after yours sells out, which affects new buyers, not your renewal.

The annual deal is also where all the value sits. RackNerd's monthly catalog, per third-party price tracking, lists 1 GB at **$17.99/month** and 4 GB at **$24.59/month**. A year of the 4 GB monthly plan runs to several times the $59.99 annual special. If you genuinely cannot commit to twelve months, the annual specials are the wrong product for you. 👉 [See the lifetime-recurring annual specials](https://my.racknerd.com/aff.php?aff=11397&rp=/store/special-promos)

Price history is worth knowing before you assume $11/year is still on the table. The 1 GB special was **$10.99/year** during Black Friday 2025 and now lists at $21.99. The 2 GB tier moved from $18.93 to $35.99, though the old SKU had 2.5 GB of RAM, so it is not a like-for-like comparison.

## What the price leaves out

**No refund and no trial.** Multiple 2026 reviews confirm RackNerd has no standard money-back guarantee on these VPS plans. A year is a year. The upside is that the downside is capped at $21.99 plus your setup time, which is roughly two coffees.

**Unmanaged, ticket-only support.** You get root and 24/7 tickets for platform failures. Nobody patches your kernel, and there is no live chat.

**Cancellation needs notice.** Reviews document roughly five days' written notice to support before your renewal date to stop a cycle.

**No built-in backups.** RAID-10 survives a dead disk. It does not survive `rm -rf` in the wrong directory. Ship encrypted backups off-site from day one.

**Node quality varies.** Third-party benchmarks from other RackNerd locations show a wide spread: a Buffalo node scored 910 single-core in Geekbench 6, a Dallas node on older Xeons scored 414. Those are not Amsterdam figures and should not be read as such, but they explain why the standard advice is to benchmark your own box on day one. One 2026 review roundup rates RackNerd around 6.5/10 and calls it a cheap utility server, which is a fair description of what you are buying.

If any of that is a dealbreaker, stop here rather than buy and dispute later. 👉 [Check what the current Amsterdam specials include before you commit](https://my.racknerd.com/aff.php?aff=11397&rp=/store/amsterdam-kvm-vps-specials)

## Which tier fits which job

**1 GB ($21.99/yr):** WireGuard or OpenVPN for a handful of devices, a static or small LEMP site, Uptime Kuma, a cron-driven bot. The 3 TB cap works out to about 100 GB a day, which this class of workload will not approach.

**2 GB ($35.99/yr, or $22.38 if the Amsterdam SKU is live):** the point where self-hosting several things at once makes sense. Nextcloud, Gitea, Vaultwarden and a small n8n instance fit; RackNerd's own guidance puts n8n and Coolify at 2 GB and up. It also carries a Minecraft server for a few friends, not a 50-player public one. The ceiling is RAM, not CPU. Once the working set spills past 2 GB with no swap configured, the OOM killer starts closing processes.

**4 GB ($59.99/yr):** the entry point for local AI tooling. Hermes Agent, AnythingLLM, Ollama and LibreChat all want at least 4 GB.

**8 GB ($119.99/yr):** OpenClaw wants 8 GB, and Docker-heavy setups get real breathing room.

Skip the lineup entirely if you need dedicated CPU under sustained production load, managed operations, or an SLA with teeth.

## How the Amsterdam price compares (reference only)

Collected in late 2026 from a single third-party comparison. Prices move, so verify before relying on any of these.

| Provider | Cheapest Amsterdam plan | Price | Billing |
| --- | --- | --- | --- |
| RackNerd | 1 GB / 1 vCPU / 20 GB SSD / 3 TB | $21.99/yr | Annual |
| HOSTKEY | 1 core / 1 GB | from €2/mo | Monthly |
| Melbicom | KVM NVMe entry tier | from €3.90/mo | Monthly |
| EDIS Global | KVM Smart, 1 vCPU | €4.99/mo | Monthly |
| Hostwinds | Unmanaged SSD Cloud 1, 1 vCPU / 1 GB | $4.99/mo | Monthly |
| Scaleway | Stardust1-S | $0.51/mo | Monthly, stock scarce |

The math is straightforward. EDIS at €4.99/month is roughly €60/year for a single vCPU against $21.99 here. Past about four months of commitment, the annual special wins on total cost; below that, or if you specifically need NVMe or month-to-month flexibility, the monthly providers are the sensible choice.

## Ordering: the one step people get wrong

1. Open the specials page and hit Order Now on your plan.
2. **Confirm the location dropdown says Amsterdam.** The general specials page does not pre-select it; the dedicated Amsterdam store page does. Check either way.
3. Choose your OS: CentOS, Rocky Linux, AlmaLinux, Fedora, Debian or Ubuntu. Custom ISOs go through a support ticket.
4. Set a hostname and a root password of at least 8 characters.
5. Pay. PayPal, major cards, Alipay, Bitcoin, Ethereum and USDT are accepted.
6. Expect two emails: order confirmation, then IP and login credentials. Provisioning usually takes minutes.
7. SSH in, then benchmark before migrating anything real. Run a YABS pass, watch `htop` for CPU steal, test your route with `mtr`. If the node underperforms, keep the numbers and open a ticket.

Upgrades are in place and cost the difference, with about a minute of downtime for the reboot.

## FAQ

**Does the price go up on renewal?** No. RackNerd's specials FAQ states the price is lifetime recurring, so the 1 GB plan renews at $21.99 every year you keep it.

**Is there a refund or a trial?** No standard refund policy and no trial on these VPS plans. Assume the first payment is final.

**Can I run Docker or Ollama?** Docker on any tier, including the 1 GB plan. Ollama and other local model tools want 4 GB minimum; OpenClaw wants 8 GB.

**Do I get IPv6 in Amsterdam?** RackNerd provides up to 100 free IPv6 addresses on request in Los Angeles and France and says more locations are coming. Amsterdam is not guaranteed, so open a ticket after ordering to confirm.

**Can I pay monthly?** The specials are annual only. The monthly catalog exists but prices the same hardware far higher, around $17.99/month for 1 GB.

## The decision rule

Need a European exit node for a VPN, a blog or a bot, and you can live with a year's commitment? Take the **1 GB plan at $21.99/year**; you can upgrade later if you outgrow it. Running several self-hosted apps or anything AI-adjacent? The **4 GB plan at $59.99/year** is the better spend, at roughly $5/month for enough RAM to run Ollama. Want month-to-month billing or NVMe specifically? Compare the monthly providers above before buying anything annual.

Two things to confirm before you click: that Amsterdam appears in the location dropdown for the plan you chose, and that you accept there is no refund window. 👉 [Order a RackNerd Amsterdam KVM VPS from $21.99/year](https://my.racknerd.com/aff.php?aff=11397&rp=/store/special-promos)
