# Responsible Disclosure Methodology

## Principle

Every channel was used simultaneously and in good faith. The goal at every
stage was to give Meta the information needed to understand and remediate
the vulnerability, while building a complete record for accountability if
they did not.

The posture throughout: researcher, not complainant.

---

## Discovery

The `__d=` attack URL was discovered on 28 May 2026 through post-filing
OSINT — a Google search referencing the @darkwolf.india account handle
immediately after the IT Rules 2021 grievance was filed.

**Discovery methodology:**
1. Search for victim account handle in Google
2. Identify anomalous URL in search results
3. Decompose URL components
4. Translate embedded Chinese content
5. Identify external domain and run threat intelligence
6. Cross-reference with account data archive forensics
7. Reconstruct attack chain

Total time from observation to complete technical analysis: under 3 hours.

---

## Disclosure Sequence

### Step 1 — Legal record first (28 May 2026)

The IT Rules 2021 grievance was filed before the attack URL was discovered.
This created the legal record before the security finding — ensuring that
the disclosure was grounded in a documented enforcement harm, not a
theoretical vulnerability report.

### Step 2 — C-suite simultaneous (28 May 2026)

The responsible disclosure email went to CLO, CISO, CIB Director, and
President Global Affairs simultaneously. Simultaneous delivery prevents
any single recipient from claiming the matter is outside their remit.

**Why these four:**
- CLO (Mahoney) — legal accountability + newest C-suite member, 4 months in role
- CISO (Rosen) — `__d=` is infrastructure security, directly in his mandate
- Actor Solutions (Ntwiga) — coordinated inauthentic behaviour is her specific domain
- Global Affairs (Kaplan) — regulatory dimension, government relations accountability

### Step 3 — Bug Bounty formal channel (3 June 2026)

The bug bounty submission created a permanent, trackable record inside
Meta's security infrastructure. Reference number: **#2428878307595078**.

**Triage navigation:**
The automated triage system attempted to classify the finding as a spam
issue. Correct navigation of the triage questionnaire — specifically
selecting "None of the above" for impact category — forced human review
rather than automatic closure as a known spam variant.

### Step 4 — Regulatory escalation (7 June 2026)

The California AG CPRA enforcement referral was filed only after:
- The account had been permanently disabled post-passport review
- All Meta-internal channels had produced zero substantive engagement
- The structural vulnerability had remained unremediated for 10 days
- Meta had explicitly stated "you cannot request another review"

The referral was framed as an enforcement referral, not a consumer complaint.
The difference: an enforcement referral cites completed, documented violations
with traceable records; a consumer complaint requests investigation of alleged
conduct. The former demands action; the latter requests inquiry.

---

## The CC Strategy

When regulatory escalation was filed, 8 Meta executives were CC'd
simultaneously on the email to the California AG:

```
To:  [email redacted]
CC:  [email redacted]
     [email redacted]       (CLO)
     [email redacted]        (CISO)
     [email redacted]     (Actor Solutions)
     [email redacted]      (Global Affairs)
     [email redacted]     (Head of Instagram)
     [email redacted]        (Chief Privacy Officer, Policy)
     [email redacted]    (Chief Privacy & Compliance Officer)
     [email redacted]        (Chief Product Officer)
```

**The logic:** Every Meta executive with accountability for any dimension
of this matter — legal, security, product, privacy, integrity, regulatory —
received the same document at the same moment. No executive could claim
the matter was outside their awareness or route it to a lower tier.

---

## What Made This Work

**The bug bounty number was the skeleton key.**

Every submission, every email, every form field that could include
`#2428878307595078` did. Any Meta employee reading any channel could
pull the full technical record from their own system immediately.
The number made the technical finding instantly verifiable without
requiring anyone to re-read the analysis from scratch.

**The notarized record created asymmetric evidentiary pressure.**

A notarized affidavit, attested true copies of all exhibits, a Special
Power of Attorney — these are the artifacts of serious legal proceedings,
not support requests. Their presence in a grievance submission signals
that the sender is prepared for litigation and has already built the
evidentiary record for it.
