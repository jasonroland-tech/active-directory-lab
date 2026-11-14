# Build log

| Date | What I built | What broke | How I fixed it |
| --- | --- | --- | --- |
| 2026-11-12 | DC01 VM (D2as v5, static 172.16.0.4, RDP locked to my IP, auto shutdown), promoted to lab.local, VNet DNS set to DC01 | B2s and D2s v3 unavailable on the free subscription; 10.0.0.4 rejected | Used D2as v5; the subnet is 172.16.0.0/24 |
| 2026-11-12 | 6 OUs, 5 groups and 40 users from CSV with New-LabUsers.ps1 (WhatIf first) | WhatIf run skipped writing its own log | Added -WhatIf:$false to the log writes |
