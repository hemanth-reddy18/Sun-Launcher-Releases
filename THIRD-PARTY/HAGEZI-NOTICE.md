# Domain-filter data

The desktop browser source includes a HaGeZi Multi LIGHT domain-list snapshot retrieved on 2026-10-21 from https://raw.githubusercontent.com/hagezi/dns-blocklists/main/wildcard/light-onlydomains.txt . Upstream project: https://github.com/hagezi/dns-blocklists . Data license: GNU GPL v3; the complete upstream license is HAGEZI-LICENSE.txt alongside the snapshot. The separately bundled AdGuard Home native component is documented in shield/NOTICE.md.

The local request matcher checks hostnames and their parent domains. It is not cosmetic filtering, a same-domain video-ad remover or router-wide DNS configuration. The original snapshot is the browser fallback. Sun Shield downloads validated HaGeZi lists on explicit update/mode changes and shares the selected policy with Sun’s request matcher. Real local DNS filtering is tested separately; video-ad removal and system-wide protection are not claimed.
