# Elprisprognos SE3

Öppen prognos för spotpriset i elområde SE3 (Nord Pool day-ahead), kvart för kvart 1–10 dygn framåt, med
osäkerhetsband och uppmätt träffsäkerhet.

- **Dashboard:** https://8bitcat.github.io/elprisprognos/
- **API:** https://8bitcat.github.io/elprisprognos/api/v1/index.json

| Fil | Innehåll |
|---|---|
| `api/v1/SE3/senaste.json` | Senaste prognosen: 240 timmar och 960 kvartar, p10/p50/p90 i SEK/kWh |
| `api/v1/SE3/prognoser/<datum>.json` | Prognosen som gjordes den morgonen. Ändras aldrig |
| `api/v1/SE3/traffsakerhet.json` | Medelfel per prognoslängd och per kvart på dygnet, skarpt och efterhandsprövat |
| `api/v1/SE3/inlarning.json` | Inlärningsslingan: felet per iteration och versionerna i drift |

Filerna uppdateras varje dag ca 10:30, före Nord Pools auktion kl 12. Commit-tiden i historiken visar att
prognosen fanns innan priset publicerades. Prognoserna får användas fritt med angivande av källa (CC BY 4.0).
