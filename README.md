# Lekòl Anliy

Sit lekòl an liy: elèv yo achte kou, pwofesè yo touche yon pousantaj sou chak vant, epi admin nan peye pwofesè yo.

## Paj yo
- **Akèy** – prezantasyon lekòl la ak kou popilè yo
- **Kou yo** – katalòg kou yo (bouton "Achte" similye yon vant)
- **Espas pwofesè** – revni, lajan an atant, lajan disponib, demann retrè
- **Admin** – revni lekòl la, demann retrè pou peye, règ peman yo

## Règ peman (pa default)
| Règ | Valè |
|---|---|
| Pati pwofesè | 70% apre frè |
| Frè peman | 3% |
| Jou an atant anvan lajan disponib | 14 |
| Retrè minimòm | 1,000 HTG |

## Eta pwojè a
Sa se yon **demo**: tout done yo rete nan navigatè a (localStorage), pa gen vrè lajan ki sikile.

## Pwochen etap
1. Backend + baz done (kont elèv, pwofesè, kou, vant, peman)
2. Konekte MonCash / NatCash (oswa Bazik API) pou resevwa ak voye peman
3. Login pou elèv, pwofesè ak admin
4. Non domèn + hosting

## Kijan pou louvri l
Louvri `index.html` nan navigatè a. Oswa aktive **GitHub Pages** (Settings → Pages → branch `main`).

## Koneksyon Google (pou aktive l pou tout bon)
1. Ale sou https://console.cloud.google.com → kreye yon pwojè (egzanp: "Lekol Anliy").
2. **APIs & Services → OAuth consent screen**: chwazi "External", mete non sit la, imèl ou, epi pibliye l.
3. **APIs & Services → Credentials → Create credentials → OAuth client ID** → tip **Web application**.
4. Nan **Authorized JavaScript origins**, mete: `https://zayden509.github.io` (epi domèn ou si w genyen youn, egzanp `https://lekolanliy.com`).
5. Kopye **Client ID** a (li fini ak `.apps.googleusercontent.com`).
6. Nan `index.html`, chèche `const GOOGLE_CLIENT_ID="";` epi kole ID a ant gimè yo.

⚠️ Sou yon vrè sit, backend la dwe verifye token Google la anvan li louvri kont lan.
