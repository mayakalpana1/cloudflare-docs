---
_build:
  publishResources: false
  render: never
  list: never
---

Use this selector to match domains (and optionally, [IP addresses](/cloudflare-one/policies/gateway/domain-categories/#filter-traffic-by-resolved-ip-category)) belonging to specific [security categories](/cloudflare-one/policies/gateway/domain-categories/#security-categories).

| UI name             | API example                            | Evaluation phase      |
| ------------------- | -------------------------------------- | --------------------- |
| Security Categories | `any(dns.security_category[*] in {1})` | Before DNS resolution |
