## Κίνηση

Τα μπλοκ `Κίνηση `{:class="block3motion"} σου επιτρέπουν να μετακινείς το αντικείμενό σου στη Σκηνή.

### Κίνηση

Το μπλοκ `κινήσου`{:class="block3motion"} είναι ο απλούστερος τρόπος για να ξεκινήσεις τη μετακίνηση ενός αντικειμένου:

```blocks3
move [10] steps
```

Μπορείς να χρησιμοποιήσεις τα μπλοκ `πήγαινε σε`{:class="block3motion"} ή `ολίσθησε στη θέση`{:class="block3motion"} δείκτη ποντικιού, μια τυχαία θέση στη Σκηνή (ή το δάχτυλό σας σε ένα tablet) ή σε άλλο αντικείμενο:

```blocks3
go to (random position v)

glide [1] secs to (random position v)
```

Μπορείς επίσης να χρησιμοποιήσεις τα μπλοκ `πήγαινε σε`{:class="block3motion"} ή `ολίσθησε στη θέση`{:class="block3motion"} σε μια θέση που δίνεται από τις `x`{:class="block3motion"} και τις `y`{:class="block3motion"} Συντεταγμένες στη Σκηνή.

```blocks3
go to x: [0] y: [0] 

glide [1] secs to x: [0] y: [0]
```

[[[scratch3-glide-to-object]]]

**Συμβουλή:** Όταν σύρεις ένα αντικείμενο στη Σκηνή, τα μπλοκ κίνησης που χρησιμοποιούν συντεταγμένες `x`{:class="block3motion"} και `y`{:class="block3motion"} ενημερώνουν το μενού μπλοκ `Κίνηση`{: class="block3motion"}. Οι τρέχουσες συντεταγμένες `x`{:class="block3motion"} και `y`{:class="block3motion"} εμφανίζονται στο παράθυρο Sprite.

### Περιστροφή
Μπορείς επίσης να αλλάξεις την `κατεύθυνση `{:class="block3motion"} προς την οποία κοιτάει ένα αντικείμενο. Αυτό αλλάζει την κατεύθυνση προς την οποία θα κινηθεί το αντικείμενο εάν χρησιμοποιήσεις ένα μπλοκ `κινήσου`{:class="block3motion"}. Μπορεί επίσης να αλλάξει την περιστροφή της ενδυμασίας του αντικειμένου ανάλογα με τη ρύθμιση `τρόπος-περιστροφής`{:class="block3motion"}.

Όταν προσθέτεις ένα αντικείμενο, θα είναι στραμμένο προς τα δεξιά (90 μοίρες). Μπορείς να το αλλάξεις στο παράθυρο Αντικείμενα ή χρησιμοποιώντας μπλοκ κώδικα.

```blocks3
turn right [15] degrees

turn left [15] degrees

point in direction [90] // Click on 90 and drag the arrow to change

point towards (mouse-pointer v)

(direction)

set rotation style [left-right v] // or all-around or none
```

[[[scratch3-sprite-direction]]]

[[[scratch3-left-right-direction]]]

--- collapse ---
---
title: Περιστροφή
---

--- no-print ---

**Περιστρεφόμενη νυχτερίδα **: [Δες μέσα](https://scratch.mit.edu/projects/435704980/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435704980/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Αυτός ο κώδικας κάνει ένα αντικείμενο να περιστρέφεται όταν γίνει κλικ στην πράσινη σημαία:

```blocks3
when flag clicked
forever
turn right (1) degrees :: motion
```

Σε ένα μπλοκ `στρίψε`{:class="block3motion"} μέσα σε ένα βρόχο `για πάντα`{:class="block3control"}, άλλαξε τον αριθμό των μοιρών σε `1` και το αντικείμενό σου θα εμφανιστεί να περιστρέφεται.

**Συμβουλή:** Εάν δεν προσθέσεις ένα μπλοκ `κινήσου`{:class="block3motion"}, το αντικείμενό σου σας θα περιστραφεί στη θέση που βρίσκεται.

--- /collapse ---

--- collapse ---
---
title: Κίνηση σε κύκλο
---

--- no-print ---

**Τροχιά σελήνης**: [Δες μέσα](https://scratch.mit.edu/projects/435701055/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/435701055/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Αυτός ο κώδικας κάνει ένα αντικείμενο να πετάει σε κύκλο όταν γίνει κλικ στην πράσινη σημαία:

```blocks3
when green flag clicked
forever
move (1) steps
turn right (1) degrees :: motion
```

Άλλαξε τις τιμές σε ένα μπλοκ `κινήσου`{:class="block3motion"} και σε ένα μπλοκ `στρίψε`{:class="block3motion"}μέσα σε ένα βρόχο`για πάντα`{:class="block3control"} σε `1` και το αντικείμενο θα φαίνεται να κινείται σε μεγάλο κύκλο.

**Συμβουλή:** Εάν θέλεις το αντικείμενό σου να ξεκινά πάντα στο κέντρο του Σκηνικού, μπορείς να προσθέσεις ένα μπλοκ `πήγαινε σε θέση x:`{:class="block3motion"} `0` `y:`{:class="block3motion "} `0` πριν από το μπλοκ `για πάντα`{:class="block3control"}.

--- /collapse ---

### Αναπήδηση

Το μπλοκ `εάν σε όριο, αναπήδησε`{:class="block3motion"} είναι πολύ χρήσιμο όταν θέλεις να κάνεις ένα αντικείμενο να αναπηδά και να παραμένει στη Σκηνή:

```blocks3
if on edge, bounce
```

Δες μερικούς από τους τρόπους με τους οποίους μπορείς να κάνεις το αντικείμενό σου να αναπηδήσει:

--- collapse ---
---
title: Αναπήδηση σε όλη τη σκηνή
---

--- no-print ---

**Κορίτσι κινείται στη Σκηνή**: [Δες μέσα](https://scratch.mit.edu/projects/433535326/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433535326/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Αυτός ο κώδικας κάνει ένα αντικείμενο να αναπηδά στην αριστερή και δεξιά πλευρά της Σκηνής. Επειδή το αντικείμενο περιστρέφεται οριζόντια, φαίνεται να αναστρέφεται όταν αλλάζει η κατεύθυνσή του όταν γίνει κλικ στην πράσινη σημαία:

```blocks3
when green flag clicked
point in direction (90)
set rotation style [left-right v]
forever
move (5) steps
if on edge, bounce
```

Σε αυτό το παράδειγμα, το μπλοκ `δείξε προς κατεύθυνση`{:class="block3motion"} στρέφει αυτόματα το αντικείμενο προς τα δεξιά (`90` μοίρες) όταν γίνει κλικ στην πράσινη σημαία. Εάν αλλάξεις τον αριθμό των μοιρών σε `-90`, το αντικείμενό σου θα στραφεί προς τα αριστερά.

Πρόσθεσε ένα μπλοκ `όρισε τρόπο περιστροφής`{:class="block3motion"} και επίλεξε `αριστερά-δεξιά`{:class="block3motion"} στο αναπτυσσόμενο μενού, έτσι ώστε το αντικείμενό σου να μην αναποδογυρίζει όταν αναπηδά στην άκρη της Σκηνής.

**Συμβουλή:** Μπορείς να σύρεις το αντικείμενό σου στη Σκηνή για να το μετακινήσεις στη θέση y (πάνω-κάτω) που θέλεις.

--- /collapse ---

--- collapse ---
---
title: Αναπήδηση πάνω και κάτω στη Σκηνή
---

--- no-print ---

**Το κορίτσι που αναπηδά**: [Δες μέσα](https://scratch.mit.edu/projects/433595822/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433595822/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Αυτός ο κώδικας κάνει ένα αντικείμενο να αναπηδά πάνω και κάτω στη Σκηνή όταν γίνει κλικ στην πράσινη σημαία:

```blocks3
when green flag clicked
point in direction (0)
set rotation style [don't rotate v]
forever
move (5) steps
if on edge, bounce
```

Άλλαξε τον αριθμό των μοιρών στο μπλοκ `δείξε προς κατεύθυνση`{:class="block3motion"} σε `0` για να κάνεις ένα αντικείμενο να δείχνει προς τα πάνω.

Πρόσθεσε ένα μπλοκ `όρισε τρόπο περιστροφής`{:class="block3motion"} και επίλεξε `μην περιστρέψεις`{:class="block3motion"} στο αναπτυσσόμενο μενού, έτσι ώστε το αντικείμενό σου να σταματήσει να αναστρέφεται, ακόμα και όταν αναπηδά.

**Συμβουλή:** Μπορείς να σύρεις το αντικείμενό σου στη Σκηνή για να το μετακινήσεις στη θέση x (αριστερά-δεξιά) που θέλεις.

--- /collapse ---

--- collapse ---
---
title: Αναπήδηση υπό γωνία
---

--- no-print ---

**Η μπάλα ποδοσφαίρου που αναπηδά**: [Δείτε μέσα](https://scratch.mit.edu/projects/433536479/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/433536479/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

--- /no-print ---

Αυτός ο κώδικας κάνει ένα αντικείμενο να φαίνεται ότι περιστρέφεται τυχαία όταν γίνει κλικ στην πράσινη σημαία:

```blocks3
when green flag clicked
point in direction (45)
set rotation style [all around v]
forever
move (5) steps
if on edge, bounce
```

Εάν το αντικείμενό σου κινηθεί στις `45` μοίρες, θα διαπιστώσεις ότι φαίνεται να αναπηδά στην άκρη της Σκηνής υπό γωνία. Άλλαξε τον αριθμό των μοιρών στο μπλοκ `δείξε προς κατεύθυνση`{:class="block3motion"} σε `45` για να κάνεις το αντικείμενό σου να αναπηδά τριγύρω.

Πρόσθεσε ένα μπλοκ `όρισε τρόπο περιστροφής`{:class="block3motion"} και επίλεξε `τριγύρω`{:class="block3motion"} στο αναπτυσσόμενο μενού, έτσι ώστε το αντικείμενό σου να στρίβει όταν αναπηδά στην άκρη της Σκηνής.

--- /collapse ---

### Χρήση συντεταγμένων

Μπορείς επίσης να `αλλάξεις `{:class="block3motion"} και να `ορίσεις`{:class="block3motion"} τις συντεταγμένες `x`{:class="block3motion"} και `y`{:class="block3motion"} και χρησιμοποιήσεις τις τιμές τους σε άλλα μπλοκ:

[[[generic-scratch3-coordinates]]]

```blocks3 
change x by [10]

set x to [0]

change y by  [10]

set y to [0]

(x position)

(y position)
```

--- collapse ---
---
title: Δεν μπορώ να δω τα μπλοκ Κίνησης
---

Εάν έχεις επιλέξει τη Σκηνή, τότε δεν θα δεις μπλοκ `Κίνηση`{:class="block3motion"}, επειδή η Σκηνή δεν μπορεί να μετακινηθεί.

Κάνε κλικ σε ένα αντικείμενο στο παράθυρο Αντικείμενα και στη συνέχεια κάνε κλικ στην καρτέλα **Κώδικας** για να δεις τα μπλοκ `Κίνηση`{:class="block3motion"}.

--- /collapse ---

