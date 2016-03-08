# Changes 0.1 > 0.2

## Planed phoneme inventory

V = a u i e   y     o
   /a u i ɛ~e y~ɨ~ɯ ɔ~o/

|             | Bilabial | Linguolabial | Alveolar | Palatal | Velar | Glottal |
| ----------- |:--------:|:------------:|:--------:|:-------:|:-----:|:-------:|
| Plosive     | p        | t̼ (p̈)        | t        | [c]     | k     | ʔ  (')   |
| Nasal       | m        | n̼ (m̈)        | n        | ɲ (ń)   |       |         |
| Trill       |          |              | r        |         |       |         |
| Affricative |          |              |          | tɕ (c)  |       | h       |
| Fricative   | β (v)     | ð̼ (v̈)        | ʃ (s)    | ç (j)   |       |         |
| Lateral     |          |              | l        |         |       |         |

[c] is an allophone/in free variation with [tɕ]

Type p̈ m̈ v̈ using U_308

Example wordgen:
N=nljrtk
C=ptkcjqPmMnvVsrlh
V=auieyo
W=AUIEYO

A|ai
U|au
I|ia
E|eo
Y|ye
O|yo
P|p̈
M|m̈
V|v̈
CV
CW
CVN

U: unrounded vowel
O: rounded vowel

## Palatalisation
k > c / _i, _y, _e
n > ɲ / _i, _y
kʰ > k
i, y > Ø / ɲ_V (Reduce diphthongs ia iu ye yo > a u e o)
i, y > V / ɲ_C...V (Vowel gets replaced by the next vowel)

## Linguolabial consonants
First establish some new consonants and get the speakers used to them, then spread them everywhere.
ts > t̼ / U_U, #_U (katpe > kap̈e)
pn > n̼ / U_U, #_U (kapne > kam̈e)
pʰ > t̼ / _U (partial, as a form of emphasis)
m > n̼ / U_U, #_U
n > n̼ / U_U, #_U
β, s > / ð̼ #_U
pʰ > p (loose the remains of aspiration)
mp > n̼d̼ / _U

# Changes ?? > ??

Maybe establish a bi-syllabic root system using tone and infixes. Or create another language for it.
Example derivations for **pa.ku**:
pánkù, pālkur, apákùn, pakūkū, pákūkù
