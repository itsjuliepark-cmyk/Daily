# Connecting School Outlook Without Signing In Every Time

School accounts (Microsoft 365) usually have external app connections blocked by school IT.
That is why Claude's Microsoft 365 connector often gets stuck on "Admin approval required".
**We do not store the school password in the bot** (it would not work because of MFA, and it could violate school policy).

## Option A (recommended): auto-forward Outlook to Gmail

Set it up once and school email keeps getting copied to Gmail, so the bot only needs to look at Gmail. No sign-in expiry.

1. In Outlook on the web, click **⚙️ Settings** at the top right
2. **Mail → Forwarding**
3. Check **Enable forwarding**
4. Forward to: my Gmail address
5. Check **Keep a copy of forwarded messages** ← important!
6. Save

Then create a filter in Gmail:
- Filter icon next to the search bar → **To**: `@school-domain` (e.g. `@school.edu`)
- **Create filter** → **Apply the label: `School`** (+ "Skip the Inbox" if you want)

> If forwarding does not work and you get a bounce such as `550 5.7.520 Access denied, your organization does not allow external forwarding`,
> the school has blocked external forwarding. Use Option B or C.

## Option B: reconnect the Microsoft 365 connector

https://claude.ai/customize/connectors → Microsoft 365 → Reconnect.
If an "Admin approval required" screen appears, it is blocked by school IT policy.
Note: this connector is **search and read-only** for mail, so even when connected, labels and replies are only possible on the Gmail side.

## Option C: use the browser session (only while the computer is on)

With the Claude desktop app plus the Claude in Chrome extension, Claude can read an Outlook tab that is already signed in.
However, this only works while the computer is on and the browser stays signed in, so for a "run automatically every morning" setup, Option A is much more reliable.
