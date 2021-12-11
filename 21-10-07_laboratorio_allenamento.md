# Esercizio 1

> Teorema: X ⊆ X ∪ ∅
> 
> (Simboli utilizzabili: ∈ ∅ ∪ ∩ ⊆ ∀ ∃ ∧ ∨ ¬ ⇒ ⇔)

| Mio/Nostro                                                            | Prof                                                                           |
| -:                                                                    | :-                                                                             |
| Sia X un insieme.                                                     | Sia X un insieme.                                                              |
| Dobbiamo dimostrare X ⊆ X ∪ ∅,                                        | Dobbiamo dimostrare X ⊆ X ∪ ∅,                                                 |
| ovvero ∀Y . Y ∈ X ⇒ Y ∈ X ∪ ∅                                         | ovvero ∀Y. Y ∈ X ⇒ Y ∈ X ∪ ∅.                                                  |
| Per l'assioma dell'unione binaria Y ∈ X ∪ ∅ ⇔ Y ∈ X ∨ Y ∈ ∅.          | Sia Y un insieme t.c. Y ∈ X (H).                                               |
| Y non ∈ ∅ per l'assioma dell'insieme vuoto, quindi Y ∈ X ∪ ∅ ⇔ Y ∈ X. | Per l'assioma dell'unione binaria possiamo ridurci a dimostrare Y ∈ X ∨ Y ∈ ∅. |
| Debbo dimostrare Y ∈ X ⇔ Y ∈ X. Qed.                                  | Dimostro Y ∈ X.                                                                |
|                                                                       | Ovvio per H. Qed.                                                              |

# Esercizio 2

> Teorema: X ∪ ∅ ⊆ X
> 
> (Simboli utilizzabili: ∈ ∅ ∪ ∩ ⊆ ∀ ∃ ∧ ∨ ¬ ⇒ ⇔)

| Mio/Nostro                                                       | Prof                                                                           |
| -:                                                               | :-                                                                             |
| Sia X un insieme.                                                | Sia X un insieme.                                                              |
| Debbo dimostrare che X ∪ ∅ ⊆ X,                                  | Dobbiamo dimostrare X ∪ ∅ ⊆ X,                                                 |
| ovvero ∀Y . Y ∈ X ∪ ∅ ⇒ Y ∈ X                                    | ovvero ∀Y. Y ∈ X ∪ ∅ ⇒ Y ∈ X.                                                  |
| Sia Y un insieme tale che Y ∈ X ∪ ∅.                             | Sia Y un insieme t.c. Y ∈ X ∪ ∅ (H).                                           |
| Per il teorema dell'unione binaria Y ∈ X oppure Y ∈ ∅.           | Per l'assioma dell'unione binaria e H, Y ∈ X ∨ Y ∈ ∅.                          |
| Per l'assioma dell'insieme vuoto non è possibile il secondo caso | Procediamo per casi.                                                           |
| Caso 1. Y ∈ X (H): Debbo dimostrare che Y ∈ X. Ovvio per H       | Caso Y ∈ X (H). Dobbiamo dimostrare Y ∈ X. Ovvio per H.                        |
|                                                                  | Caso Y ∈ ∅ (H). Per H e l'assioma dell'insieme vuoto, assurdo. Quindi Y ∈ X.   |
|                                                                  | Qed.                                                                           |

# Esercizio 3

> Teorema: se X ⊆ Y allora X ∩ Y = X
> 
> (Simboli utilizzabili: ∈ ∅ ∪ ∩ ⊆ ∀ ∃ ∧ ∨ ¬ ⇒ ⇔)

| Mio/Nostro                                                             | Prof                                                                                     |
| -:                                                                     | :-                                                                                       |
| Siano X, Y insiemi t.c. X ⊆ Y (H1)                                     | Siano X, Y insiemi t.c. X ⊆ Y,                                                           |
| Ovvero ∀Z . Z ∈ X ⇒ Z ∈ Y                                              | ovvero ∀Z. Z ∈ X ⇒ Z ∈ Y (H1).                                                           |
| Sia Z un insieme tale che Z ∈ X                                        | Dobbiamo dimostrare X ∩ Y = X.                                                           |
| Per (H1) Z ∈ Y (H2)                                                    | Per l'assioma di estensionalità, ci riduciamo a dimostrare ∀Z. Z ∈ X ∩ Y ⇔ Z ∈ X.        |
| Debbo dimostrare X ∩ Y = X.                                            | Sia Z insieme.                                                                           |
| Per l'assioma dell'estensionalità X ∩ Y = X ⇔ (∀Z (Z ∈ X ∩ Y ⇔ Z ∈ Y)) |                                                                                          |
| Debbo dimostrare quindi ∀Z (Z ∈ X ∩ Y ⇔ Z ∈ Y)                         | Dimostriamo Z ∈ X ⇒ Z ∈ X ∩ Y.                                                           |
| Sia Z un insieme tale che Z ∈ X ∩ Y                                    | Assumiamo Z ∈ X (H2).                                                                    |
| Ovvero Z ∈ X ∧ Z ∈ Y                                                   | Quindi, per H1, Z ∈ Y (H3).                                                              |
| Poichè X ⊆ Y allora                                                    | Per H2, H3 e il teorema che caratterizza l'intersezione binaria, Z ∈ X ∩ Y.              |
|                                                                        |                                                                                          |
|                                                                        | Dimostriamo Z ∈ X ∩ Y ⇒ Z ∈ X.                                                           |
|                                                                        | Assumiamo Z ∈ X ∩ Y.                                                                     |
|                                                                        | Quindi, per il teorema che caratterizza l'intersezione binaria, Z ∈ X (H2) e Z ∈ Y (H3). |
|                                                                        | Per H2 Z ∈ X.                                                                            |
|                                                                        |                                                                                          |
|                                                                        | Qed.                                                                                     |

# Esercizio 4

> Teorema: se X ⊆ Y allora X ∪ Y = Y
> 
> (Simboli utilizzabili: ∈ ∅ ∪ ∩ ⊆ ∀ ∃ ∧ ∨ ¬ ⇒ ⇔)

| Mio/Nostro | Prof    |
| -:         | :-      |
| Siano X, Y insiemi tali che X ⊆ Y,                                                  | Siano X, Y insiemi t.c. X ⊆ Y,                                                     |
| ovvero ∀Z . Z ∈ X ⇒ Z ∈ Y (H1).                                                     | ovvero ∀Z. Z ∈ X ⇒ Z ∈ Y (H1).                                                     |
| Debbo dimostrare X ∪ Y = Y.                                                         | Dobbiamo dimostrare X ∪ Y = Y.                                                     |
| Per l'assioma dell'estensionalità ci riduciamo a dimostrare ∀Z . Z ∈ X ∪ Y ⇔ Z ∈ Y. | Per l'assioma di estensionalità, ci riduciamo a dimostrare ∀Z. Z ∈ X ∪ Y ⇔ Z ∈ Y.  |
| Sia Z un insieme.                                                                   | Sia Z insieme.                                                                     |
| Procedo per casi                                                                    |                                                                                    |
| - Z ∈ X ∪ Y ⇒ Z ∈ Y:                                                                | Dimostriamo Z ∈ Y ⇒ Z ∈ X ∪ Y.                                                     |
| Suppongo Z ∈ X ∪ Y, per l'assioma dell'unione binaria Z ∈ X (H2) oppure Z ∈ Y (H3). | Assumiamo Z ∈ Y (H2).                                                              |
| Procedo per casi                                                                    | Per l'assioma dell'unione binaria ci riduciamo a dimostrare Z ∈ X ∨ Z ∈ Y.         |
| - Suppongo valga H2, Z ∈ X                                                          | Dimostro Z ∈ Y. Ovvio per H2.                                                      |
| Debbo dimostrare Z ∈ Y, ovvio per H2 e H1 (Per H2 Z ∈ X, per H1 Z ∈ Y)              |                                                                                    |
| - Suppongo valga H3, Z ∈ Y                                                          | Dimostriamo Z ∈ X ∪ Y ⇒ Z ∈ Y.                                                     |
| Debbo dimostrare Z ∈ Y, ovvio per H3.                                               | Assumiamo Z ∈ X ∪ Y.                                                               |
| - Z ∈ Y ⇒ Z ∈ X ∪ Y:                                                                | Quindi, per l'assioma dell'unione binaria, Z ∈ X o Z ∈ Y (H2).                     |
| Suppongo Z ∈ Y (H2).                                                                | Dobbiamo dimostrare Z ∈ Y. Procedo per casi su H2.                                 |
| Debbo dimostrare Z ∈ X ∪ Y, ovvero Z ∈ X oppure Z ∈ Y.                              | Caso Z ∈ X (H3). Ovvio per H3 e H1.                                                |
| Ovvio per H2.                                                                       | Caso Z ∈ Y (H3). Ovvio per H3.                                                     |
| Qed.                                                                                |                                                                                    |
|                                                                                     | Qed.                                                                               |

# Esercizio 5

> Teorema: se X ∪ Y = Y allora X ⊆ Y
> 
> (Simboli utilizzabili: ∈ ∅ ∪ ∩ ⊆ ∀ ∃ ∧ ∨ ¬ ⇒ ⇔)

| Mio/Nostro                                                            | Prof                                                                    |
| -:                                                                    | :-                                                                      |
| Siano X, Y insiemi tali che X ∪ Y = Y.                                | Siano X, Y insiemi t.c. X ∪ Y = Y.                                      |
| Per l'assioma dell'estensionalità ∀Z . Z ∈ X ∪ Y ⇔ Z ∈ Y (H1)         | Quindi, per l'assioma di estensionalità, ∀Z. (Z ∈ X ∪ Y ⇔ Z ∈ Y) (K).   |
| Per l'assioma dell'unione binaria ∀Z . Z ∈ X ∪ Y ⇔ Z ∈ X ∨ Z ∈ Y (H2) | Dobbiamo dimostrare X ⊆ Y, ovvero ∀Z. (Z ∈ X ⇒ Z ∈ Y).                  |
| Debbo dimostrare che X ⊆ Y, ovvero ∀Z . Z ∈ X ⇒ Z ∈ Y                 | Sia Z un insieme t.c. Z ∈ X (H).                                        |
| Sia Z insieme                                                         | Dobbiamo dimostrare Z ∈ Y.                                              |
| Per H2 Z ∈ X ⇒ Z ∈ X ∪ Y.                                             | Per K mi riduco a dimostrare Z ∈  X ∪ Y.                                |
| Per H1 Z ∈ X ∪ Y ⇒ Z ∈ Y.                                             | Per l'assioma dell'unione binaria mi riduco a dimostrare Z ∈ X ∨ Z ∈ Y. |
| qed                                                                   | Dimostro Z ∈ X. Ovvio per H.                                            |
|                                                                       | Qed.                                                                    |

---