# Portfolio evidence previews

These previews reuse already-public sanitized screenshots from Jason Twyman's lab repositories. They are presentation derivatives, not new lab runs. Source links are pinned to the exact commits reviewed for this update.

Only raster images are included here. No datasets, raw events, credentials, packet captures, or executable telemetry were imported. The evidence and third-party material exclusions in the repository's [licensing notice](../../../LICENSE.md) apply; these screenshots are provided for portfolio review and verification, not relicensed as original code or prose.

## Splunk telemetry overview

- Preview: [splunk-dashboard.webp](splunk-dashboard.webp)
- Source: [published PNG](https://github.com/jasontwyman/splunk-mimikatz-detection-lab/blob/b5a90fbc6bc7dc5abc2ee6f387c4face52d843a7/docs/images/splunk-dashboard-overview-real-telemetry.png)
- Source SHA-256: `a37dd0eaf51253a3ad8fcb5b57816e159482c46883712dd8baeb663149cdb2f5`
- Preview SHA-256: `76622ea8c32f1876469d7c62aea31bfbc47ae35f183e89e14aac5d1556501248`
- Dimensions: 1342 x 637 pixels; 143264 bytes.
- Transformation: metadata-free RGB, lossless WebP encoding; no crop, resize, or changed RGB pixels.
- Supported view: event volume over time, top event IDs, and Windows logon activity from the historical OTRF dataset. This image is not independent proof of compromise, successful credential theft, or an alert firing. See the source repository's [evidence boundary](https://github.com/jasontwyman/splunk-mimikatz-detection-lab/blob/b5a90fbc6bc7dc5abc2ee6f387c4face52d843a7/README.md#public-evidence-boundary).

## Windows client share-access check

- Preview: [ad-share-validation.webp](ad-share-validation.webp)
- Source: [published PNG](https://github.com/jasontwyman/active-directory-home-lab/blob/9cafa9f09a19c8144ea4f67c04641c41558e4362/evidence/screenshots/23-client01-share-crud-validation.png)
- Source SHA-256: `642c391a9328b48405250744b4539a3acc2804335c44a1583fae99a8075effee`
- Preview SHA-256: `139db0b79e12c91f403bebb7499c13fbb7201d783fde9bb5c3778778cff31466`
- Dimensions: 960 x 277 pixels; 5398 bytes.
- Transformation: crop rectangle `(64, 65, 1024, 342)` in original pixel coordinates, with right and bottom exclusive; metadata-free RGB and lossless WebP encoding. No resize or changed RGB pixels within the retained region.
- The crop removes desktop background, the taskbar, and unused terminal area. It retains the PowerShell title, CLIENT01 heading, fictitious lab identity, mapped-share path, and all three validation outcomes.
- Supported view: the CLIENT01 lab check reports successful create, matching read-back, and delete results for the mapped share. It does not by itself establish all directory permissions, client-policy settings, or production readiness. See the source repository's [client validation context](https://github.com/jasontwyman/active-directory-home-lab/blob/9cafa9f09a19c8144ea4f67c04641c41558e4362/README.md#client01-domain-policy-and-mapped-drive-validation).
