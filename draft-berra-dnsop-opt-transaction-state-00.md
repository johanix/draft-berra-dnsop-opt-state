---
title: "Automating DNS Delegation Management via DDNS"
abbrev: DDNS Updates of Delegation Information
docname: draft-johani-dnsop-delegation-mgmt-via-ddns-03
date: {DATE}
category: std

ipr: trust200902
area: Internet
workgroup: DNSOP Working Group
keyword: Internet-Draft

stand_alone: yes
pi: [toc, sortrefs, symrefs]

author:
 -
    ins: J. Stenstam
    name: Johan Stenstam
    organization: The Swedish Internet Foundation
    country: Sweden
    email: johan.stenstam@internetstiftelsen.se

normative:

informative:

--- abstract

...

This document proposes such a mechanism.

TO BE REMOVED: This document is being collaborated on in Github at:
[https://github.com/johanix/draft-berra-dnsop-opt-transaction-state](https://github.com/johanix/draft-johani-dnsop-delegation-mgmt-via-ddns).
The most recent working version of the document, open issues, etc, should all be
available there.  The author (gratefully) accept pull requests.

--- middle

# Introduction

...

Knowledge of DNS NOTIFY {{!RFC1996}} and DNS Dynamic Updates
{{!RFC2136}} and {{!RFC3007}} is assumed. DNS SIG(0) transaction
signatures are documented in {{!RFC2931}}. In addition this
Internet-Draft borrows heavily from the thoughts and problem statement
from the Internet-Draft on Generalized DNS Notifications (work in progress).

## Requirements Notation

The key words "**MUST**", "**MUST NOT**", "**REQUIRED**", "**SHALL**",
"**SHALL NOT**", "**SHOULD**", "**SHOULD NOT**", "**RECOMMENDED**",
"**NOT RECOMMENDED**", "**MAY**", and "**OPTIONAL**" in this document
are to be interpreted as described in BCP 14 {{!RFC2119}} {{!RFC8174}}
when, and only when, they appear in all capitals, as shown here.

# Use Cases

...

## Synchronization of SIG(0) Key State Between Child and Parent  
 
...

## Synchronization of State Between Signers in Distributed Multi-Signer
 
...

# Terminology

SIG(0)
: An assymmetric signing algorithm that allows the recipient to only
  need to know the public key to verify a signature created by the
  senders private key.

# Comparision With Extended DNS Error Codes

...

# Security Considerations.

...

# IANA Considerations.

IANA is requested to assign a new "scheme" value to the registry for
"DSYNC Location of Synchronization Endpoints" as follows:

Reference
: (this document)

| RRtype | Scheme | Purpose               | Reference       |
| ------ | ------ | --------------------- | --------------- |
| ANY    |      2 | Delegation management | (this document) |

-------

# Acknowledgements.

...

--- back

# Change History (to be removed before publication)

* draft-berra-dnsop-opt-transaction-state-00

> Initial public draft.
