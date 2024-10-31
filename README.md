# Actor Recognizor

**Actor Recognizor** je projekat koji koristi **duboko učenje** za prepoznavanje lica poznatih ličnosti na slikama.
Projekat koristi skup od **17,354 slika** sa licima 105 poznatih glumaca. 

## Tehnike i Pristup

- **Priprema podataka**: Skaliranje slika na 224x224, konverzija u tenzore, i normalizacija za stabilniji trening.
- **Modeli**: Primena **VGG** i **ResNet** arhitektura sa **fine-tuning** pristupom, omogućava brže treniranje i bolje performanse.
- **Trening strategija**: Modeli su trenirani prvo na samo potpuno povezanim slojevima, zatim na konvolucionim slojevima, a zatim na oba zajedno.
  
## Rezultati

**ResNet** se pokazao kao najbolji model, sa visokom preciznošću prepoznavanja, zahvaljujući rezidualnim blokovima koji omogućavaju efikasnije treniranje dubljih mreža. Testiranje je potvrdilo da model generalizuje dobro i nije preprilagođen (bez overfittinga).

## Zaključak

Fine-tuning pre-treniranih modela poput ResNet-a omogućio je visoke performanse čak i sa manjim skupom podataka, čime je projekat pokazao robusnost i pouzdanost za realne primene.

---

**Tehnologije korišćene**: PyTorch, VGG, ResNet, preprocessing i evaluacija performansi.

[Pregledajte PDF dokument](https://github.com/dimitrijemarkovic/ActorRecognizer/blob/main/Prepoznavanje%20glumaca%20koriscenjem%20neuronskih%20mreza.pdf)
