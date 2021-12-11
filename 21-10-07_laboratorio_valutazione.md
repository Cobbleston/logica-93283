# Esercizio 1

> Teorema: se X ∩ Y = X allora X ⊆ Y
> 
> (Simboli utilizzabili: ∈ ∅ ∪ ∩ ⊆ ∀ ∃ ∧ ∨ ¬ ⇒ ⇔)

| Mio/Nostro                                                                  | Prof                                                                        |
| -:                                                                          | :-                                                                          |
| Siano X e Y insiemi tali che X ∩ Y = X,                                     | Siano X, Y insiemi t.c. X ∩ Y = X.                                          |
| ovvero, per l'assioma dell'estensionalità, ∀Z, Z ∈ X ∩ Y ⇔ Z ∈ X, (H1)      | Quindi, per l'assioma di estensionalità, si ha ∀Z. Z ∈ X ∩ Y ⇔ Z ∈ X (H).   |
| ovvero, per teorema intersezione binaria, ∀Z, (Z ∈ X ∧ Z ∈ Y) ⇔ Z ∈ X. (H2) | Dobbiamo dimostrare X ⊆ Y,                                                  |
| Quindi, ∀Z, (Z ∈ X ∧ Z ∈ Y) ⇔ Z ∈ X. (H3)                                   | ovvero ∀W. W ∈ X ⇒ W ∈ Y.                                                   |
| Devo dimostrare X ⊆ Y,                                                      | Sia W insieme t.c. W ∈ X.                                                   |
| ovvero ∀Z, (Z ∈ X ⇒ Z ∈ Y).                                                 | Quindi, per H, si ha W ∈ X ∩ Y.                                             |
| Sia Z insieme tale che Z ∈ X,                                               | Quindi, per il teorema dell'intersezione binaria, W ∈ X (H1) e W ∈ Y (H2).  |
| ovvio per H3 da destra a sinistra.                                          | Dobbiamo dimostrare W ∈ Y.                                                  |
|                                                                             | Ovvio per H2. qed.                                                          |

---

# Esercizio 2

> Teorema: X ∩ (Y ∪ Z) ⊆ (X ∩ Y) ∪ (X ∩ Z)
> 
> (Simboli utilizzabili: ∈ ∅ ∪ ∩ ⊆ ∀ ∃ ∧ ∨ ¬ ⇒ ⇔)

| Mio/Nostro                                                                                                                                    | Prof                                                                                                  |
| -:                                                                                                                                            | :-                                                                                                    |
| Siano X, Y, Z insiemi.                                                                                                                        | Siano X, Y, Z insiemi.                                                                                |
| Devo dimostrare che X ∩ (Y ∪ Z) ⊆ (X ∩ Y) ∪ (X ∩ Z),                                                                                          | Dobbiamo dimostrare X ∩ (Y ∪ Z) ⊆ (X ∩ Y) ∪ (X ∩ Z),                                                  |
| ovvero ∀W, W ∈ X ∩ (Y ∪ Z) ⇒ W ∈ (X ∩ Y) ∪ (X ∩ Z),                                                                                           | ovvero ∀W. W ∈ X ∩ (Y ∪ Z) ⇒ W ∈ (X ∩ Y) ∪ (X ∩ Z).                                                   |
| ovvero, per il teorema dell'intersezione binaria e dell'unione binaria, ∀W, (W ∈ X ∧ W ∈ (Y ∪ Z)) ⇒ (W ∈ (X ∩ Y) ∨ W ∈ (X ∩ Z)).              | Sia W insieme t.c. W ∈ X ∩ (Y ∪ Z).                                                                   |
| Ovvero, per il teorema dell'intersezione binaria e dell'unione binaria, ∀W, (W ∈ X ∧ (W ∈ Y ∨ W ∈ Z)) ⇒ ((W ∈ X ∧ W ∈ Y) ∨ (W ∈ X ∧ W ∈ Z)).  | Quindi, per il teorema dell'intersezione, W ∈ X (H1) e W ∈ Y ∪ Z.                                     |
| Sia W insieme tale che W ∈ X (H1) e (W ∈ Y (H2) oppure W ∈ Z (H3))                                                                            | Quindi, per l'assioma dell'unione binaria, W ∈ Y o W ∈ Z.                                             |
| Procedo per casi:                                                                                                                             | Procediamo per casi:                                                                                  |
|                                                                                                                                               |                                                                                                       |
| - Suppongo valgano H1 e H2.                                                                                                                   | - Caso W ∈ Y (H2):                                                                                    |
| Devo dimostrare che (W ∈ X e W ∈ Y) oppure (W ∈ X e W ∈ Z).                                                                                   |   Dobbiamo dimostrare W ∈ (X ∩ Y) ∪ (X ∩ Z).                                                          |
| Ovvio per H1 e H2.                                                                                                                            |   Per l'assioma dell'unione binaria, è sufficiente dimostrare W ∈ (X ∩ Y) o W  ∈(X ∩ Z).              |
|                                                                                                                                               |   Dimostriamo W ∈ X ∩ Y.                                                                              |
|                                                                                                                                               |   Per il teorema dell'intersezione binaria è sufficiente dimostrare W ∈ X e W ∈ Y.                    |
|                                                                                                                                               |   Ovvio per H1 e H2.                                                                                  |
|                                                                                                                                               |                                                                                                       |
| - Suppongo valgano H1 e H3.                                                                                                                   | - Caso W ∈ Z (H2):                                                                                    |
| Devo dimostrare che (W ∈ X e W ∈ Y) oppure (W ∈ X e W ∈ Z).                                                                                   |   Dobbiamo dimostrare W ∈ (X ∩ Y) ∪ (X ∩ Z).                                                          |
| Ovvio per H1 e H3.                                                                                                                            |   Per l'assioma dell'unione binaria, è sufficiente dimostrare W ∈ (X ∩ Y) o W ∈ (X ∩ Z).              |
|                                                                                                                                               |   Dimostriamo W ∈ X ∩ Z.                                                                              |
|                                                                                                                                               |   Per il teorema dell'intersezione binaria è sufficiente dimostrare W ∈ X e W ∈ Z.                    |
|                                                                                                                                               |   Ovvio per H1 e H2.                                                                                  |
|                                                                                                                                               |                                                                                                       |
|                                                                                                                                               | qed.                                                                                                  |

---

# Esercizio 3

> Sia c(W) = { Y ∈ U | ¬(Y ∈ W) } il complementare di W rispetto a U.
> 
> Teorema: se X ⊆ Y allora c(Y) ⊆ c(X)
> 
> (Simboli utilizzabili: ∈ ∅ ∪ ∩ ⊆ ∀ ∃ ∧ ∨ ¬ ⇒ ⇔)

| Mio/Nostro                                    | Prof                                                                                              |
| -:                                            | :-                                                                                                |
| Siano X, Y insiemi tali che X ⊆ Y,            | Siano X, Y, U insiemi t.c. X ⊆ Y,                                                                 |
| ovvero ∀Z, Z ∈ X ⇒ Z ∈ Y (H).                 | ovvero ∀Z. Z ∈ X ⇒ Z ∈ Y (H).                                                                     |
| Devo dimostrare che c(Y) ⊆ c(X),              | Dobbiamo dimostrare c(Y) ⊆ c(X),                                                                  |
| ovvero ∀Z, Z ∈ c(Y) ⇒ Z ∈ c(X),               | ovvero ∀W. W ∈ c(Y) ⇒ W ∈ c(X).                                                                   |
| ovvero ∀Z, ¬(Z ∈ Y) ⇒ ¬(Z ∈ X),               | Sia W insieme t.c. W ∈ c(Y).                                                                      |
| ovvero ∀Z, Z ∈ X ⇒ Z ∈ Y.                     | Quindi, per l'assioma di separazione, W ∈ U (H1) e ¬(W ∈ Y) (H2).                                 |
| Sia Z insieme tale che Z ∈ X. Ovvio per H.    | Dobbiamo dimostrare W ∈ c(X).                                                                     |
|                                               | Per l'assioma di separazione possiamo ridurci a dimostrare W ∈ U e ¬(W ∈ X).                      |
|                                               | - W ∈ U per H1                                                                                    |
|                                               | - Supponiamo W ∈ X (K) e dimostriamo l'assurdo. Da K e H si ha W ∈ Y. Quindi, per H2, assurdo.    |
|                                               | qed.                                                                                              |

---