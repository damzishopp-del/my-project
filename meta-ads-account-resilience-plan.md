# Meta Ads Account Resilience Plan
### Warm-up, launch, scaling and long-term compliance for a white-hat e-commerce brand

**Scope:** Facebook and Instagram ads for a store that sells legitimate physical products.
**Budget path:** about $5/day during warm-up, rising to **150 ILS/day (about $40)** for one cold-audience Sales (acquisition) campaign that sends traffic to a standard product page.

---

## 0. Read this first: three facts that set the ground rules

1. **Meta does not publish how its enforcement works.** The detection mechanisms below come from Meta's published policies, its Business Help Center documentation, and patterns that show up across many advertisers. Where a point is a working rule from practice and not documented Meta behavior, this plan says so. Don't trust anyone who claims to know the exact thresholds.

2. **A "warm-up" doesn't build trust by itself; a clean history does.** Spending $5/day doesn't flip a switch. What Meta's risk systems weigh is a record of verified identity, successful charges, approved ads, normal activity pace, steady spend growth and satisfied customers. The slow ramp in Section 3 works because it builds that record before you ask for more spend.

3. **Don't use new identities to get around an old restriction.** If your personal profile, Business Portfolio or Page currently has an advertising restriction, a new ad account will be linked back to it within days. Meta connects assets through identity documents, devices, IP addresses, payment cards, domains, Pages and admins. Using a second profile, a rented or bought account, or a "farm" account to get around a restriction breaks Meta's *Circumventing Systems* policy. That leads to permanent bans that also hit every linked asset, and it's the most common reason "fresh" accounts die in their first week.
   - **Before you do anything else**, open **Account Quality** (`facebook.com/accountquality`) on your real profile and your Business Portfolio. If anything is restricted, use **Request review** there first. Build the new setup only on assets that show no active restrictions.

---

## 1. Why you were banned before, and how Meta's systems catch each cause

Meta's integrity systems score each account for risk using many signals at once. **Your past bans most likely didn't come from a single cause. Several signals stacked up.** A new account (no trust) that launches many ads (high activity) with aggressive claims (policy risk) and then multiplies its budget (spend jump) and fails a charge (payment risk) looks almost exactly like a fraudster or a stolen account. Every item below adds to that risk score.

### 1.1 Too many ads launched in a fresh account

| | |
|---|---|
| **What happened** | A new ad account created many campaigns, ad sets and ads in its first hours or days. |
| **Why it looks bad** | Fraud operations and hijacked accounts work exactly this way: they launch a lot at once to spend as much as possible before they're shut down. A legitimate new advertiser usually starts with one or two campaigns. |
| **How it's detected** | Activity-rate signals (new objects per hour or day compared with account age and spend history). Every new ad also goes through automated review, so each ad is another chance for a rejection. Several rejections in a short window count heavily against a new account. |
| **The fix** | Strict limits on how much you create (Section 3.4). One campaign, one ad set and two or three ads at launch. |

### 1.2 Misleading claims

| | |
|---|---|
| **What happened** | Ad copy, on-image text or the landing page made claims Meta classifies as deceptive: exaggerated results, guarantees, fake urgency, or "too good to be true" offers. |
| **Relevant policies** | *Unacceptable Business Practices*, *Misinformation*, *Low-Quality or Disruptive Content* (exaggerated claims, unrealistic outcomes, sensationalized language), and *Personal Health and Appearance*. |
| **How it's detected** | Text classifiers on the primary text, headline and description. **OCR** reads text inside images. **Speech-to-text** transcribes video audio. A **crawler checks the landing page**, so claims on the product page count too. After launch, user feedback ("Hide ad", "Report ad"), negative comments, and the **post-purchase survey that sets your Page's feedback score** keep feeding the system. |
| **The fix** | A claims ladder (Section 4.3), proof on file for every factual claim, and the landing page saying the same thing as the ad (Section 2.5). |

### 1.3 Too much body exposure

| | |
|---|---|
| **What happened** | Images or videos showed too much skin, implied nudity, close-up crops of body parts, or suggestive poses, even though the product itself was harmless. |
| **Relevant policies** | *Adult Nudity and Sexual Activity* and *Adult Content* (which covers sexually suggestive content even with no nudity). For health or beauty products, *Personal Health and Appearance* also bans focusing on specific body parts and before/after images. |
| **How it's detected** | Image classifiers estimate how much of the frame is skin, how close the crop is to sensitive areas, the pose and the context. **Videos are sampled frame by frame, and the thumbnail and first frame weigh heavily.** One bad frame can get the whole ad rejected. |
| **The fix** | The visual rules in Section 4.5. Product first, models fully clothed, catalog-style framing. |

### 1.4 Multiplying budgets too quickly

| | |
|---|---|
| **What happened** | Budgets jumped by large multiples (for example $5 to $50, or doubled several times within days) on an account with little payment history. |
| **Why it looks bad** | A sudden jump in spend on a new account is a classic sign of account takeover or card fraud. It also raises your financial exposure: you get billed more often, at larger amounts, against a card Meta hasn't seen pay much yet. That's how a budget jump turns into a **payment failure** (Section 1.6). |
| **How it's detected** | Spend-rate checks against account age and payment history. New accounts also have a **daily spending limit** set by Meta that only goes up after successful payments. Pushing against it triggers risk review. |
| **The fix** | The step-by-step ramp in Section 3.3. Each budget step depends on successful charges and a clean account. |

### 1.5 Hacked ad accounts or breaches

| | |
|---|---|
| **What happened** | An attacker got into a profile or Business Portfolio and ran their own ads (often scams or prohibited products), or changed admins and payment methods. Meta then disabled the account and often every asset linked to it. |
| **Common attack routes** | (a) Phishing messages pretending to be "Meta Support" or "Page violation / copyright notice". (b) **Session-cookie-stealing malware** from cracked software, fake "ad tools", "ad report" ZIP or RAR files, or shady browser extensions. **This gets past 2FA.** (c) Old admins, freelancers or agencies whose access was never removed. |
| **How it's detected** | New log-in locations and devices, admin changes, payment method changes, a sudden jump in spend, and ads unlike your history. Meta usually disables first and investigates later. |
| **The fix** | The security protocol in Section 2.2, plus an **account spending limit** that caps the damage. |

### 1.6 Payment failures and billing problems

| | |
|---|---|
| **What happened** | Charges were declined, so the account had an unpaid balance. Ads stopped and the account was restricted. Repeated failures led to a disable. |
| **Common causes in Israel** | The bank blocks foreign merchant charges (Meta bills through Meta Platforms Ireland), online or international transactions aren't enabled, 3-D Secure fails, the card limit is too low, or the **account currency differs from the card currency** (which adds conversion fees and risk flags). |
| **How it's detected** | Directly. Every declined charge is logged against the account, and **adding and removing many cards** (especially in different names) is a strong fraud signal on its own. |
| **The fix** | The payment protocol in Section 2.3. |

### 1.7 About your first-person ("I" instead of "You") idea

You're **partly right, but not for the reason you think.**

- **What it actually avoids:** the *Personal Attributes* policy. That policy bans ads that **state or imply the viewer's personal attributes** (health, medical or mental condition, weight, finances, age, religion, race or ethnicity, sexual orientation, criminal record, and so on). "Struggling with back pain?" or "Are *you* overweight?" breaks it. "I used to wake up with back pain" usually doesn't.
- **What it doesn't do:** lower how strictly the system reviews you. "You" isn't banned ("You'll love how light it is" is fine). **First-person claims are reviewed exactly like any other claim.** "I lost 10 kg in two weeks" is still an unrealistic-outcome claim, and in health or appearance categories it's still before/after territory.
- **One more catch:** a first-person "testimonial" that's made up is itself a deceptive practice. Use real customer stories (with written consent) or the founder's own honest voice.

Keep using first person. It does help. But it's a framing tool, not protection against review. The full framework is in Section 4.

---

## 2. Long-term prevention: the foundations (keep these for years)

### 2.1 Identity and asset setup

Set up a clean, simple, fully verified structure, and keep it that way:

```
Your real personal profile (aged, real name, real photo, 2FA)
 └── ONE Business Portfolio (formerly Business Manager), business verified
      ├── Facebook Page (brand) + linked Instagram professional account
      ├── ONE ad account (currency ILS, timezone Asia/Jerusalem)
      ├── Pixel / dataset + Conversions API
      ├── Verified domain (your store domain)
      └── Second admin: a trusted person with their own real profile and 2FA
```

Checklist:
- [ ] **Personal profile:** real name, real photo, some normal activity, ID-verified if Meta asks, no restrictions in Account Quality.
- [ ] **Business Portfolio:** legal business name, address and phone **exactly as on your official registration documents and invoices**. Finish **Business Verification** (Security Center → Business verification).
- [ ] **Page:** clear branding, an About section with contact details, website and email, and **at least 6–10 organic posts** (product photos, behind the scenes, customer photos you have permission to use) before you run ads. An empty Page next to a new ad account is a weak trust signal. Check the **Page Transparency** section is filled in.
- [ ] **Instagram:** a professional account linked to the Page, with a few posts.
- [ ] **Domain verification** for your store domain (Brand Safety → Domains).
- [ ] **Pixel and Conversions API (CAPI)** installed. Most Shopify, WooCommerce and Wix stores can do this through the official Meta integration. Check events in Events Manager (PageView, ViewContent, AddToCart, InitiateCheckout, Purchase), and aim for an event match quality of 6+.
- [ ] **Ad account currency = ILS and timezone = Asia/Jerusalem.** Pick these carefully. **You can't change them later** without creating a new ad account.
- [ ] **Optional but useful: Meta Verified for Business** (where available). It gives you access to real human support, which is far more valuable than any trick when something goes wrong.

**Don't:** create several Business Portfolios, several ad accounts "as backups", pages you don't need, or extra profiles. Every extra asset is one more thing that can be linked to a problem, and it adds nothing to your resilience.

### 2.2 Security protocol (this prevents a repeat of the hacked-account ban)

| Control | How to do it |
|---|---|
| **Strong 2FA** | Use an authenticator app (Google Authenticator, Authy, 1Password) or a **physical security key**. Don't use SMS only. Save the recovery codes offline. |
| **Require 2FA for everyone in the Business Portfolio** | Security Center → Two-factor authentication → *Required for everyone*. |
| **Two admins, no more** | You and one trusted person. Everyone else gets *partial* or *employee* access to only the assets they need. Never make freelancers admins. Give agencies **partner access** to specific assets instead. |
| **Quarterly access audit** | Remove anyone who no longer needs access. Check *People*, *Partners*, *System users* and *Apps*. |
| **Clean device** | Keep a dedicated browser profile just for ad management. Install no unknown extensions. Never run cracked software, "free ad tools", or ZIP or RAR "reports" sent by strangers. Run up-to-date antivirus. |
| **Phishing rule** | Meta never threatens to delete your Page over Messenger and never asks for your password or 2FA code. Check any "official" email under **Settings → Security → Recent emails from Meta**. Any notice that's real will also appear in Account Quality and Business Support Home. |
| **Email security** | The email on your profile and Business Portfolio must have its own strong 2FA. Whoever controls your email controls your account. |
| **Log-in alerts** | Turn on unrecognized-log-in alerts. Check *Where you're logged in* once a month and end unknown sessions. |
| **Spending cap that limits damage** | Set an **Account Spending Limit** (Billing → Payment settings) at about 1.3× your planned monthly spend (for example about 6,000 ILS once you're spending 150 ILS/day). If someone gets in, they can't run up an unlimited bill, and you're the one who decides when to raise it. |

### 2.3 Payment protocol (this prevents a repeat of the billing ban)

1. **One main card in your name or the business's name, matching the profile and Business Portfolio details.** Prefer a standard card from your bank over prepaid, gift or disposable virtual cards.
2. **Call your bank before launch.** Ask them to allow recurring **foreign online charges from "Facebook / Meta Platforms Ireland"**, confirm 3-D Secure is active, and check the card's monthly limit leaves at least **3× your planned monthly ad spend** of headroom.
3. **Bill in ILS** (the account currency) to avoid currency mismatch.
4. **Add one backup payment method from the same owner.** Don't keep adding and removing cards. Make every payment-method change deliberate and rare.
5. **Never leave a failed charge unpaid.** If a charge fails: (a) pay the balance right away with **Pay now**, (b) don't launch or edit anything until it's settled, (c) fix the cause with the bank before ads resume.
6. **Let the billing threshold rise naturally.** New accounts are charged often, at small amounts. Every successful charge builds trust. **Successful charges are the most valuable part of the warm-up.**
7. **Keep invoices.** Download the monthly receipts. If there's ever a dispute, they prove you have a clean payment record.
8. **Never dispute a Meta charge with your bank (chargeback)**. Settle it through Meta's billing support instead. A chargeback is one of the fastest ways to get an ad account disabled.

### 2.4 Following ad policy (the standing rules)

- Read Meta's **Advertising Standards** once in full, then quickly again every quarter. Policies change.
- Keep a **claims proof file** (a shared folder): for every factual claim (materials, dimensions, certifications, "ships in 3 days", "1-year warranty"), keep the supporting document.
- **Don't edit a live ad just to "refresh" it.** Every edit sends it back to review and resets learning.
- **When an ad is rejected:**
  1. Read the exact policy named in the rejection.
  2. If the rejection is **valid**, don't resubmit the same thing. Make a clearly compliant new version.
  3. If it's **wrong**, request a review **once** through Account Quality, with a short, polite explanation.
  4. **Never** keep editing and resubmitting a rejected ad. Repeated violations add up into an account-level restriction.
- Don't use Meta's or Facebook's names or logos, celebrity images, fake UI (play buttons, notification badges, fake "close" buttons), countdowns that aren't real, or strikethrough prices you've never actually charged.

### 2.5 Landing page and store hygiene (Meta's crawler checks this)

Your product page is part of the ad review. Make sure it has:
- [ ] Clear **business identity**: name, contact email, phone or WhatsApp, and physical or registered business address.
- [ ] **Shipping policy, return/refund policy, privacy policy, terms**, all linked in the footer.
- [ ] **The same price, offer and claims as the ad.** If the ad says "Free shipping over 200 ILS", the page must say it too.
- [ ] **Real reviews only.** No imported fake reviews, no "23 people are viewing this", no fake stock counters.
- [ ] A fast, mobile-friendly page with HTTPS and no surprise pop-ups or redirects.
- [ ] **Delivery promises you can keep.** Late deliveries cause negative post-purchase survey answers, which lower your Page's **feedback score**. A low score reduces delivery and can lead to restrictions. Customer service is a compliance issue.

### 2.6 Operational discipline (the habits that keep an account healthy for years)

- **Change log:** a simple sheet with date, what changed, why, and the result. Before each change, ask: "When did I last make a significant change here?" Follow the 72-hour rule (Section 3.5).
- **Weekly checks:** Account Quality, Business Support Home, Payment Activity, and ad feedback (comments and hides).
- **Monthly:** security audit (sessions, admins, apps), a backup of creatives and copy, review of Page feedback score.
- **Quarterly:** policy re-read, access audit, a call to the bank about card limits if spend has grown.
- **Don't rely on Meta alone.** Build email/SMS lists, Google Shopping and organic social so the business survives any single platform problem. This is the most important protection for the long run.

---

## 3. The phased warm-up and scaling protocol

### 3.1 Principles

- **One campaign, one ad set, a few ads.** Simplicity is your safety.
- **The budget only goes up when every gate passes** (Section 3.6). The calendar is a ceiling, not a promise.
- **Each budget step is at most about 20–25%,** with **at least 3 days** between steps. (This is a widely used working rule, not a published Meta threshold. It keeps both risk systems and the delivery algorithm stable.)
- **Be realistic about results:** at 20–100 ILS/day, a purchase-optimized ad set won't reach the ~50 conversions per week Meta needs to finish its learning phase. It will show **"Learning limited."** That's expected and fine during warm-up. **The goal of Phase 1–3 is building trust, not profit.**

### 3.2 Phase 0: setup (Day −14 to Day 0, no ad spend)

| Day | Action |
|---|---|
| −14 | Check Account Quality on your profile. Secure the profile and email (2FA). Create or clean up the Business Portfolio and start Business Verification. |
| −12 | Page and Instagram: finish the profile and start posting (2–3 posts a week). |
| −10 | Domain verification. Install pixel and CAPI, then test events with a test purchase. |
| −7 | Bring the landing page up to the checklist in Section 2.5. Call your bank (Section 2.3). |
| −5 | Create **one** ad account (ILS, Asia/Jerusalem). Add the main card and the backup card. Set the account spending limit. |
| −3 | Prepare 4–6 compliant creatives (Section 4) and run every one through the pre-flight check (Section 4.7). **Launch only 2–3.** Keep the rest as reserves. |
| 0 | Final check: Business Verification approved or pending without problems, events firing, no restrictions anywhere. |

*Optional:* If the Page is brand new, a small boosted post (for example 10–15 ILS/day for 3–5 days) on your best organic post can give the account a first successful charge before the Sales campaign. It's not required.

### 3.3 Budget schedule: about $5/day to 150 ILS/day

**Campaign setup (create once, then leave it alone):**
- **Objective:** Sales. **Conversion location:** Website. **Optimization event:** Purchase. (If your pixel has never recorded a purchase, you can start on Add to Cart and later open a **new** Purchase ad set at steady state. Changing the event on an existing ad set resets learning.)
- **Budget level:** ad-set budget (ABO) with one ad set. You'll move to campaign budget only when you have more ad sets.
- **Audience:** Israel (or your market), suitable ages, **broad** targeting or Advantage+ audience. No complicated interest stacks.
- **Placements:** Advantage+ placements.
- **Bid strategy:** Highest volume (lowest cost). No cost caps during warm-up.
- **Ads:** 2–3, each a different angle (Section 4.2).

| Phase | Days | Daily budget (ILS) | ≈ USD | Increase | What you're allowed to do |
|---|---|---|---|---|---|
| **1 – Foundation** | 1–7 | **20** | ~$5 | — | Launch 1 campaign / 1 ad set / 2–3 ads. **No changes for the first 72 hours.** |
| **2 – Early ramp** | 8–10 | 25 | ~$7 | +25% | Budget change only. |
| | 11–13 | 30 | ~$8 | +20% | Budget change only. |
| | 14–16 | 37 | ~$10 | +23% | You may add **1** new ad (a creative from the reserve) if one has clearly failed. |
| **3 – Building** | 17–19 | 45 | ~$12 | +22% | Budget change only. |
| | 20–22 | 55 | ~$15 | +22% | You may add 1 new ad. |
| | 23–25 | 68 | ~$18 | +24% | Budget change only. |
| | 26–28 | 82 | ~$22 | +21% | You may pause clearly losing ads (but always keep at least 2 running). |
| **4 – Approach** | 29–31 | 100 | ~$27 | +22% | Budget change only. |
| | 32–34 | 120 | ~$32 | +20% | You may add 1 new ad. |
| **5 – Steady state** | 35+ | **150** | ~$40 | +25% | Normal operations (Section 3.7). |

**About five weeks from $5/day to 150 ILS/day, with no single change bigger than 25%.**

Notes:
- Meta may spend up to about **75% above your daily budget** on some days and makes up for it on others (it won't go over 7× your daily budget for the week). A day where 20 ILS turns into 33 ILS is normal and not a problem.
- **Change the budget once, at the start of your day** (morning, Israel time). Don't make several small changes the same day.
- **Never raise two things at once** (for example budget and a new ad on the same day).

### 3.4 Limits on creating new objects (protection against "too many ads")

These are working rules from practice. They're conservative on purpose.

| Account age | New campaigns | New ad sets | New ads | Edits to live ads |
|---|---|---|---|---|
| Week 1 | 1 (total) | 1 (total) | 2–3 (total) | 0 |
| Weeks 2–5 | 0 | 0 | max **1 per 6 days** | Budget only |
| Months 2–3 | max 1 per 2 weeks | max 1 per week | max 3 per week | Minimal |
| Month 4+ | as needed, still one at a time | max 2 per week | max 5 per week | Minimal |

Also:
- Don't bulk-duplicate campaigns or ad sets to "test".
- Don't keep turning things on and off. Pausing for more than 7 days also restarts learning.
- After any rejection, **stop creating anything for 7 days**, except a corrected replacement ad.

### 3.5 The 72-hour rule and what counts as a significant change

After any **significant change**, make no further changes for at least **72 hours**. Meta counts these as significant (they reset learning):
- Large budget changes
- Adding or replacing ads, or editing creative or copy
- Changing targeting, placements, optimization event or bid strategy
- Pausing for 7+ days

Budget steps of 20–25% are moderate. They're the only change you should make often.

### 3.6 Gates: conditions for each budget step

**Only raise the budget when every one of these is true:**
1. ✅ All charges in the last 7 days succeeded (Payment Activity).
2. ✅ No rejected ads in the last 7 days.
3. ✅ Nothing flagged in Account Quality or Business Support Home.
4. ✅ No new spending-limit warnings and no requests for ID or verification still open.
5. ✅ Performance isn't falling apart. For example, cost per add-to-cart or cost per purchase isn't more than about 2× its average so far. (At small budgets, judge trends across 3+ days, not single days.)

**If a gate fails, hold the budget for 3–7 days and fix the cause. Don't skip steps or "catch up" later.**

### 3.7 Steady state (150 ILS/day) and growing beyond it

- **Creative refresh:** add 1–2 new ads every 2–3 weeks or when frequency goes above about 2.5–3 and results drop. Keep 3–5 active ads in the ad set.
- **Testing:** test a new angle in the **same ad set** (as a new ad) instead of building new campaigns.
- **Raising spend beyond 150 ILS/day (once you're profitable):**
  - **Vertical:** +20% at most every 3–4 days, still with the gates in Section 3.6.
  - **Horizontal:** at most one new ad set per week, starting at a moderate budget (about 30–50% of the main ad set's budget).
  - When you have 3+ ad sets, think about moving to **Advantage+ campaign budget**.
- **Raise the account spending limit and confirm card headroom ahead of time** before each new spend level.
- **Coming back after a long pause** (for example 30+ days): restart at about 50% of your last budget and ramp up again in 20–25% steps.

### 3.8 Incident response

| What happens | What to do right away | What not to do |
|---|---|---|
| **Ad rejected** | Read the policy. If valid, make a compliant replacement. If wrong, request one review. Freeze new objects for 7 days. | Edit and resubmit the same ad again and again, or launch lots of ads to "test" what passes. |
| **Payment declined** | Pay now with the main or backup card. Call the bank. Hold all changes until the balance is paid. | Add several new cards, or use cards in other people's names. |
| **Ad account disabled** | Account Quality → Request review. Write a short, factual and polite appeal. Use Meta Verified support if you have it. | Open a new account, use another profile, or buy or rent an account. |
| **Suspected breach** (unknown admin, unknown ads, card changes) | Change the password, end all sessions, check 2FA, remove unknown admins, apps and partners, pause ads, contact Meta through `facebook.com/hacked` and Business Support. | Click "recovery" links in DMs or emails. |
| **ID or verification request** | Complete it promptly with your real documents. | Ignore it or upload anything that isn't genuine. |

---

## 4. Creative framework: ads that pass automated and human review

### 4.1 Core principles

1. **The product is the main subject.** The person is the context.
2. **Show, don't promise.** Demonstrate features. Don't promise outcomes.
3. **Speak from your own experience ("I") without labeling the viewer.**
4. **Every claim is checkable** (Section 4.3).
5. **The ad, the thumbnail, the video audio, the on-screen text and the landing page all say the same thing.** The system reads all of them.

### 4.2 First-person angles (with safe templates)

| Angle | Template | Why it's safe |
|---|---|---|
| **Founder story** | "I started [brand] because I couldn't find a [product] that was [specific feature]. So I designed one." | A personal statement about a verifiable product feature. |
| **Real customer experience** *(with written consent)* | "I've used mine every day for three months. What I like most is [feature]." | A description of experience, not a promise of results. |
| **Routine / in use** | "My morning routine: coffee, [product], out the door. Here's how I use it." | Shows the product in use. |
| **"Why I switched"** | "I switched from [generic alternative] because I wanted [feature: lighter / washable / no batteries]." | A comparison by feature, with no competitors named. |
| **"What I wish I knew"** | "Three things I wish I'd known before buying a [product category]…" | Educational, adds value. |
| **Honest skeptic** | "I was skeptical about the price. Here's what made it worth it for me: [materials, warranty, details]." | Fair, and the claims are concrete. |
| **Behind the scenes** | "I check every order myself before it ships. Here's what that looks like." | Builds trust and is verifiable. |

**Example primary text (general product):**
> I designed this bag after years of carrying a laptop in bags that hurt my shoulders. I added a padded strap, a separate laptop sleeve, and water-resistant fabric. I've used mine daily for a year. Free shipping in Israel, 30-day returns.

**Example (gift product):**
> I made these for my sister's birthday and ended up turning it into a business. Each one is hand-finished, packed in a gift box, and ships within 3 business days.

### 4.3 The claims ladder

| Level | Type | Examples | Rule |
|---|---|---|---|
| 🟢 **Green: use freely** | Verifiable product facts and terms | "100% cotton", "Fits a 15.6-inch laptop", "Ships in 3 business days", "30-day returns", "1-year warranty" | Keep proof on file. |
| 🟡 **Yellow: use carefully** | Personal opinion and experience | "My favorite", "Feels really soft", "The one I use every day", "Customers often tell us…" (only if true) | Must clearly read as opinion. No numbers unless you can prove them. |
| 🔴 **Red: never** | Outcomes, guarantees, health or body, sensational | "Guaranteed results", "Lose X kg", "Cures / heals / treats", "Instant", "100% effective", "Doctors hate…", "Changed my life overnight", "Only 2 left!" (if false), "#1 in Israel" (without proof) | Don't use, not in "I" form either. |

**Words to replace:**
- "Guaranteed" → "30-day return policy"
- "Best" → "My favorite"
- "Miracle / amazing results" → a concrete feature
- "Last chance!!!" → a real, dated offer ("Sale ends Sunday 23:59")

### 4.4 Language you must not use: the personal attributes trap

Don't **assert or imply anything about the viewer's** health, weight, appearance problems, finances, age, religion, ethnicity, sexual orientation, gender identity, disability, or criminal record.

| ❌ Breaks policy | ✅ Compliant alternative |
|---|---|
| "Tired of your back pain?" | "I designed this chair with lumbar support because I sit 10 hours a day." |
| "Are you overweight?" | Don't advertise around weight. Focus on product features. |
| "Struggling with money?" | "Everyday quality at a fair price. Free shipping in Israel." |
| "Hey moms over 40…" | "Made for busy mornings." *(use audience targeting, not copy, to reach a group)* |

### 4.5 Visual rules: body exposure and image safety

**People in creatives:**
- Models **fully clothed** in everyday clothes suited to the product. For swimwear or underwear, use standard catalog framing only (straight-on, neutral pose) and expect closer review. Where possible, prefer **product-only images (flat lay, mannequin)** for these categories.
- **No crops or zooms** on chest, buttocks, groin or abs. No shots from above or below aimed at the body.
- **No suggestive poses**, wet-skin looks, bed or bath scenes with implied nudity, or framing that suggests nudity.
- **No before/after**, no split screens comparing bodies, no tape measures or scales, no zoomed skin texture, and no "ideal body" imagery.
- If the product is worn on the body (jewelry, bags, clothes), **frame by the product**, not the body.

**Video:**
- **The thumbnail and first frame must be the safest frame in the video:** ideally the product itself.
- Check **every second** before uploading. A single frame can trigger rejection.
- If the audio says a claim, it counts like written text (speech-to-text).

**General:**
- On-image text short and factual. No ALL-CAPS headlines that shout.
- No fake buttons, play icons, notification dots or "Facebook" interface elements.
- No celebrity images, no news-site look, no fake endorsements.
- Use only images you own or have licensed, and photos of your **real product**.

**Formats:** 4:5 (feed), 9:16 (Stories/Reels), 1:1 (backup). Videos 15–30 seconds, subtitles on, product in the first 2 seconds.

### 4.6 Ad-to-landing-page consistency

| Element in the ad | Must also appear on the page |
|---|---|
| Price or discount | The same price and discount, valid right now |
| "Free shipping" | The same threshold and conditions |
| Product name and photos | The same product, in the variants shown |
| Feature claims | Listed in the product description |
| Return or warranty mention | A policy page that says exactly that |

### 4.7 Pre-flight checklist (do this for **every** ad before upload)

- [ ] No red-level claims (Section 4.3), in copy, on-image text **or** video audio.
- [ ] No mention of the viewer's personal attributes (Section 4.4).
- [ ] People fully clothed, no body-part crops, no suggestive poses. Thumbnail and first frame are safe.
- [ ] No before/after, no body comparisons.
- [ ] No fake UI, no Meta or Facebook names or logos, no celebrities, no fake reviews.
- [ ] Any urgency is real and dated.
- [ ] Every factual claim has proof in the claims file.
- [ ] Price, offer and claims match the landing page.
- [ ] Landing page has contact details, shipping, returns, privacy and terms.
- [ ] First-person testimonial is real and consented (or it's the founder's own voice).
- [ ] Creative and copy are your own or licensed.
- [ ] Launching it doesn't break the creation limits in Section 3.4.

---

## 5. Routine at a glance

| How often | Tasks |
|---|---|
| **Daily (5 min, morning)** | Glance at spend, delivery and comments. Reply to comments. Hide spam and abuse. **Don't change anything unless the schedule says so.** |
| **Every 3 days** | Review KPIs on 3-day trends. Make the scheduled budget step if the gates pass. Log it in the change log. |
| **Weekly** | Account Quality, Business Support Home, Payment Activity, ad feedback, check pending creatives against the pre-flight list. |
| **Monthly** | Security check (sessions, admins, apps). Page feedback score. Download invoices. Back up creatives. Customer-service quality (delivery times, complaints). |
| **Quarterly** | Re-read the Advertising Standards. Access audit. Card limit and account spending limit check. Review other traffic channels. |

---

## 6. The "never do" list

1. Never use another profile, a bought or rented account, or a new identity to get around a restriction.
2. Never launch more than 2–3 ads in the first week of a new ad account.
3. Never raise the budget by more than about 25% in one step, or more often than every 3 days, during the ramp.
4. Never let a failed charge stay unpaid, and never dispute a Meta charge with your bank.
5. Never add or remove many payment methods, or use cards in other people's names.
6. Never use SMS-only 2FA, give admin rights to freelancers, or download "ad reports" from strangers.
7. Never claim outcomes, guarantees or health benefits, not in first person either.
8. Never state or imply the viewer's personal attributes.
9. Never show body-part crops, implied nudity, suggestive poses or before/after images.
10. Never keep editing and resubmitting a rejected ad.

---

*This plan is based on Meta's published Advertising Standards and Business Help Center guidance as of late 2026, plus widely observed practice. Meta changes policies and enforcement often, so re-check the policy pages each quarter. Following this plan greatly lowers your risk. No method can guarantee an account will never be restricted, but a clean, verified, slowly scaled account with compliant creatives and satisfied customers is the strongest position any advertiser can have.*
