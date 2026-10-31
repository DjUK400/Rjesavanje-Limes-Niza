# Rješavanje limesa niza

### 👉 [Otvori sajt: djuk400.github.io/Rjesavanje-Limes-Niza](https://djuk400.github.io/Rjesavanje-Limes-Niza/)

Besplatan sajt za studente koji rješava limese nizova **korak po korak**. Cilj nije da prepišeš rezultat, nego da naučiš postupak: svaki korak ima hint i obrazloženje *zašto* se radi baš tako. Zadaci su urađeni po uzoru na vježbe, kolokvijume i ispitne rokove iz Matematike 1 (građevinski fakultet).

Radi na računaru i na telefonu (i na iPhoneu), bez instalacije i bez prijave.

---

## Podržani tipovi zadataka

| # | Tip | Primjer | Metoda |
|---|-----|---------|--------|
| 1 | Količnik polinoma (∞/∞) | (2n²+3n−4)/(3n²−4n+1) → 2/3 | izvlačenje najvećeg stepena |
| 2 | Zbir stepena aⁿ / zbir stepena | (2ⁿ⁺¹+3ⁿ⁺¹)/(2ⁿ+3ⁿ) → 3 | izvlačenje najveće osnove |
| 3 | n-ti korijen zbira stepena | ⁿ√(1+5ⁿ+9ⁿ) → 9 | teorema o dva policajca |
| 4 | Suma 1…n kroz polinom | (1²+2²+…+n²)/n³ → 1/3 | formule za Σk, Σk², Σk³ |
| 5 | Teleskopska suma | 1/(1·2)+…+1/(n(n+1)) → 1 | rastavljanje i poništavanje |
| 6 | Sendvič za sumu | Σ 1/√(4n²+k) → 1/2 | teorema o dva policajca |
| 7 | Razlika korijena (∞−∞) | n(√(n²+1) − ∛(n³+n)) → 1/6 | racionalizacija |
| 8 | Oblik 1^∞ | ((2n+3)/(2n+1))²ⁿ → e² | svođenje na (1+1/x)ˣ → e |
| 9 | Ograničen × nula-niz | n^(4/5)·cos(nπ)/(2n+3) → 0 | teorema o ograničenom nizu, podnizovi |
| 10 | Određivanje parametara a i b | √(x²−3x+2) − ax + b → 0 ⇒ a=1, b=3/2 | koeficijent uz x = 0, konstanta = L |

Svaki tip ima dugmad sa primjerima sa kolokvijuma, koji se učitaju jednim klikom.

## Kako pomaže u učenju

- **Hintovi (prekidač):** kad je uključen, za svaki korak prvo vidiš samo pitanje-hint, pa korak otvaraš sam. I rezultat je sakriven. Kad je isključen, odmah se vidi cijelo rješenje.
- **„Zašto?“:** uz svaki korak je obrazloženje pravila ili teoreme koja se koristi.
- **Pokušaj sam:** upišeš svoj odgovor (`2/3`, `-inf`, `e^2`, `sqrt(2)/2`, `ne postoji`), a sajt ga provjeri.
- **Numerička provjera:** tabela vrijednosti za n = 10, 100, 1000… služi samo kao ilustracija, nije dokaz.

## Tab „Pravila i pojmovi“

- definicija limesa (ε–n₀), konvergencija i divergencija, ograničenost, monotonost, podnizovi
- pravila za operacije sa limesima
- standardni limesi (qⁿ, ⁿ√a, ⁿ√n, broj e, …)
- računanje sa ∞ (određeni oblici)
- svih **7 neodređenih oblika**: 0/0, ∞/∞, ∞−∞, 0·∞, 1^∞, 0⁰, ∞⁰, uz primjere zašto su neodređeni i kako se rješavaju
- teoreme: dva policajca, ograničen × nula-niz, Weierstrass, podnizovi, teleskopska suma, Štolc
- hijerarhija rasta: ln n ≪ nᵖ ≪ aⁿ ≪ n! ≪ nⁿ
- formule za sume i algebarske formule za racionalizaciju
- „Koju metodu kada?“ i česte greške

## Kako se unosi

- množenje: `3n` ili `3*n` · stepen: `n^2` · zagrade: `(2k+1)^2` · razlomak broja: `7/4`
- eksponencijalni član: `3*2^(n+1)`, `(-2)^n`
- brojilac i imenilac se unose u odvojena polja
- pregled zadatka se prikazuje uživo dok kucaš

## Ograničenja

- Sajt rješava **samo navedene tipove** (šablone). Ako unos ne odgovara šablonu, dobiješ obavještenje na ekranu, a ne pogrešno rješenje.
- Nisu podržani: rekurzivni nizovi, dokazi po definiciji (ε) i opšti nizovi sa ln i n!.
- Koraci su matematički ispravni, ali zapis se može razlikovati od onog koji traži profesor.
- Formule se prikazuju preko biblioteke KaTeX, za koju je potreban internet. Bez interneta računanje radi, ali se formule vide kao sirovi tekst.

## Tehnički

Jedan fajl, `index.html`, bez servera. Računanje se radi u browseru tačnom racionalnom aritmetikom (BigInt), a za korijene i broj e koristi se simbolički zapis.
