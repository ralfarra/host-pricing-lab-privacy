# Pricing Lab — Privacy Policy

Effective date: September 28, 2026 · Applies to extension version 1.14.1 and later

Pricing Lab is a Chrome extension that helps Turo hosts read the prices on their
own host calendar, calculate an explainable pricing recommendation, and apply a
price they have approved back to that calendar.

## What the extension reads

When you open the extension or press a control inside it, it may read
information visible on the Turo page you are on, including:

- the page URL and listing ID;
- vehicle year, make, model, trim and visible features;
- selected trip dates and trip length;
- the displayed trip total and derived daily average;
- included mileage and overage rate;
- pickup location, rating and trip count when visible;
- the per-day prices, booked status and custom/dynamic status shown on your own
  host calendar.

If you use the optional Compare feature, it also reads publicly listed prices of
comparable cars from Turo's own search results, and your own vehicle list so
your listing can be excluded from your own market median.

Nothing is read on a timer, on a schedule, or on any site other than turo.com.
Every read starts with something you pressed.

One thing does outlive the popup, and it is worth stating plainly: a **Compare**
run you started keeps working after you close the popup. It finishes reading
Turo's search results, saves the result for you to come back to, and marks the
toolbar icon when it is done. It stops on its own when it finishes. Nothing else
in the extension continues after the popup closes, and closing the popup never
starts anything.

## What the extension writes

Pricing Lab can change prices on your own host calendar. This is not automatic
and never happens in the background:

- every change is previewed on the page, showing the current value and the new
  value, before anything is saved;
- nothing is saved until you click Apply;
- there is no scheduled, unattended or background repricing.

## What is stored on your device

The following are stored in Chrome local extension storage on your own
computer:

- your pricing rules, floors and settings;
- up to 250 captured quote snapshots;
- your most recent calendar scan;
- a log of price changes you applied;
- your Pro license status;
- a random install identifier, which is not derived from anything personal and
  is not linked to your identity;
- any feedback message that could not be sent at the time you wrote it.

You can clear snapshot history with the Clear button, or remove all extension
data by uninstalling the extension.

## What leaves your device, and only when you choose

By default, captured page data and pricing settings stay on your device. There
are four optional features that transmit data, each only when you actively use
it:

**1. The Pro AI pricing assistant.** When you submit a question, the extension
sends that question plus a compact summary of your own captured pricing,
calendar and competitor data to our proxy server at
`host-pricing-lab-proxy.vercel.app`. The proxy relays it to our AI provider,
Anthropic, and returns a text answer. If you never open the assistant, this
never happens.

**2. The Feedback tab.** When you write a bug report or feature request and
press Send, the extension sends:

- the message you typed;
- an optional reply email, if you choose to enter one — it can be left blank
  and the report will still send;
- a short list of non-identifying diagnostics: the extension version, whether
  you are on the free or Pro plan, a coarse page category such as "host
  calendar", the number of days in your last scan, and the number of saved
  snapshots;
- **only if you tick the off-by-default "Attach my last calendar scan" box:**
  the dates in your current pricing window, the price on each day, your own
  floor for each day, and whether each day is booked or below your floor.

The panel shows a "What gets sent" list generated from the actual data being
sent, so it always matches the payload.

**3. The founder check-in.** The welcome page and, once, the popup offer an
optional email box: "Want a hand setting your prices?" If you type your email
and press Email me, the extension sends your email, a random install id, where
you signed up (welcome page or popup), whether you're on Free or Pro, and the
extension version. Nothing from your Turo calendar is included. We use that
email only to write to you personally about Pricing Lab: a check-in a couple of
days later, and an occasional note about Pro while you're on the free plan.
Reply "stop" (or email turopricinglab@gmail.com) and we won't email you again.
An email you type into the Feedback tab is never added to this list; it is used
only to reply to that report.

**4. Billing.** If you choose to upgrade to Pro, the extension contacts
ExtensionPay (`extensionpay.com`), our third-party billing provider, to open
checkout and verify license status. Payment is processed by Stripe through
ExtensionPay. We never see or store your card details. No Turo page data or
pricing settings are sent to ExtensionPay.

## What is never transmitted

- Your Turo password. The extension never requests or stores it.
- Cookies, session tokens or authentication credentials.
- Your general browsing history.
- Your full Turo URL. Before any feedback leaves your device the URL is reduced
  to a coarse category such as "host calendar" or "search results", because a
  Turo URL contains a vehicle identifier.
- Which vehicle a report relates to, your name, or anything from your Turo
  account.
- Payment card details.
- Screenshots or images. The extension has no ability to capture your screen.

## Retention

Feedback reports, including any optional email and any attached calendar scan,
are retained for up to 400 days and then deleted automatically. Check-in
signups are retained for up to 400 days, or until you ask us to remove you.
AI assistant questions are not retained after the answer is returned; only an anonymous
per-install spend counter is kept, so the monthly usage cap can be enforced.

## Sharing

We do not sell, rent, or trade any of this information. We do not use it for
advertising, profiling, or credit-related decisions. It is shared only with the
service providers named above — Anthropic for the AI assistant, and
ExtensionPay and Stripe for billing — and only for the purpose described.

## Your choices

- The Feedback email field is optional; leave it blank to report anonymously.
- The check-in email box is optional and sends nothing unless you fill it in.
  To be removed, reply "stop" to any email or write to
  turopricinglab@gmail.com.
- The calendar-scan attachment is off by default and must be ticked each time.
- The AI assistant is optional and only runs when you submit a question.
- To have a feedback report deleted before its retention period ends, email
  turopricinglab@gmail.com with the report id shown when you sent it.

## Security

The extension requests only the permissions required for its single purpose.
All executable code is packaged with the extension; no remote code is loaded or
evaluated.

## Children

Pricing Lab is intended for adult vehicle hosts and is not directed to
children.

## Changes

Material changes to this policy will be published here alongside an updated
extension release, with a new effective date.

## Contact

turopricinglab@gmail.com

Or open an issue at
https://github.com/ralfarra/host-pricing-lab-privacy/issues

## Trademark disclaimer

Pricing Lab is an independent project and is not affiliated with, endorsed by,
or sponsored by Turo. "Turo" is used descriptively to identify the marketplace
the extension supports.
