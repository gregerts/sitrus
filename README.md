# SITRUS

## Formål

SITRUS-prosjektet har som formål å finne svaret på et av de store spørsmål:
*Hva er sammenhengen mellom sitrusfrukters ytre og indre egenskaper?*
De fleste har en formening om hva som er en god klementin og hva som er en dårlig,
men stemmer denne troen med virkeligheten?
Kan man si noe om en sitrusfrukt er søt, syrlig, saftig eller tam ved å se på skallet?
Det er dette vi skal finne ut...

## Metode

Prosjektet skal samle inn anonym sitrusdata fra deltakere i Norge.
Dette gjøres ved hjelp av en vevbasert *klient* som generere data,
og en *tjener* som logger innsamlet data til en sentral database for senere analyse.

Klienten vil ha sider for forskjellige sitrusfrukter, i første omgang spesifikt klementiner.
Følgende prosedyre følges for hver frukt som konsumeres:

1. Man trykker på binære utsagn om fruktens ytre kvaliteter,
er skallet tykk eller tynt og så videre. Deretter trykker man videre.
2. Man gjetter så på en del binære utsagn om fruktens indre kvaliteter, som sødme,
syrlighet, har den steiner og så videre. Deretter spiser man frukten.
3. Man fyller så ut de samme påstandene som i det forrige punktet etter man har konsumert frukten.
4. Til slutt trykker man send, og er klar for en ny frukt.

Innsamlet data vil bli analyser med Bayesianske metoder, mer om det siden.

## Implementasjon

Klienten blir utviklet i HTML og Javascript med støtte for små skjermer.

Tjeneren blir utviklet som REST-grensesnitt med Python, Flask og JSON.

PostgreSQL benyttes som database.

Analyse med Python, Pandas, PyMC og lignende.

## Resultat

Ved nok innsamlet data og statistisk signifikante resultat vil det utarbeides en selvhøytidlig artikkel som vil bli gjort tilgjengelig i romjulen 2015.
