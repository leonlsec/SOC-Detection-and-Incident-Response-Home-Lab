# Evidence manifest — Defender XDR Incident 3 (QA-reviewed draft)

Source: `Screenshots(2).zip` (original member bytes unchanged). Each packaged PNG is a documented cropped/redacted derivative; original and derivative SHA-256s are supplied for provenance.

| Packaged image | Original archive member | Original SHA-256 | Packaged SHA-256 | Evidence / limitations |
| --- | --- | --- | --- | --- |
| `evidence/01-device-inventory.png` | `Screenshots/Screenshot (119).png` | `e8b0b697e204a48a598fb1ac3b1d6234a62e0233dd305f34f0ebd06e11d1bb4b` | `3754113db2465f1b48bbc3bdab074b4dbcc7c54fe4803b377884bbaf3f4f3926` | Primary - device health and scan-history caveat |
| `evidence/02-incident-created.png` | `Screenshots/Screenshot (125).png` | `7f57e5f40cc821edb1d2f8e26b5c11aab49a89099139f2e6df831a7551aaa8ad` | `5cfc5d392ebde95df286321e8df9ce2254ddbbaf5b6ddef87d2edec3a993219f` | Primary - initial incident |
| `evidence/03-alert-blocked.png` | `Screenshots/Screenshot (126).png` | `e2999c2886e3a4390b116168abe405e221f1dea9ca94b2dbdc0c3a6d6ece2476` | `538a8f982b7239f2831c04f612cfd51f39efbe44254855ba665cef206d37ad8c` | Primary - protection Blocked, workflow New |
| `evidence/04-process-tree.png` | `Screenshots/Screenshot (127).png` | `17182d40272b72cfd3130824ab3e8d75af99b71ad8fb804c744b40288b7b4193` | `3602137297babfab6335dc54db1526255c7e6eda8fb9498ce94eac9335e8b5cf` | Primary - process ancestry |
| `evidence/05-incident-resolved.png` | `Screenshots/Screenshot (132).png` | `3e1d2460d2eb3a2a65b3d5af8e0770112251c7ba4115b29a4666cef20e05d8d4` | `a9d24f0c28772e04d2cd322feebef93670a22a73a7974628918edea76c346b96` | Primary - incident resolved, Unclassified |
| `evidence/appendix-alertinfo-kql.png` | `Screenshots/Screenshot (170).png` | `621a2d59c0574382043f64375ab3c219289bf197d4e7bc8fe3ec433575d8a8ab` | `db922e6206b3afc81c1653a330c1d8e5d6416f1c6841fa30e5887e075e2821c0` | Appendix - original query and one result |

## Supporting images not included

- `Screenshot (128).png`: **pre-save** alert classification selected as Informational, expected activity; not evidence that this classification persisted after saving.
- `Screenshot (130).png`: post-save Resolved alert row, distinct from classification.
- Independent scan/isolation/release/Live Response exercises from Module 10 Step 10.6 are **not** containment of Incident 3 and are excluded from this case.

**Specific boundaries:** The original PowerShell command produced a `CommandNotFoundException` although Defender blocked the observed test behavior. Incident 3 ended Resolved with 0 active alerts while **incident-level classification remained Unclassified**. The `AlertInfo` query is historical and has a relative time filter. The inventory screenshot retains its scan-history warning and uses a solid mask over the source device/network identifier area.

## Review status

- Verified local README image links and packaged file integrity.
- Viewed all selected screenshots and checked them against the documented proof claim.
- Inspected visible crops for URL identifiers, email addresses, authentication secrets and network identifiers.
- Lab-only names and technical context remain; the author approved keeping the lab-only identifiers, and the repository was published on 27 November 2026.
- No claims of current cloud access, real intrusion, or production response are made.
