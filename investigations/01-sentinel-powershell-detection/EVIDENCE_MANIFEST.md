# Evidence manifest — Sentinel Incident 4 (QA-reviewed draft)

Source: `Screenshots(2).zip` (original member bytes unchanged). Each packaged PNG is a documented cropped/redacted derivative; original and derivative SHA-256s are supplied for provenance.

| Packaged image | Original archive member | Original SHA-256 | Packaged SHA-256 | Evidence / limitations |
| --- | --- | --- | --- | --- |
| `evidence/01-process-creation.png` | `Screenshots/Screenshot (347).png` | `a1737e737372d61c3f2819c0b3bb464d58b2c7504cff3b679d40c31b0e4da109` | `adf5d5c9bfca35a23502dba202c2079b39265aebb22f9b1130b023b72f75c5f4` | Primary - unique process and parent-child PID |
| `evidence/02-analytics-rule.png` | `Screenshots/Screenshot (329).png` | `098cf13c1cb79fa5bd448944060a4959f8c426d90384000af6c6e4359a868bd0` | `a4c1fd370591c3a88d29d6eaa71c3add7d5e530b287deef6de6051e9f1934d74` | Primary - validated rule; pre-save UI |
| `evidence/03-incident-created.png` | `Screenshots/Screenshot (334).png` | `291aa275fd39cf5dc6dc04b6073633c2a3dbfc7157042157a6bb1f06bed74586` | `79c9a95f7d13fe6a51c96cbfaacd3bd86d1433fe7cee9384d1aa46b443b9422b` | Primary - incident with one alert |
| `evidence/04-timeline-34-events.png` | `Screenshots/Screenshot (340).png` | `63642a0af0701e72be577915f5e110000c9e1181581aa4b6dee60e8a526c5f92` | `f52e26984468885c91b3b87b18fe48a089a735742e12baac01b273d676ecd96a` | Primary - 34 event timeline; partial query |

## Supporting images not included

- `Screenshot (344).png`: 12-event intermediate result.
- `Screenshot (345).png`: one-event result (duplicates the expanded evidence in 347).
- `Screenshot (338).png`: **pre-save** incident closure settings, not confirmation that Save completed. Historical closure is documented in Module 11.

**Specific boundaries:** Event ID 4688 is established from the case notes and original query; it is not visible as a column in the expanded Screenshot 347. Screenshot 329 is a validated **pre-save** rule; Screenshot 334 is the separate actual incident. Screenshot 340 shows only the tail of the original investigation KQL.

## Review status

- Verified local README image links and packaged file integrity.
- Viewed all selected screenshots and checked them against the documented proof claim.
- Inspected visible crops for URL identifiers, email addresses, authentication secrets and network identifiers.
- Lab-only names and technical context remain; public-release naming decision and final user review remain outstanding.
- No claims of current cloud access, real intrusion, or production response are made.
