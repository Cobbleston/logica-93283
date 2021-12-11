# Logica appunti veloci

Siano X, X', Y insiemi tali che X ⊆ X'.

Ovvero ∀Z, Z ∈ X ⇒ Z ∈ X' (H)

Debbo dimostrare X × Y ⊆ X' × Y, 

Ovvero ∀Z, Z ∈ X × Y ⇒ Z ∈ X' × Y,

Sia Z insieme tale che Z ∈ X × Y$,

Ovvero ∃a ∈ X, ∃b ∈ Y . Z = ⟨a, b⟩

Debbo dimostrare Z ∈ X' × Y,

Ovvero ∃a' ∈ X', ∃b' ∈ Y . Z = ⟨a', b'⟩

Scelgo a, b. Ovvio per H

---

Sia A insieme e f, g funzioni tali che f ∈ A^A (H1) e g ∈ A^A (H2) e f iniettiva (H3) e g iniettiva (H4)

Per H3 ∀x, y ∈ A, (f(x) = f(y) ⇒ x = y) (H3')
Per H4 ∀x, y ∈ A, (g(x) = g(y) ⇒ x = y) (H4')

Devo dimostrare ∀x, y ∈ A, (f(g(x)) = f(g(y)) ⇒ x = y)

Siano x, y ∈ A tali che f(g(x)) = f(g(y))
Per H3 g(x) = g(y)
Per H4 x = y
qed.

---

Siano W, X, Y insiemi tali che W ∈ X × Y ∩ Y × X.

Ovvero, per il teorema dell'intersezione binaria, W ∈ X × Y ∧ W ∈ Y × X

Devo dimostrare che X ∪ Y ≠ ∅

