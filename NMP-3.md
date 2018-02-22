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

Depending on processes dicated by the methodology associated with a retired CRC,
the short-term estimation error of that retired CRC can decrease.

When the short-term estimation error of a retired CRC is reduced, then the quantity
of restricted NORI tokens transfered during the sale of that CRC will be reduced
by the same amount by lifting restriction on some of those tokens.

### Surplus CRC Creation

... todo ...

### Deficit Settlement process

... todo ...


_Below is some language we might use in writing the above:_

If a qualified audit report suggests more CO2 has been removed
and stored in the Project soils and above-ground biomass than was
previously recognized in CRCs, the Supplier can claim up to 50%
of the suggested CRC surplus, as CRC1s, which they can now exchange.

Nori will receive the remaining 50% of the surplus as unretrcited CRC1s
to self-insure against [possible future deficits](explanation).

If/when a Supplier instructs Nori to transfer CRC1s to a Buyer's account,
the CRC1s will be immediately retired and an equivalent number of NORI
tokens will be deposited in the Supplier's Unrestricted token account.

If the qualified audit report suggests less CO2 was removed and stored than total
historical CRC claims, Nori shall reclaim and return to Nori's treasury,
NORI tokens in Supplier's related Restricted token account up to a limit
equal to the estimated over-issuance of CRCs. Any NORI tokens remaining
in the Supplier's Restricted token account will be immediately transferred
to the Supplier's Unrestricted token account.

_Note_: These are "strawdog discount
rates. We need to talk about different verification standards, what
each means in terms of estimation error/uncertainty and relate these
different verification procedures to the CRC Quality rating and
unrestricted/restricted token ratios.  I need to include other folks in such a discussion.

_Note_: Reconsider "restricted" vs "escrowed" or some similar terminology
