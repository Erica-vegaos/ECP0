# TAL-E Commercial Extension – Detailed Pricing & Usage Guide
_Effective: 2025-04-25 · Maintained by Eriga Enrich Inc._

---

## 1 Token Definition & Billing Unit
* **Count method** = OpenAI tokenizer (≈ 4 characters ≈ 0.75 Chinese chrs).  
* **Direction** = **in + out** tokens per request.  
* **Billing granularity** = blocks of **1 000 tokens** (rounded up).  
* **Reset** = token quota resets at 00:00 UTC on the 1st of each month.

---

## 2 API Endpoints & Rate Limits

| Tier | Endpoint | RPS | Burst | Tenant Type |
|------|----------|-----|-------|-------------|
| **Sandbox** | `POST /v1/check` | 10 | 50 | Shared |
| **Enterprise** | `POST /enterprise/{key}/check` | 30 | 150 | Single-tenant |
| **Enterprise Plus** | Custom domain / on-prem | Negotiated | Negotiated | Dedicated |

> **429 Too Many Requests** ⇒ exponential back-off.  
> Spike capacity > Burst needs advance notice (≥ 48 h).

---

## 3 Tier Specifications

### 3.1 Free / Internal
* **Quota** ≤ 50 users _or_ ≤ 1 M tokens / month.  
* **Permitted** academic & internal R&D.  
* **SLA** community best-effort.  
* **TX access** TX01, TX04.

### 3.2 Sandbox — $199 / month
| Item | Quota |
|------|-------|
| Included tokens | **5 M / month** |
| Rate limit | 10 RPS, burst 50 |
| Overage | **$9 / M** |
| Support | 72 h email |
| TX access | + TX02-Lite, TX05-Lite |

### 3.3 Enterprise — $29 / seat / month (annual billing)
| Item | Quota |
|------|-------|
| Included tokens | **50 M / seat / month** |
| Seats counted | Unique humans/calendar-month |
| Overage | **$6 / M** |
| SLA | 24 h email (workdays) |
| Additional seat | $1 500 / year |
| TX access | + TX02-Pro, TX03, TX05-Pro |

### 3.4 Enterprise Plus — custom (≥ $100 000 / year)
* Min. commit ≥ 500 M tokens / year.  
* Options: dedicated VPC, on-prem, white-label.  
* SLA 4 h ticket / Slack 24×7.  
* Eligible for **joint-IP clause design**.

---

## 4 Upgrade / Downgrade

| From | To | Immediate? | Proration |
|------|----|------------|-----------|
| Free → Sandbox | ✅ | N/A |
| Sandbox → Enterprise | ✅ | Overage credited |
| Enterprise → Plus | ✅ | Custom |
| Paid → Lower tier | 30-day notice | End-of-cycle |

---

## 5 Support & SLA Matrix

| Tier | Response window | Incident updates |
|------|-----------------|------------------|
| Sandbox | ≤ 72 h | N/A |
| Enterprise | ≤ 24 h (workdays) | Every 8 h |
| Enterprise Plus | ≤ 4 h | Every 2 h |

---

## 6 Compliance Add-ons

| Pack | Fee | Contents |
|------|-----|----------|
| EU AI Act / SOC 2 reports | $5 000 one-off | Audit mapping, report template |
| Custom clause dev. | from $20 000 | Joint IP or exclusive |

---

## 7 Billing & Payment
* Invoiced annually (monthly option +8 %).  
* Accepted: bank wire (USD / TWD), major cards.  
* Prices exclude VAT/GST.

---

## 8 Contact
For quotes or the TAL-E Extension Agreement  
✉️ **ericaxvega@hotmail.com** (primary contact)

*All prices may change; existing customers receive 90-day notice.*

