# Byte — juridiska sidor

Publika sidor för appen **Byte** (`se.byte.app`), länkade från Google Play.

| Sida | Används av |
|------|------------|
| [privacy.html](https://appa87.github.io/byte-legal/privacy.html) | Play Console → Store listing → Privacy policy |
| [radera-konto.html](https://appa87.github.io/byte-legal/radera-konto.html) | Play Console → Data safety → Account deletion |
| [terms.html](https://appa87.github.io/byte-legal/terms.html) | Användarvillkor |

## Redigera inte filerna här

De är **genererade**. Källan är `apps/mobile/constants/legal.ts` i huvudrepot,
samma modul som appens egna skärmar renderar — så texten i appen och texten
Google Play länkar till kan inte glida isär.

Ändra texten där, kör generatorn, och synka hit:

```bash
npm run build:legal-site -w @byte/mobile   # skriver docs/
npm run publish:legal-site                 # speglar docs/ hit och pushar
```

En redigering direkt i det här repot skrivs över vid nästa synk.

## Varför ett eget repo

Huvudrepot är privat, och GitHub Pages på privat repo kräver GitHub Pro. Det
här repot innehåller bara de fyra sidor som ändå är tänkta att vara offentliga
— ingen kod.
