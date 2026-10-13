# DMIT coupon code: how to verify a live code at checkout, match it to the right plan line, and lock in a recurring discount

Search "DMIT coupon code" and you get a dozen lists, most of them recycling the same dead promo strings from a Christmas sale that ended months ago. Paste one into checkout, hit Validate, watch it fail, and you're back where you started.

DMIT doesn't run a permanent coupon page. Codes appear around hardware launches, holiday promotions and new-region rollouts, they're tied to one network line (Premium/Pro, Eyeball, or Tier 1) and often to one billing term. The cheapest stock, the stuff that sells out in hours, usually takes no code at all because the discount is already baked into the price.

So the useful skill isn't memorizing a string. It's knowing which code fits the plan you're actually buying, and confirming it before money changes hands. That's what this covers.

## Why DMIT coupon codes behave differently from other hosts

Three things make DMIT's discounting messier than a typical VPS store.

Codes are segmented by product line. A LAX Eyeball code does nothing on a Hong Kong Premium order. The code names usually tell you the scope if you read them: `LAX-EB-...` is Los Angeles Eyeball, `202510_HKG_TYO_PRO_...` covers Hong Kong and Tokyo Premium, `2025-TYO-T1-...` is Tokyo Tier 1 only.

Billing term is part of the condition. Several codes only validate on quarterly, semi-annual or annual orders, and the monthly ones are a different string entirely. Pick the term first, then the code.

Some codes recur, some don't. A "RECURRING" code keeps applying on every renewal, which over three years is worth far more than a one-time percentage. Codes with no such marker generally apply to the first invoice.

And the flash stock is exempt. The budget tiers that get the "restock" announcements, the WEE and CORONA and MALIBU models, are priced as standalone deals. Community trackers list them explicitly as having no coupon. Trying to stack a code on a $36.90/year plan is usually a waste of a minute.

## The codes currently circulating

Everything below comes from public affiliate trackers and community posts, not from a DMIT coupon page. DMIT rotates and retires these without notice, so treat the table as candidates to test, not as a guarantee. The countdown clock on validity starts the moment the promotion ends, and several of these are seasonal.

| Code | Applies to | Discount | Term requirement | Notes |
| --- | --- | --- | --- | --- |
| `2025-XMAS-LAX-PRO-EB-ANNUALLY-STARTER-AND-HIGHER-15OFF-RECURRING` | LAX Pro / EB, STARTER tier and up | 15% off + 10% cashback | Annual | Roughly 25% combined value; recurring |
| `2025-XMAS-LAX-PRO-EB-10-OFF-RECURRING` | LAX Pro / EB, standard plans | 10% off + 5% cashback | Any regular term | Recurring |
| `2025-XMAS-LAX-T1-10-OFF-RECURRING` | LAX Tier 1 | 10% off + 5% cashback | Any regular term | Excludes WEE |
| `LAX-EB-LAUNCH-NON-MONTHLY-RECURRING-20OFF` | LAX EB, TINY and above | 20% off | Quarterly or longer | Recurring; the strongest single-line code |
| `202510_HKG_TYO_PRO_20OFF_RECURRING` | HKG Pro / TYO Pro | 20% off | Quarterly or longer | Recurring |
| `202510_HKG_TYO_T1_30OFF_RECURRING` | HKG Tier 1 / TYO Tier 1 | 30% off | Quarterly or longer | Excludes WEE |
| `2025-TYO-T1-HI-GSL-NON-MONTHLY-30OFF` | TYO Tier 1, TINY and above | 30% off | Quarterly or longer | Tokyo Tier 1 only |
| `2025-TYO-T1-HI-GSL-MONTHLY-10OFF` | TYO Tier 1, TINY and above | 10% off | Monthly | The monthly counterpart of the code above |
| `Lite-Annually-Recur-30OFF` | Standard / Lite network line | 30% off | Annual | Long-running, reported as still valid |
| `Lite-Semi-Annually-Recur-20OFF` | Standard / Lite network line | 20% off | Semi-annual | Long-running, reported as still valid |
| `2025-EXISTING-CUSTOMER-10OFF` | Wide range, including Tokyo Pro | 10% off | Any | Only works if the account already has at least one completed order |

Two older LAX-only codes, `Existing-Super20%` and `NEW-Super13%`, still show up on review sites from the AN4 generation. They're tied to plan names DMIT has since replaced, so don't count on them.

If none of these validate, that's information, not a dead end: it usually means the plan you selected is flash stock or the promotion window closed.

## How to apply a code without wasting an order

The order flow is standard WHMCS, and there's a validation step before payment, so you can test safely.

1. Pick your plan and go to the order page. Check the plan name matches the code's scope, especially the region prefix.
2. Choose the billing cycle the code requires. A non-monthly code will simply reject a monthly selection.
3. Find the coupon field on the configuration or checkout screen and paste the code.
4. Click Validate Code. A valid code shows the adjusted total immediately. An invalid one gives you an error and no change.
5. Read the new total before paying, and check whether the discount is marked as recurring on the summary.

One code per order in normal practice. If a promo advertises "15% off plus 10% cashback," the cashback portion is handled through the account, not as a second coupon field.

Ready to test them against your plan? 👉 [Open the DMIT order page and validate a code before checkout](https://www.dmit.io/aff.php?aff=12046)

## A recurring 20% beats a one-time 30% most of the time

This is the part most coupon lists skip. If you're staying on the same plan for a year or more, a smaller recurring discount compounds.

Take LAX Eyeball TINY at $10.90/month. That's $130.80 over twelve months. A 20% recurring code drops it to $104.64 a year, and the same 20% comes off again at every renewal for as long as the plan exists. A one-time 30% code would save $39.24 once, then the bill returns to $130.80.

Recurring codes are worth hunting hardest when you expect to keep the machine, which for a relay, a production site or a dev box is the normal case.

The counter-example is the flash stock. A LAX Tier 1 WEE runs $36.90/year for 1 core, 1GB RAM, 20GB SSD and 1TB of monthly traffic on a 4Gbps port. No code applies, and the equivalent monthly Tier 1 TINY at $6.90/month totals $82.80 over a year for the same 1 core and 1GB, with 2TB of traffic instead of 1TB. If traffic volume isn't your limiting factor, the annual flash plan beats any discounted monthly order, code or no code.

That's the real question behind a coupon search: not "what's the biggest percentage," but "what's the cheapest twelve months for the configuration I need."

## Which DMIT plans refuse a coupon

Based on how these deals are structured, expect no code to apply on:

- Limited/restock tiers priced as standalone deals, typically the WEE entries and the periodically restocked bargain models
- Model lines that have already been retired from the catalogue (the older LAX AN4 lineup and its MALIBU and CORONA variants, for instance)
- Any plan where the code's region or tier doesn't match the plan you selected, which isn't a refusal so much as a mismatch

Some codes also carry an account condition rather than a plan condition. The existing-customer code requires a prior completed order on the account. A brand-new account can't use it no matter which plan is in the cart.

## The full plan list, so you can match a code to a real plan

Prices and configurations below are compiled from DMIT product listings as published across multiple trackers and reseller pages. DMIT revises prices, retires hardware generations and rotates stock frequently, and the same nominal tier can shift between platforms. Confirm the figure on the order page before paying.

### Los Angeles (LAX)

LAX.AS3.Pro, the CN2 GIA line: China Telecom return via AS4809, China Unicom direct via AS4837, China Mobile inbound via Hong Kong, all three return over CN2 GIA. Overage throttles to 4Mbps rather than shutting the machine off.

| Plan | CPU / RAM / SSD | Traffic & port | Price | Billing | Order |
| --- | --- | --- | --- | --- | --- |
| LAX.AS3.Pro.TINY | 1 core / 2GB / 20GB | 1TB @ 1Gbps | $10.90 | Monthly | [Check LAX Pro TINY pricing](https://www.dmit.io/aff.php?aff=12046&pid=253) |
| LAX.AS3.Pro.Pocket | 2 cores / 2GB / 40GB | 1.5TB @ 4Gbps | $16.90 | Monthly | [Check LAX Pro Pocket pricing](https://www.dmit.io/aff.php?aff=12046&pid=254) |
| LAX.AS3.Pro.STARTER | 2 cores / 2GB / 80GB | 3TB @ 10Gbps | $34.90 | Monthly | [Check LAX Pro STARTER pricing](https://www.dmit.io/aff.php?aff=12046&pid=255) |
| LAX.AS3.Pro.MINI | 4 cores / 4GB / 80GB | 5TB @ 10Gbps | $62.90 | Monthly | [Check LAX Pro MINI pricing](https://www.dmit.io/aff.php?aff=12046&pid=256) |
| LAX.AS3.Pro.MICRO | 4 cores / 4GB / 160GB | 7TB @ 10Gbps | $87.90 | Monthly | [Check LAX Pro MICRO pricing](https://www.dmit.io/aff.php?aff=12046&pid=257) |
| LAX.AS3.Pro.MEDIUM | 6 cores / 8GB / 160GB | 14TB @ 10Gbps | $199.90 | Monthly | [Check LAX Pro MEDIUM pricing](https://www.dmit.io/aff.php?aff=12046&pid=258) |

LAX.AS3.EB, the Eyeball line: China Telecom load-balanced between AS9929 and premium China Mobile routes, Unicom over AS9929, Mobile over CMIN2. Same hardware generation, noticeably more traffic at the same price points, which is why the EB launch code is the one people hunt.

| Plan | CPU / RAM / SSD | Traffic & port | Price | Billing | Order |
| --- | --- | --- | --- | --- | --- |
| LAX.AS3.EB.TINY | 1 core / 2GB / 20GB | 1.5TB @ 2Gbps | $10.90 | Monthly | [Check LAX EB TINY pricing](https://www.dmit.io/aff.php?aff=12046&pid=259) |
| LAX.AS3.EB.Pocket | 2 cores / 2GB / 40GB | 3TB @ 4Gbps | $16.90 | Monthly | [Check LAX EB Pocket pricing](https://www.dmit.io/aff.php?aff=12046&pid=260) |
| LAX.AS3.EB.STARTER | 2 cores / 2GB / 80GB | 5TB @ 10Gbps | $34.90 | Monthly | [Check LAX EB STARTER pricing](https://www.dmit.io/aff.php?aff=12046&pid=261) |
| LAX.AS3.EB.MINI | 4 cores / 4GB / 80GB | 10TB @ 10Gbps | $62.90 | Monthly | [Check LAX EB MINI pricing](https://www.dmit.io/aff.php?aff=12046&pid=262) |
| LAX.AS3.EB.MICRO | 4 cores / 4GB / 160GB | 14TB @ 10Gbps | $87.90 | Monthly | [Check LAX EB MICRO pricing](https://www.dmit.io/aff.php?aff=12046&pid=263) |
| LAX.AS3.EB.MEDIUM | 6 cores / 8GB / 160GB | 30TB @ 10Gbps | $199.90 | Monthly | [Check LAX EB MEDIUM pricing](https://www.dmit.io/aff.php?aff=12046&pid=264) |

LAX.AS3.T1, the international BGP line: no China-specific routing, larger ports, more traffic, lowest entry price in the LAX catalogue.

| Plan | CPU / RAM / SSD | Traffic & port | Price | Billing | Order |
| --- | --- | --- | --- | --- | --- |
| LAX.AS3.T1.WEE | 1 core / 1GB / 20GB | 1TB @ 4Gbps, 100Mbps after overage | $36.90 | Annual | [Check LAX T1 WEE pricing](https://www.dmit.io/aff.php?aff=12046&pid=270) |
| LAX.AS3.T1.TINY | 1 core / 1GB / 20GB | 2TB @ 4Gbps | $6.90 | Monthly | [Check LAX T1 TINY pricing](https://www.dmit.io/aff.php?aff=12046&pid=271) |
| LAX.AS3.T1.STARTER | 2 cores / 2GB / 40GB | 4TB @ 10Gbps | $12.90 | Monthly | [Check LAX T1 STARTER pricing](https://www.dmit.io/aff.php?aff=12046&pid=272) |
| LAX.AS3.T1.MINI | 2 cores / 4GB / 80GB | 8TB @ 10Gbps | $21.90 | Monthly | [Check LAX T1 MINI pricing](https://www.dmit.io/aff.php?aff=12046&pid=273) |
| LAX.AS3.T1.MICRO | 4 cores / 4GB / 120GB | 16TB @ 10Gbps | $32.90 | Monthly | [Check LAX T1 MICRO pricing](https://www.dmit.io/aff.php?aff=12046&pid=274) |

### Hong Kong (HKG)

Hong Kong sits physically closest to mainland China, which is why its Premium pricing is several times the LAX equivalent. The T1 line trades that proximity advantage for a much lower price and bigger traffic allowances. Stock on the Hong Kong Eyeball line has come and gone repeatedly across recent restocks, so don't assume it's purchasable on the day you read this.

| Plan | CPU / RAM / SSD | Traffic & port | Price | Billing | Order |
| --- | --- | --- | --- | --- | --- |
| HKG.AS3.T1.WEE | 1 core / 1GB / 20GB | 1TB @ 4Gbps | $36.90 | Annual | [Check HKG T1 WEE pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG.AS3.T1.TINY | 1 core / 1GB / 20GB | 2TB @ 4Gbps | $6.90 | Monthly | [Check HKG T1 TINY pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG.AS3.T1.STARTER | 1 core / 2GB / 40GB | 4TB @ 10Gbps | $12.90 | Monthly | [Check HKG T1 STARTER pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG.AS3.T1.MINI | 2 cores / 2GB / 60GB | 8TB @ 10Gbps | $21.90 | Monthly | [Check HKG T1 MINI pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG.AS3.T1.MICRO | 4 cores / 4GB / 80GB | 16TB @ 10Gbps | $32.90 | Monthly | [Check HKG T1 MICRO pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG.AS3.T1.MEDIUM | 4 cores / 8GB / 160GB | 32TB @ 10Gbps | $49.90 | Monthly | [Check HKG T1 MEDIUM pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG.AS3.T1.LARGE | 8 cores / 16GB / 320GB | 64TB @ 10Gbps | $99.90 | Monthly | [Check HKG T1 LARGE pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG.AS3.T1.GIANT | 8 cores / 24GB / 640GB | 128TB @ 10Gbps | $199.90 | Monthly | [Check HKG T1 GIANT pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AS3 TINY | 1 core / 1GB / 20GB | 500GB @ 1Gbps | $39.90 | Monthly | [Check HKG Premium TINY pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AS3 STARTER | 1 core / 2GB / 40GB | 1TB @ 1Gbps | $79.90 | Monthly | [Check HKG Premium STARTER pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AS3 MINI | 2 cores / 2GB / 60GB | 1.5TB @ 1Gbps | $126.90 | Monthly | [Check HKG Premium MINI pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AS3 MICRO | 2 cores / 4GB / 80GB | 2TB @ 1Gbps | $179.90 | Monthly | [Check HKG Premium MICRO pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AS3 MEDIUM | 4 cores / 4GB / 160GB | 2.5TB @ 1Gbps | $239.90 | Monthly | [Check HKG Premium MEDIUM pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AN5 MINI | 2 cores / 2GB / 80GB | 1.5TB @ 1Gbps | $149.90 | Monthly | [Check HKG Premium AN5 MINI pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AN5 MICRO | 2 cores / 4GB / 160GB | 2TB @ 1Gbps | $159.90 | Monthly | [Check HKG Premium AN5 MICRO pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AN5 MEDIUM | 4 cores / 4GB / 160GB | 2.5TB @ 1Gbps | $180.00 | Monthly | [Check HKG Premium AN5 MEDIUM pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AN5 LARGE | 4 cores / 8GB / 320GB | 3TB @ 1Gbps | $240.00 | Monthly | [Check HKG Premium AN5 LARGE pricing](https://www.dmit.io/aff.php?aff=12046) |
| HKG Pro AN5 GIANT | 8 cores / 16GB / 640GB | 6TB @ 1Gbps | $500.00 | Monthly | [Check HKG Premium AN5 GIANT pricing](https://www.dmit.io/aff.php?aff=12046) |

The AN5 platform runs AMD EPYC 9005 generation hardware with larger disks than the AS3 generation at similar or slightly higher prices. On the entry tiers the AS3 version is usually the cheaper way in; the AN5 tiers only start at MINI.

### Tokyo (TYO)

Tokyo is the smallest catalogue of the three, and the plan names are harder to pin down because the Premium line has appeared under different model names across restocks.

| Plan | CPU / RAM / SSD | Traffic & port | Price | Billing | Order |
| --- | --- | --- | --- | --- | --- |
| TYO.T1.WEE | 1 core / 1GB / 20GB | 1TB @ 4Gbps, 50Mbps after overage | $36.90 | Annual | [Check Tokyo T1 WEE pricing](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.TINY | 1 core / 1GB / 20GB | 2TB | $6.90 | Monthly | [Check Tokyo T1 TINY pricing](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.STARTER | 1 core / 2GB / 40GB | 4TB | $12.90 | Monthly | [Check Tokyo T1 STARTER pricing](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.MINI | 2 cores / 2GB / 60GB | 8TB | $21.90 | Monthly | [Check Tokyo T1 MINI pricing](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.MICRO | 4 cores / 4GB / 80GB | 16TB | $32.90 | Monthly | [Check Tokyo T1 MICRO pricing](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.MEDIUM | 4 cores / 8GB / 160GB | 32TB | $49.90 | Monthly | [Check Tokyo T1 MEDIUM pricing](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.LARGE | 8 cores / 16GB / 320GB | 64TB | $99.90 | Monthly | [Check Tokyo T1 LARGE pricing](https://www.dmit.io/aff.php?aff=12046) |
| TYO.T1.GIANT | 8 cores / 24GB / 640GB | 128TB | $199.90 | Monthly | [Check Tokyo T1 GIANT pricing](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro (Shinagawa) | 1 core / 2GB / 60GB | 800GB @ 500Mbps | $239.90 | Annual, or $69.90 quarterly | [Check Tokyo Premium pricing](https://www.dmit.io/aff.php?aff=12046) |

The Tokyo Premium line is the one place where the loyalty code matters most. Spending above roughly $3.33/month on the account qualifies you for the existing-customer discount, which is a straight 10% off on top of an already expensive plan.

## Matching a code to the plan you actually need

If you're running a site that serves mainland China visitors, the LAX Pro line is the one the 15% annual code targets, and the code plus a year of prepayment is where the discount lands hardest. Eyeball is the better match if your audience skews toward China Mobile and China Unicom: the same price as Pro buys 50% more traffic on TINY and double on STARTER, and the EB launch code is the biggest recurring discount in the whole list.

If you don't need China-optimized routing, don't buy it. The Tier 1 line exists for exactly this, and a `LAX.AS3.T1.WEE` at $36.90/year with no code is cheaper than any discounted monthly Pro plan. The 10% and 30% T1 codes are worth applying only when you need a bigger tier, where the annual flash price isn't available.

Hong Kong is a latency purchase, not a value purchase. The Premium plans cost roughly four times their LAX equivalents for less traffic, and the only reason to pay that is proximity. The 20% Hong Kong Premium code softens the entry price meaningfully on the quarterly term, and the T1 30% code applies to the international line if you need a Hong Kong IP without China routing.

Tokyo makes sense if your users are in Japan or Northeast Asia, or if you want a Tier 1 machine that handles China Mobile traffic reasonably well without CN2 pricing.

## The policies that matter more than a few percentage points

A coupon saves you a fixed amount once. These terms are what determine whether a bad month costs you a machine.

Refunds: a full refund within three days of purchase if you've used under 30GB of transfer, and a pro-rated refund within 30 days based on remaining time or traffic, minus payment gateway fees. The three-day window is short, so test routing and speeds immediately after delivery rather than at the end of the week.

IP replacement: if an IP becomes unreachable, DMIT allows a free replacement on a roughly 15-day cycle. For anyone running services aimed at mainland China, where IPs get blocked, this matters more than a discount.

Overage handling: traffic over the plan limit throttles the port instead of suspending the server. A LAX Pro plan drops to 4Mbps, Tier 1 plans hold 100Mbps on the entry tiers. Your site stays up, slowly, and the surprise bill doesn't arrive.

Payment: Alipay, PayPal and credit cards are all supported, along with Chinese-language support.

## Quick answers

Does DMIT have a permanent coupon page? No. Codes appear with promotions and get retired. There's no standing public code list on the official site.

Will the code still work next month? If it carries a `RECURRING` marker, the discount repeats on renewals, but the code itself can still be deactivated for new orders at any time. Validate before every purchase.

Can I stack two codes? Not in practice. One coupon field, one code per order.

Why did a valid-looking code fail? Region or plan mismatch, wrong billing term, or a retired string. Check the prefix against the product line first.

Should I buy the flash plan or the discounted regular plan? Compare twelve-month totals for the configuration you need, not the headline percentage. A $36.90 annual flash plan with no code often beats a discounted monthly plan with a working one.

Is now a good time to buy? Stock and pricing shift constantly, and restocks of the cheap tiers sell out within days. If a plan you want is in stock and a code validates, that combination tends not to last. 👉 [Head to DMIT and validate your code against the current plan list](https://www.dmit.io/aff.php?aff=12046)
