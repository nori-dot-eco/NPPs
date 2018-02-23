CoderPad + Markdown
===================

Welcome to a real-time collaborative [Markdown][1] editor.

In addition to all the usual Markdown features, it uses
[Github-Flavored Markdown][2], except with breaks on newlines
disabled.

Arbitrary HTML input is disabled, for obvious security reasons,
and "smart" quotes are enabled.

We also support code fencing, through either backticks or
indentation.

```javascript
function hello() {
  var s = "Hi there!";
  console.log(s);
}
```

[1]: http://daringfireball.net/projects/markdown/
[2]: https://help.github.com/articles/github-flavored-markdown



Your previous Plain Text content is preserved below:

## Preamble

  NMP: NMP-3

  Title: Carbon Removal Claims (CRCs) for Agricultural Soils (Croplands, Grazing and Rangelands) 

  Extended Title: Soil Methodologies: Validating CRC Listings And Removing Restrictions On NORI token transfers

  Author: Aldyen Donnelly

  Type: Methodology

  Categroy: Carbon Removal

  Status: Draft

  Created: February 22, 2018

  Replaces: N/A



### Summary

This methodology outlines a historical Carbon Removal Claim audit process.
The intended result is to cause the transfer of NORI tokens from a restricted
to an unrestricted account.

### Motivation
... briefly describe why this nmp is needed ...


### The Historical CRC Creation Claim Audit Process

At least once each 10 year Project term, but not earlier than the
6th anniversary of the Original Project Registration date, the Supplier
shall commission a Historical CRC Audit Report.

The audit report must be completed by a Nori Whitelisted Validator.
Entities that provide verification services may also act as validators,
but may not act as validators for a Project/CRC stream for which they acted
as CRC claim verifiers.

_Note_: Others might suggest no earlier than year 7 or 8.

_Note_: funding for the audit report will be covered elsewhere

_Note_: Verification is for the more frequent "in progress" measurement
and maintenance of the project, Auditing is the "final" measurement
of project output.

### The Audit Report

The Audit report shall include a whitelisted third party estimate of the volume of CO2:

  * removed from the atmosphere

  * retained in the soil

These measurements will be taken from within:

  * the Project's boundaries

  * the [Project's timeline](NMP-???) <-- Jaycen: requisite definition in every nmp <type: project>


_Note_: Need to talk about timing and who pays for verification and auditing
Methods.  I have a bunch of ideas, but these need
discussion before finalizing.  Needs Discussion, first among
Norinauts and then with others.

### Impact of Audit on historical Carbon Removal Claims

A qualified audit report will reveal three potential scenarios:

1. a surplus of CO2 relative to historical data was removed and stored

   * this will trigger [additional CRC1 creation](NIP-???).

2. a deficit of CO2 relative to historical data was removed and stored

   * this will trigger [deficit settlement](NIP-???).
   
3. neither a surplus nor a deficit of CO2 relative to historical data
   was removed and stored
   
   * this will trigger [project phase closure](NIP-???)


# NIP-??

## Preamble

  NIP: NIP-???

  Title: CRC and NORI token transfers for multi-tiered CRCs

  Author: Aldyen Donnelly

  Type: Standard Track

  Categroy: Core

  Status: Draft

  Created: February 22, 2018

  Replaces: N/A


### Initial Tiered CRC and NORI token transfer

NORI tokens may be restricted or unrestricted.

 * _unrestricted tokens_ can be exchanged for other currencies (fiat, crypto, etc.)
 
 * _restricted tokens_ can not be exchanged for other currencies.

Tiered CRCs have an associated rating equal to the short-term estimation error
of the model used to measure the ongoing carbon removal and storage.

For example, a CRC with a short-term estimation error of 40% with be a lower tier
than a CRC with a short-term estimation error of 20%.

Depending on the short-term estimation error of a CRC, an exchange of NORI
tokens for that CRC will result in a share of the NORI tokens being restricted.

The share of restricted tokens will equal the short-term estimation error.

Restricted tokens can be transitioned to unrestricted status. This process
is covered in the sections below.

### Incremental lifting of restrictions

Depending on processes dictated by the methodology associated with a retired CRC,
the short-term estimation error of that retired CRC can decrease.

When the short-term estimation error of a retired CRC is reduced, then the quantity
of restricted NORI tokens transfered during the sale of that CRC will be reduced
by the same amount by lifting restriction on some of those tokens.

For example, when 100 NORI tokens are exchanged for 100 CRCs with a +/- 40% short-term
estimation error, 40 of those NORI tokens will be restricted upon deliver to the
supplier. If after auditing, or some other process, that estimation error is reduced
10%, the restriction will be lifted on 30 of the NORI tokens.

_Note_: It's possible that the lowest acheivable estimation error will be greater
than +/- 0%, and we need to make sure that aspect is communicated.

### Surplus CRC Creation

In the event that final auditing indicates that more CO2 was removed and stored
than was reflected in the historical CRC generation, then additional CRCs will
be created.

These surplus CRCs will be tier-1 rated, and will be immediately tradeable.

These surplus CRCs will be split between the original supplier and
the [market risk mitigation account](section-???).

_Note_: The exact amount that is split between supplier and market risk
mitigation account still needs to be determined and may be dependent
on market dynamics, methodology, specific projects, etc.

_Note_: One way to calculate the split between supplier and mitigation account
is based on the size of the mitigation account. As it gets bigger, the
suppliers of a surplus retain more of the surplus.

### Deficit Settlement process

In the event that final auditing indicates that _less_ CO2 was removed and stored
than was reflected in the historical CRC generation, then the remaining restricted
NORI tokens will be used to purchase and retire additional CRCs.

If there are not enough remaining NORI tokens to cover the deficit, then
additional CRCs from the [market risk mitigation account](section-???) will
be retired to coer the rest.

_Note_: The only time the purchase of a CRC does not result in that CRC
being retired is when the purchase is performed by the market risk mitigation
account.

For example:

100 CRCs
--> 60 unrestricted NORI, 40 restricted NORI
--> audit says only 70 TCO2e were done (30 CRC deficit)
--> 70 unrestricted NORI, 30 restricted NORI
--> 30 restricted NORI used to retire 30 additional CRCs to cover the deficit

100 CRCs
--> 60 unrestricted NORI, 40 restricted NORI
--> audit says only 50 TCO2e were done (50 CRC deficit)
--> remaining 40 restricted NORI used to retire 40 additional CRCs to cover the deficit
--> additional 10 CRCs retired from the risk mitigation account

_Note_: These are "strawdog discount
rates. We need to talk about different verification standards, what
each means in terms of estimation error/uncertainty and relate these
different verification procedures to the CRC Quality rating and
unrestricted/restricted token ratios.  I need to include other folks in such a discussion.

_Note_: Reconsider "restricted" vs "escrowed" or some similar terminology
