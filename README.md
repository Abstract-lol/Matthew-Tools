# Matthew-Tools
Crackelt verziója a Matthew Tools kliensnek.

```diff
- Nem biztos hogy a kliensben nincsen grabber, nem lett teljesen visszafejtve, csak az authot bypassoltuk.
```

## Hogyan?
A crack egy **hosts** file exploitot használ, ami felülírja az eredeti auth szervernek a helyét *(api.kolink.best ➔ 127.0.0.1)*, ahol egy elkülönített auth szerver fut.

# Telepítés / Setup
1. A **hosts** fájlodat kell patchelned. Ezt megteheted a mellékelt .bat fájllal amit mellékeltünk, vagy a `C:\Windows\System32\drivers\etc\hosts` fájl végére bemásolod ezt: `127.0.0.1 api.kolink.best`. *Ez annyit csinál, hogy az api.kolink.best-et átirányítja localhostra.*
2. A szervert hostolnod is kell. Erre [**xampp**](https://www.apachefriends.org/hu/index.html)-t ajánlunk. Csak Apache servicet kell elíndítani.
***VAGY***
2.1 A szervert egy weboldal hoston is hostolhatod, hogyha ezt csinálod a `127.0.0.1`-et cseréld ki a weboldal domainodra.
3. Índítsd el a kliens-t, és jelentkezz be bármilyen adattal.
