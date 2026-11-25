# MarketplaceTools Privacy Policy

- **Effective date:** November 25, 2026
- **Last updated:** November 25, 2026
- **Applies to:** MarketplaceTools for Google Chrome

## At a glance

- **Local-first analysis:** MarketplaceTools analyzes product listings locally in your browser. The
  analysis itself does not send listing data to us. (Section 2)
- **Secure account sign-in:** Sign-in is handled by our authentication provider, Supabase. We
  never store your password. (Section 4)
- **Cloud synchronization:** When you are signed in, your target keywords and Action Plan progress
  can be synchronized to your account, per product. No listing text is uploaded. (Section 5)
- **AI only when requested:** Listing text is sent for AI processing only when you ask
  MarketplaceTools to generate improvements, and only the text sections that are needed.
  (Section 6)
- **Limited usage records:** For AI requests, we record the model, the amount of text processed
  and the outcome, not the listing content itself. (Section 7)
- **No sale or advertising use:** We do not sell user information or use it for advertising.
  (Section 12)

## 1. Introduction

MarketplaceTools is a Chrome extension that helps marketplace sellers analyze and improve their
product listings. When you view a product page on a supported marketplace, MarketplaceTools reads
the listing, checks it against listing-quality guidelines, and shows the results and improvement
suggestions in Chrome's side panel. The currently supported marketplace is OTTO (otto.de).
MarketplaceTools may support additional marketplaces in future releases.

MarketplaceTools is provided by Dudes6Partner - Willi Deubner ("we", "us", "our"). MarketplaceTools is an
independent tool. It is not affiliated with, operated by or endorsed by OTTO or any other
marketplace.

This policy explains what information MarketplaceTools handles, where that information is kept, who
receives it, and what we do, and do not do, with it.

> **In short:** The listing analysis runs locally in your browser. If you sign in, we process your
> account data to provide account features, and your target keywords and Action Plan progress can be
> synchronized to your account. If you ask for AI suggestions, the listing text needed for them is
> sent through our server to our AI provider. Analytics and advertising trackers are not used, and
> we do not sell your data.

## 2. Information MarketplaceTools accesses

### Product pages on supported marketplaces

MarketplaceTools works only on product pages of supported marketplaces, which is currently OTTO
(otto.de). When you view a product page there, MarketplaceTools reads the listing information
shown on that page:

- page address, product ID and variant ID
- title, brand, category and breadcrumb navigation
- current price and comparison (crossed-out) price
- Bulletpoints, Besondere Merkmale and product description
- image addresses and image descriptions (alt text), and the number of videos
- average rating and number of reviews (not the review texts or reviewer names)
- delivery information and availability
- test seals and sustainability seals (labels and image addresses)
- Rich Content text and image addresses

MarketplaceTools uses this information to analyze the listing and to provide its features.

> Reading and analyzing this information happens locally in your browser. It does not mean the
> information is sent anywhere. Only cloud synchronization (section 5) and AI suggestions
> (section 6) send selected information, as described there.

MarketplaceTools does not read your marketplace account, login details, passwords, cookies or
payment information, and it does not change marketplace pages.

### Other websites

MarketplaceTools does not run on other websites and does not read their content. Chrome lets
MarketplaceTools see the address of a browser tab only when that tab shows a supported marketplace;
for other websites, it does not see the address at all (see section 9). MarketplaceTools does not
collect your browsing history and does not keep a record of the websites you visit.

### Information you enter

You can enter or add information yourself:

- target keywords for a product
- your Action Plan progress (which recommendations you selected and marked as done)
- competitor products you add, with your own notes and tags
- search positions (rank tracking) that you record by hand or import from a CSV or JSON file you
  choose
- your email address and password when you sign in (section 4)

Files you import are read locally and are not uploaded.

## 3. Information stored on your device

MarketplaceTools saves your work in your browser's storage on your device, so it is still there
when you close and reopen the side panel. This data is not synchronized through your Google
account. Most of it stays only on your device; the table shows which information is also
synchronized to your account (section 5).

| What is stored | Also synchronized to your account? | How long it stays on your device |
| --- | --- | --- |
| **Analysis results and saved product workspace** for each product you analyze (up to the 25 most recently used products): the analysis results (score, rule results and short facts such as "5 images", "24 characters", the delivery text, the rating and review count), the previous analysis for comparison, and view settings. Full listing texts and page HTML are not stored here. | No | Until you clear it or remove the extension. When you work on more than 25 products, the oldest workspace is removed automatically. |
| **Target keywords and Action Plan progress** (selection and done marks), saved with the product workspace | Yes, when you are signed in (section 5) | Until you clear the workspace or remove the extension |
| **Competitor data** you add: the competitor product's page address, product and variant ID and name, the listing information captured from its page (the same kinds of information listed in section 2; only the most recent capture is kept), and your notes and tags | No | Until you remove the competitor, clear the competitor data, or remove the extension |
| **Rank-tracking data** you record: tracked products (page address, product ID, name), keywords and the search positions you entered or imported (up to 100 recent entries per keyword) | No | Until you remove the keyword, clear the rank data, or remove the extension |
| **Guided-tour settings** (whether the tour is suggested and when it last ended) | No | Until you remove the extension |
| **Language preference** (German or English), stored in the side panel's local storage | No | Until you change it, clear your browsing data, or remove the extension |
| **Scroll position** of the side panel per browser tab, stored in the side panel's session storage | No | Deleted at the latest when you close the browser |
| **Sign-in session**, while you are signed in: an access token, a refresh token, your user ID and email address | No (issued and renewed by Supabase, section 4) | Until you sign out or the session expires |
| **Synchronization status**: which account this browser's saved workspaces belong to, and which changes are still to be uploaded | No | Until you clear all saved workspaces or remove the extension |

Except for the language preference and the scroll position, this information is stored in Chrome
extension storage (`chrome.storage.local`).

Some information is held only temporarily in memory while the extension is running and is never
saved: the current page analysis, keyword-research results, AI suggestions (section 6), the
temporary session used while you reset your password (section 4), and the address of the
supported marketplace page open in each tab.

## 4. Account and authentication data

You can use the listing analysis without an account. Signing in is needed for cloud
synchronization and AI suggestions. Accounts are created by MarketplaceTools; you cannot sign up
inside the extension.

When you sign in, the extension sends your **email address and password** to our authentication
provider, **Supabase**, which checks them. MarketplaceTools does not store your password; Supabase
stores only a protected (hashed) form of it. As part of providing its service, Supabase also
processes technical information such as your IP address.

After you sign in, Supabase issues a **session**. The extension stores it in your browser's
storage and renews it automatically, so you stay signed in after closing the side panel or
restarting Chrome. If the session can no longer be renewed, you are signed out and asked to sign in
again.

**Resetting your password:** if you forget your password, you can ask for a recovery code on the
sign-in form. Supabase sends the code to your email address. You enter the code and a new password
in the extension, and Supabase stores the new password in protected (hashed) form. The temporary
session used for the reset is kept only in memory and is not saved. After the reset, all sessions of
your account are signed out, and you sign in again with the new password.

**Signing out** ends the session in this browser and removes it from your browser's storage. Your
local work stays on your device, and your synchronized data stays in your account.

For each account, we keep:

- the **account record** at Supabase: your email address, user ID, and when the account was
  created and last used
- an **access profile**: your user ID, your access level, and when the profile was created and
  changed

We use this information to sign you in and to decide which features your account may use. Access
levels are set by MarketplaceTools.

## 5. Cloud synchronization

When you are signed in and your account has access to cloud synchronization, MarketplaceTools keeps
a copy of part of your saved work in your account, so that you can use it on other devices. For
each product that has a product ID, only the following is stored:

- the marketplace and the marketplace's product ID
- your target keywords, and whether they were checked
- your Action Plan selection and the recommendations you marked as done (with the time you marked
  them)
- when you last changed this data

**Not synchronized:** listing texts (title, Bulletpoints, Besondere Merkmale, description, Rich
Content), prices, images and image addresses, page addresses, analysis results, view settings,
competitor data and rank-tracking data. These stay on your device.

The synchronized copy is stored with Supabase and linked to your user ID. Database rules ensure that
each account can access only its own synchronized data, and only while the account has access.

Your browser's copy is the working copy:

- Changes are uploaded shortly after you make them.
- The synchronized copy is downloaded when you open a product.
- If the same product was changed on two devices, the most recent change is kept.
- The first account that synchronizes in a browser is linked to that browser's saved workspaces. If
  another account signs in on the same browser, those workspaces are not uploaded to it or
  downloaded from it.

**Deleting synchronized data:** if you clear a saved workspace while signed in, its synchronized
copy is deleted as well. A deletion marker is kept so that your other devices also remove the
workspace. It contains only the marketplace, the product ID and the time of deletion, not your
keywords or Action Plan.

## 6. AI processing

MarketplaceTools can suggest improved listing text using an AI model. This happens **only when you
explicitly request it**: you must be signed in, your account must have access, and you must ask
MarketplaceTools to generate suggestions.

When you request an AI-generated improvement, the extension sends the following to the
**MarketplaceTools server**, together with your sign-in token:

- the listing's title, Bulletpoints, Besondere Merkmale and description
- Rich Content teaser headline, teaser text and footnote
- brand, category and breadcrumb navigation
- your target keywords, with their status and priority
- which sections should be improved, the improvement goals, length limits and the language
- a random request number, used to match the answer to the request

**Not sent:** the page address, product and variant ID, prices, images and image addresses,
rating, review count, delivery information, availability, number of videos, seals, Rich Content
images and highlight blocks.

The MarketplaceTools server checks your sign-in and access level and applies usage limits
(section 7). It then sends the listing information and keywords to our AI provider, **Anthropic**
(Claude), to generate the suggestions. Anthropic does not receive your email address, user ID,
sign-in token or IP address from us. Anthropic processes this information to provide the service,
according to the applicable service agreement and its privacy terms. The extension never contacts
Anthropic directly.

The suggestions are returned through the MarketplaceTools server to your browser. Our server does
not store the listing text, the request sent to Anthropic, or the suggestions. In the extension,
the suggestions are kept only in memory while the side panel is open. You decide whether to copy
them; you can also save them as a file on your device.

## 7. AI usage records

For each AI request, the MarketplaceTools server records:

- your user ID
- the time of the request
- the AI model used
- the amount of text processed (input and output tokens)
- the outcome (for example: success, timeout, or no usable result)

The server stores these records in our database at Supabase, in an area that the extension and
user accounts cannot access.

These records contain **no** listing text, keywords, prompts, AI suggestions, email address or IP
address. We use them to apply fair-use limits per minute and per day, and to manage costs. Our
server's error logs record only the type of event (for example "rate limited"), not user IDs or
content.

Retention periods for these records are determined by MarketplaceTools' operational requirements
and applicable legal obligations.

## 8. Analytics, cookies and tracking

MarketplaceTools does not use analytics, telemetry, crash reporting, advertising trackers,
advertising identifiers or any other tracking tools. The extension does not set cookies.

## 9. Chrome permissions

When you install MarketplaceTools, Chrome asks for the following permissions. Chrome's warnings
describe what a permission *could* allow; this table explains what MarketplaceTools actually does.

| Permission | Why MarketplaceTools needs it | What MarketplaceTools does with it |
| --- | --- | --- |
| **Access to supported marketplaces** (`https://www.otto.de/*`, `https://otto.de/*`) | To read the product page you view. Chrome describes this as being able to "read and change" your data on these sites. | Reads the product information listed in section 2 and processes it locally. This access also lets MarketplaceTools see the address of tabs that show a supported marketplace, so the side panel can show the analysis for the page you are looking at. It does not change marketplace pages and does not run on any other website. |
| **`storage`** | To save your work and your sign-in session on your device (see section 3). | Stores your workspaces, competitor data, rank-tracking data, settings and sign-in session locally. Nothing is synchronized through your Google account. |
| **`sidePanel`** | To show the MarketplaceTools interface in Chrome's side panel next to the product page. | Displays the analysis and tools. |

MarketplaceTools does not request Chrome's `tabs`, browsing history, cookies, bookmarks, downloads
or location permissions, and it does not load code from the internet; all of its code is part of
the installed extension. Sign-in, cloud synchronization and AI suggestions do not need any
additional Chrome permission.

When support for another marketplace is added, Chrome will ask for access to that marketplace's
website, and we will update this policy.

## 10. Network requests

### Listing analysis

MarketplaceTools does not send listing data to us for the analysis. To show the product's main image
in the side panel, your browser loads it directly from the marketplace's servers (currently OTTO),
the same image you see on the product page. As with any image your browser loads, the marketplace
receives the usual technical information (such as your IP address) with that request.

### Sign-in and cloud synchronization

When you sign in, the extension connects to Supabase to sign you in and to renew your session. If
you reset your password, it connects to Supabase to request the recovery code and to set the new
password.
While you are signed in, it also connects to Supabase to upload and download the synchronized data
described in section 5.

### AI suggestions

Only when you request AI suggestions, the extension connects to the MarketplaceTools server, which
connects to Anthropic as described in section 6. The extension never connects to Anthropic
directly.

All of these connections are encrypted (HTTPS). Without signing in, MarketplaceTools sends no data
to us, to Supabase or to Anthropic.

### This privacy-policy web page

The web page that shows this policy loads its layout styles (Bootstrap) from cdn.jsdelivr.net and
its icons (Font Awesome) from cdnjs.cloudflare.com. When you open the page, your browser connects to
those servers, which receive the usual technical information such as your IP address. The page
itself sets no cookies and uses no analytics. This concerns only the web page, not the
MarketplaceTools extension.

## 11. Third-party services

| Service | Role | When it is used |
| --- | --- | --- |
| **Supabase** | Authentication and the database for accounts and cloud synchronization, acting on our behalf. Receives your email address, the password check, your session, user ID and access level, and the synchronized data described in section 5. Sends password-recovery codes by email. Also stores the AI usage records described in section 7. | When you sign in, while you are signed in, when you reset your password, and when you request AI suggestions |
| **MarketplaceTools server** | Our server, operated with a hosting provider acting on our behalf. Processes the AI request described in section 6, applies usage limits and writes the usage records described in section 7. As with any server connection, the hosting provider processes technical connection data such as your IP address. | When you request AI suggestions |
| **Anthropic** | AI model provider (Claude), acting on our behalf. Receives the listing text sections and keywords described in section 6. | When you request AI suggestions |
| **OTTO (otto.de)** | The marketplace whose product pages MarketplaceTools reads. The product image shown in the side panel is loaded from OTTO's servers. We do not share any data with OTTO, and OTTO is not a partner of MarketplaceTools. | When you analyze an OTTO product page |
| **Google Chrome Web Store** | Distributes the extension. Installing and updating extensions is handled by Google under Google's own privacy policy. | Installation and updates |

## 12. Data sharing

- **Listing analysis:** runs in your browser. No listing content is sent to us.
- **Cloud synchronization:** only the selected workspace information described in section 5 is
  stored in your account.
- **AI suggestions:** only the listing content described in section 6 is sent, and only when you
  request AI suggestions.
- **Usage records:** limited information about each AI request is recorded to manage AI usage
  (section 7).

We share information only with the service providers listed in section 11, and only as needed to
provide MarketplaceTools. We do not:

- sell or rent personal information or other user data
- share user data for advertising
- show targeted advertising
- track you across websites
- use advertising cookies
- collect your browsing history
- use data to determine creditworthiness or for lending

If you contact us (see section 20), we use your message only to answer your request.

## 13. Limited Use

MarketplaceTools' use of information it handles, including the marketplace website content it
reads, complies with the Chrome Web Store User Data Policy, including the Limited Use requirements.
MarketplaceTools uses this information only to provide the features described in this policy:
analyzing product listings, synchronizing your keywords and Action Plan, and generating listing
suggestions when you request them. It transfers information only to the service providers named in
section 11, and only to provide these features. It does not use the information for advertising or
to determine creditworthiness or for lending purposes. Our server does not store your listing text,
so no one at MarketplaceTools reads it.

## 14. Data retention and deletion

**Data on your device** stays there until you delete it or remove the extension.

**Delete it in MarketplaceTools.** Under **More** (German: **Mehr**), you can delete your saved
data at any time. It is removed from your browser's storage straight away.

- **Saved workspace** → **Clear saved workspace** (one product) or **Clear all saved OTTO
  workspaces** (German: *Gespeicherten Arbeitsstand löschen* / *Alle gespeicherten
  OTTO-Arbeitsstände löschen*)
- **Competitor Intelligence** → **Remove** (one competitor) or **Clear Competitor Data**
  (German: *Entfernen* / *Wettbewerber-Daten löschen*)
- **Rank Tracking** → **Remove** (one keyword, with its recorded positions) or **Clear Rank Data**
  (German: *Entfernen* / *Ranking-Daten löschen*)

**Remove the extension.** When you remove MarketplaceTools from Chrome (for example on the
`chrome://extensions` page), Chrome deletes all data that MarketplaceTools stored in your browser.
This includes the guided-tour and language settings, which cannot be deleted separately inside the
extension.

**Clearing Chrome's browsing data** (history, cache, cookies) does **not** delete your saved
MarketplaceTools work. It may reset the language setting.

**Sign-in session:** signing out removes your session from your browser.

**Synchronized data:** clearing a saved workspace while signed in also deletes its synchronized copy
(section 5). Synchronized data is otherwise kept as long as your account exists. Deletion markers
are kept so that your other devices also remove deleted workspaces.

**Account data:** you may request deletion of your MarketplaceTools account and the associated cloud
data by contacting us using the privacy contact in section 20.

**AI usage records:** these records are deleted when your account is deleted. Otherwise, retention
periods for these records are determined by MarketplaceTools' operational requirements and
applicable legal obligations. You can contact us about these records
(section 16).

**AI requests and suggestions** are not stored on our server.

**Messages you send us** are kept only as long as needed to handle your request and to meet legal
retention obligations.

## 15. Data security

- Data used only for the local analysis stays in your browser and is not transmitted.
- The extension's storage is restricted to the extension's own pages, and the part of the extension
  that runs on marketplace pages does not read or write it.
- The extension loads no code from the internet, and imported files are processed locally.
- Connections to Supabase and to the MarketplaceTools server are encrypted (HTTPS).
- Database rules allow each account to access only its own synchronized data.
- Our server accepts AI requests only from the MarketplaceTools extension and only with a valid
  sign-in from an account with access, and it applies usage limits. Provider credentials, such as
  the AI provider's key, are kept on our server, never in the extension.

Data saved in your browser is protected by your device and your Chrome profile. Anyone with access
to your computer and Chrome profile may be able to see it. No method of transmission or storage is
completely secure, so we cannot guarantee absolute security.

## 16. Your choices and rights

- You can use the listing analysis without an account.
- You decide whether to sign in and whether to request AI suggestions.
- You can delete your local data, sign out, and clear synchronized workspaces at any time
  (section 14).
- You can remove the extension at any time, which deletes its local data.

If data protection law such as the EU General Data Protection Regulation (GDPR) applies, you have
the right to request access to, correction of, or deletion of your personal data, to request
restriction of processing, to object to processing, and to data portability, where the legal
requirements are met. These rights apply to your account data, your synchronized data and your AI
usage records. You also have the right to lodge a complaint with a data protection supervisory
authority. To make a request, contact us (section 20).

Data used only for the local analysis stays in your browser, so we do not hold it.

## 17. Children's privacy

MarketplaceTools is a tool for business and professional marketplace sellers. It is not directed at
children, and we do not knowingly collect information from children.

## 18. International data processing

When you sign in, use cloud synchronization or request AI suggestions, some of our service providers
may process information outside the European Union or the European Economic Area. Anthropic, for
example, is based in the United States. Where this happens, we take the steps required by
applicable data protection law to protect your information.

## 19. Changes to this policy

We may update this policy as MarketplaceTools changes, for example when we add features or support
for another marketplace. Whenever a version of MarketplaceTools materially changes how it handles
information, for example what information it collects, what is sent off your device, to whom or
why, we will update this policy before that version is released. The "Last updated" date at the top
shows when this policy last changed.

## 20. Contact

For privacy questions or requests, please contact:

- **Company:** Dudes6Partner - Willi Deubner
- **Postal address:** Hauptmarkt 6, 99867 Gotha, Germany
- **Email:** info@dudes-partner.com
- **Website:** https://dudes-partner.com

We have not appointed a data protection officer. Please send privacy questions and requests to the
email address above.
