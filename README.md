# JetaFX Client Help Kit

Internal Edge support & sales page with copy-ready JetaFX help videos (Malayalam) and support email templates.

**Live site:** https://edgemarketingae-eng.github.io/JetaFX-Client-Help-Kit/

## What's on the page
- **Help videos:** 5 YouTube Shorts (Part 1–5), each with *Copy full message* for WhatsApp, plus one message with all 5.
- **Email templates:** Account Opening, Withdrawal, Deposit Not Credited, Negative Balance. Switch between *Client sends* and *Sales team sends*. Send to `support@jetafx.com`.

## How to edit
Everything is in `index.html`. Edit on GitHub (pencil icon) and commit. The live site updates in about a minute.

| To change | Look for in `index.html` |
|---|---|
| Support email address | `const SUPPORT_EMAIL=` |
| Add / change a video | `const VIDEOS=[` (one line per video: `tag`, `ml` title, `en` subtitle, `short`, `url`, `when` chips) |
| WhatsApp video message wording | `const vidMsg=` and `const seriesMsg=` |
| Email template wording | `const T=[` (`client:` and `sales:` text for each issue) |
| Email greeting / sign-off | `const OPEN=` and `const SIGN=` |

Placeholders in `{curly}` braces (e.g. `{name}`, `{id}`, `{amount}`) become the `[brackets]` the client fills in, or the value typed into *Fill in details*.

New video: copy one line in `VIDEOS`, change the text and link. A new card and top button appear automatically.
