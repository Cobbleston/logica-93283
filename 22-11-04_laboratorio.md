Siano X, Y, Z insiemi.

Devo dimostrare X ∪ (Y ∩ Z) ⊆ (X ∪ Y) ∩ (X ∪ Z).

Ovvero ∀W . W ∈ X ∪ (Y ∩ Z) ⟹ W ∈ (X ∪ Y) ∩ (X ∪ Z)

Sia W insieme tale che W ∈ X ∪ (Y ∩ Z)

Quindi, per il teorema dell'unione binaria, W ∈ X (H1) ∨ W ∈ Y ∩ Z (H2).

Quindi, per H2 e teorema dell'intersezione binaria, W ∈ Y (H3) ∧ W ∈ Z (H4).

Devo dimostrare W ∈ (X ∪ Y) ∩ (X ∪ Z)

Ovvero, per teorema dell'intersezione binaria, W ∈ X ∪ Y ∧ W ∈ X ∪ Z.

Ovvero, per il teorema dell'unione binaria, (W ∈ X ∨ W ∈ Y) ∧ (W ∈ X ∨ W ∈ Z)

Procedo a dimostrare per casi:

Caso W ∈ X (H1):
    Devo dimostrare (W ∈ X o W ∈ Y) e (W ∈ X o W ∈ Z).
    W ∈ X o W ∈ Y ovvio per H1.
    W ∈ X o W ∈ Z ovvio per H1.

Caso W ∈ Y (H3) ∧ W ∈ Z (H4):
    Devo dimostrare (W ∈ X o W ∈ Y) e (W ∈ X o W ∈ Z).
    W ∈ X o W ∈ Y ovvio per H3.
    W ∈ X o W ∈ Z ovvio per H4.

Qed.

---
---
---

# Esercizio 3

```
Funzioni:

filter(f,[]) = [] 
filter(f,X::L) = if f(X) then X::filter(f,L) else filter(f,L) 

map(f,[]) = [] 
map(f,X::L) = f(X)::map(f,L) 
```
Dimostrare, per induzione strutturale su L, che per ogni f, g si ha

`filter(f, map(g, L)) = map(g, filter(f ◦ g, L))`

dove la funzione composta f ◦ g è definita nel modo usuale, ovvero

`(f ◦ g)(x) = f(g(x))$$`

---
### Soluzione
Dimostro per induzione strutturale su L che per ogni f, g si ha

`filter(f, map(g, L)) = map(g, filter(f ◦ g, L))`

### Caso `[]`:

Devo dimostrare

`∀f,g . filter(f, map(g, [])) = map(g, filter(f ◦ g, []))`

Ovvero

`∀f,g . filter(f, []) = map(g, [])`

Ovvero

`∀f,g . [] = []`

Ovvio.

### Caso `x :: l`:

Suppongo per ipotesi induttiva

`∀f,g . filter(f, map(g, l)) = map(g, filter(f ◦ g, l)) (II)`

Devo dimostrare

`∀f,g . filter(f, map(g, (x :: l))) = map(g, filter(f ◦ g, (x ::l)))`

Ovvero

`∀f,g . filter(f, g(x) :: map(g, l)) = map(g, (if f(g(x)) then x:: filter(f ◦ g, l) else filter(f ◦ g, l)))`

Ovvero

`∀f,g . if f(g(x)) then g(x) :: filter(f, map(g, l)) else filte(f, map(g, l)) = map(g, (if f(g(x)) then x :: filter(f ◦ g, l)else filter(f ◦ g, l)))`

Siano f, g funzioni. Procedo per casi:

### Caso `f(g(x)) = true (H)`:

Devo dimostrare

`g(x) :: filter(f, map(g, l)) = map(g, x :: filter(f ◦ g, l))`

Ovvero

`g(x) :: filter(f, map(g, l)) = g(x) :: map(g, (filter(f ◦g, l)))`

Ovvero 

`filter(f, map(g, l)) = map(g, (filter(f ◦ g, l)))`

Per `(II)` mi riduco a dimostrare

`filter(f, map(g, l)) = filter(f, map(g, l))`

Ovvio.

### Caso `f(g(x)) = false (H)`:

Devo dimostrare

`filter(f, map(g, l)) = map(g, filter(f ◦ g, l))`

Per (II) mi riduco a dimostrare

`filter(f, map(g, l)) = filter(f, map(g, l))`

Ovvio.

Qed.