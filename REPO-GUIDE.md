# Repository guide · دليل تنظيم المستودعات

GitHub has no folders for repositories. Organization comes from four things: **name prefix, topics, pinned repos and Stars lists**. Apply all four to every new repo.

لا يدعم GitHub مجلدات للمستودعات؛ التنظيم يتم عبر: **بادئة الاسم، الوسوم (Topics)، المستودعات المثبتة، وقوائم النجوم**.

## 1. Naming · التسمية

`<prefix>-<product-or-client>-<component>` — lowercase, hyphens only.

| Category | Prefix | Category topic | Pillar topic | Example name |
|---|---|---|---|---|
| SaaS | `saas-` | `saas` | `axis-platforms-ai-automation` | `saas-clinic-api` |
| Odoo | `odoo-` | `odoo` | `axis-odoo-erp` | `odoo-hr-payroll-eg` |
| Vibe Coding | `vibe-` | `vibe-coding` | `axis-platforms-ai-automation` | `vibe-crm-landing` |
| AI & Automation | `ai-` | `ai-automation` | `axis-platforms-ai-automation` | `ai-whatsapp-agent` |
| BI & Dashboards | `bi-` | `business-intelligence` | `axis-business-intelligence` | `bi-sales-dashboard` |
| Integrations | `int-` | `integration` | `axis-platforms-ai-automation` | `int-odoo-shopify` |
| Mobile | `app-` | `mobile` | `axis-platforms-ai-automation` | `app-field-service` |
| Templates & Tools | `kit-` | `starter-kit` | by content | `kit-nextjs-saas` |

Odoo modules: put the target version in the topics (`odoo-17`, `odoo-18`) and keep one addon per folder at repo root so the repo works as an addons path.

## 2. Topics · الوسوم

Every repo gets 4–7 topics:

1. **Pillar topic**, exactly one, required (shared with the company profile): `axis-odoo-erp`, `axis-business-intelligence` or `axis-platforms-ai-automation`
2. **Category topic** (from the table, required: the profile links filter on it)
3. **Stack**: `python`, `nextjs`, `nestjs`, `go`, `flutter`, `postgresql`
4. **Industry** when relevant: `healthcare`, `legal`, `hospitality`, `real-estate`
5. **Status**: `production`, `mvp`, `prototype`, `archived`

## 3. Visibility rules · قواعد الظهور

| Repo type | Where | Visibility |
|---|---|---|
| Client work | `I-Solutions-Technology` org | Private, always |
| Company products (SaaS core) | `I-Solutions-Technology` org | Private |
| Open-source Odoo modules, kits | personal or org | Public |
| Vibe-coding prototypes / demos | personal | Public (no client data, no secrets) |

## 4. Profile curation · تنسيق الصفحة الشخصية

- **Pin 6 repos** max: best of SaaS, Odoo, AI, plus 1 vibe-coding demo. Pin outcomes, not experiments.
- **Stars lists** (Stars → Lists): create `SaaS`, `Odoo`, `Vibe Coding`, `AI & Automation` to group repos you own and reference repos.
- Add each repo's **About** line: one sentence on the business outcome, plus a live demo URL when one exists.

## 5. New repo checklist · قائمة إنشاء مستودع جديد

- [ ] Name follows `<prefix>-<name>`
- [ ] Pillar topic + category topic + stack + status topics added
- [ ] About description + website URL filled in
- [ ] README: problem → solution → stack → screenshots → how to run
- [ ] `.env.example` committed, no real secrets; secret scanning on
- [ ] License chosen (public repos: MIT for kits, LGPL-3 for Odoo modules)
