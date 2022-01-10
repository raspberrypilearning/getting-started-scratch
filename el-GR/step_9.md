## Συμβάντα

Τα μπλοκ στο μενού `Συμβάντα`{:class="block3events"} ελέγχουν πότε ξεκινούν τα scripts.

Τα **μπλοκ Καπέλα** εκτελούν τα μπλοκ κάτω από αυτά όταν συμβαίνει ένα συγκεκριμένο συμβάν. Είναι στρογγυλεμένα στο επάνω μέρος, σαν καπέλο, οπότε κανένα μπλοκ δεν μπορεί να πάει από πάνω τους.

Μπορείς να χρησιμοποιήσεις:

```blocks3

when flag clicked // run blocks when the green flag above the Stage is clicked

when this sprite clicked // run the blocks when the sprite for this script is clicked

when stage clicked // run the blocks when the stage is clicked

```

**Συμβουλή:** Το μπλοκ `όταν γίνει κλικ στο σκηνή`{:class="block3events"} είναι διαθέσιμο μόνο όταν εργάζεσαι στην περιοχή Κώδικας για τη Σκηνή.

Εάν χρησιμοποιείς υπολογιστή με πληκτρολόγιο, μπορείς να χρησιμοποιήσεις το `όταν πατηθεί το πλήκτρο`{:class="block3events"}:

```blocks3
when [space v] key pressed // change to number, letter or arrow keys
```

Μπορείς επίσης να χρησιμοποιήσεις το μπλοκ `όταν το υπόβαθρο αλλάξει σε`{:class="block3events"} για να ξεκινήσει ένα script όταν αλλάζει το υπόβαθρο.

[[[scratch3-changing-backdrops-pages-levels]]]

[[[scratch3-show-hide-sprites-backdrops]]]


Το μπλοκ `όταν >`{:class="block3events"} έχει δύο εκδόσεις:

```blocks3
when [loudness v] > (10) // run blocks when the microphone detects sound

when [timer v] > (10) // run blocks when the timer reaches 10 seconds
```

[[[scratch3-time-delay]]]


Τα δύο τελευταία μπλοκ στο μενού `Συμβάντα`{:class="block3events"} είναι `μπλοκ μετάδοσης`{:class="block3events"}. Μπορείς να χρησιμοποιήσεις το `όταν λάβω (μήνυμα v)`{:class="block3events"} για να ξεκινήσεις ένα script όταν οποιοδήποτε αντικείμενο εκτελεί το αντίστοιχο μπλοκ `μετάδωσε (μήνυμα v)`{:class="block3events"}.

[[[generic-scratch3-broadcast-message]]]

