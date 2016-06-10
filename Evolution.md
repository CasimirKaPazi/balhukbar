Evolution
=========

# Changes 0.1 > 0.2

## Planed phoneme inventory

|                   | Bilabial | Linguolabial | Alveolar | Palatal | Velar | Glottal |
| ----------------- |:--------:|:------------:|:--------:|:-------:|:-----:|:-------:|
| Plosive           | p        | t̼ (p̈)        | t        |         | k     | ʔ  (')  |
| Nasal             | m        | n̼ (m̈)        | n        | ɲ (ń)   | [ŋ]   |         |
| Trill             | ʙ (br/ř) |              | r        |         |       |         |
| Affricative       |          |              | [ɾ]      | tɕ (c)  |       | Ø~h~x   |
| Fricative         | ɸ (v)    | ð̼ (v̈)        | ʃ (s)    | ç (j)   |       |         |
| Lateral fricative |          |              | ɬ (ł)    |         |       |         |
| Lateral           |          | [l̼]          | l        |         |       |         |

Type p̈ m̈ v̈ using U_308

Example wordgen:  

```
N=nljrq
C=ptk'PmncjMvVsbrlłh
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
```

U: unrounded vowel  
O: rounded vowel

h > ʔ / V_V
ʔ > h / !#_ (make ʔ and h only differ at the start of a word)

## Lateral fricative
tl,tr,lt,rt > ɬ

## Bilabial trill
pr,br,vr > ʙ

## Palatalisation
k > tɕ / _i, _y, _e  
n > ɲ / _i, _y  
kʰ > k  
i, y > Ø / {tɕ,ç,ɲ}_V (Reduce diphthongs ia iu ye yo > a u e o)  
i, y > V / {tɕ,ç,ɲ}_CV (Vowel gets replaced by the next vowel)

## Linguolabial consonants
First establish some new consonants and get the speakers used to them, then spread them everywhere.  
ts > t̼ / U_U, #_U (katpe > kap̈e)  
pn,np > n̼ / U_U, #_U (kapne > kam̈e)  
pʰ > t̼ / _U
m > n̼ / U_U  
ɸ, s > ð̼ / U_U  
pʰ > p (loose the remains of aspiration)  
mp > n̼d̼ / _U
m > n̼ / #_UC[+linguolabial]
p > t̼ / #_UC[+linguolabial]
ɸ, s > ð̼ / #_UC[+linguolabial]
r > ʙ / #_UC[+linguolabial]

## Turn codas into archiphonemes

|     | Bilabial | Linguolabial | Alveolar | Palatal | Velar | Glottal | End of Word |
|:---:|:--------:|:------------:|:--------:|:-------:|:-----:|:-------:|:-----------:|
| /P/ | p        | p            | t        | k       | k     | t.h     | p           |
| /N/ | m        | n̼            | n        | ɲ       | ŋ     | n.h     | m/ŋ         |
| /R/ | r        | r            | r        | r       | r     | r.h     | ɾ           |
| /L/ | l        | l̼            | l        | l       | l     | l.h     | l           |
| /V/ | v        | ð̼            | ç        | ç       | ç     | ç.ʔ     | ç           |
            

Stops /P/ < q >  
Geminates before p, t, k.  
P > p   / _C[+bilabial]  
P > p   / _C[+linguolabial]  
P > t   / _C[+alveolar]  
P > k   / _C[+velar]  
P.C > t.ʔ / _C[+glottal] (glottal sound is replaced)  
P > k   / {a,o,u}_#  
P > p   / {i,e,y}_# (p is without release here)  

'uqbar [ʔup:ar]  
muqhan [mut.çaŋ]  


Nasals /N/ < n >  
Geminates before another nasal.  
N > m / _C[+bilabial]  
N > n̼ / _C[+linguolabial]  
N > n / _C[+alveolar]  
N > ŋ / _C[+velar]  
N > ŋ / {a,o,u}_#  
N > m / {i,e,y}_#  

patan [patam]  
tenpo [tempo]  
linma [lim:a]  

Fricative /F/ < v >  
F > ɸ / _C[+bilabial]  
F > ð̼ / _C[+linguolabial]  
F > ç / _C[+alveolar]  
F > ç / _C[+velar]  
F > ç / V_#  

Trill/Flap /R/ < r >  
R > ɾ / V_#  
R > r / else  

Lateral /l/ < l >  
L > l̼ / _C[+linguolabial]  
L > l / else  
