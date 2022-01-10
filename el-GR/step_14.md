## Οι Εντολές μου

`Οι Εντολές μου`{:class="block3myblocks"} σου επιτρέπουν να δημιουργήσεις νέα μπλοκ για ένα αντικείμενο. Δίνεις ένα όνομα στο μπλοκ και μετά `ορίζεις`{:class="block3myblocks"} τι κάνει το νέο μπλοκ χρησιμοποιώντας άλλα μπλοκ Scratch. Μπορείς να χρησιμοποιήσεις το νέο σου μπλοκ σε οποιοδήποτε σενάριο στο αντικείμενο στο οποίο ανήκει το μπλοκ.

Αυτό το παράδειγμα ορίζει ένα μπλοκ `ομιλία`{:class="block3myblocks"} που κάνει μία αλλαγή ενδυμασίας σε ένα αντικείμενο:

**Ο πιγκουίνος τιτιβίζει**: [Δες μέσα](https://scratch.mit.edu/projects/567554899/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567554899/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define talk
switch costume to (penguin2-b v)
repeat (2)
play sound (chirp v) until done
end
switch costume to (penguin2-a v)

when this sprite clicked
talk

when [space v] key pressed
talk
```

Μπορείς να χρησιμοποιήσεις την κατηγορία `Οι Εντολές μου`{:class="block3myblocks"} για να **οργανώσεις** τον κώδικά σου. Είναι πιο απλό να ομαδοποιήσεις όλα τα μπλοκ που κάνουν ένα αντικείμενο να μιλάει και, στη συνέχεια, απλώς να χρησιμοποιήσεις ένα μπλοκ `ομιλία`{:class="block3myblocks"} όταν θέλεις να μιλήσει το αντικείμενό σου.

Εάν αποφασίσεις ότι θέλεις να αλλάξεις τον τρόπο με τον οποίο μιλάει το αντικείμενό σου, τότε δεν έχεις παρά να αλλάξεις τον κώδικα σε ένα σημείο.

### Οι Εντολές μου με εισόδους

Μπορείς επίσης να προσθέσεις **εισόδους** στο `Οι Εντολές μου`{:class="block3myblocks"} ώστε να χρησιμοποιούν τις τιμές που δίνεις όταν χρησιμοποιείς το μπλοκ.

**Ο πιγκουίνος τιτιβίζει**: [Δες μέσα](https://scratch.mit.edu/projects/567538874/editor){:target="_blank"}

<div class="scratch-preview">
  <iframe src="https://scratch.mit.edu/projects/567538874/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
</div>

```blocks3
define talk (words)
switch costume to (penguin2-b v)
say (words) // use the provided input
repeat (2)
play sound (chirp v) until done
end
say (words)
switch costume to (penguin2-a v)

when this sprite clicked
talk [hello]

when [space v] key pressed
talk [hi]
```

[[[generic-scratch3-make-block]]]

--- collapse ---
---
title: Χρησιμοποίησε τις Εντολές μου για να οργανώσεις τον κώδικα
---
Ο απλούστερος λόγος για να χρησιμοποιηθούν `Οι Εντολές μου`{:class="block3myblocks"} είναι για να βοηθηθείς στην οργάνωση του κώδικά σου. Εδώ είναι ένα απλό παράδειγμα.

```blocks3
define move right
if <not <touching (edge v) ?>> then
switch costume to [right_1 v]
change x by (2)
switch costume to [right_2 v]
change x by (2)
switch costume to [right_3 v]
change x by (2)
end

define move left
if <not <touching (edge v) ?>> then
switch costume to [left_1 v]
change x by (-2)
switch costume to [left_2 v]
change x by (-2)
switch costume to [left_3 v]
change x by (-2)
end

when flag clicked
forever
if <key (right arrow v) pressed> then
move right
end
if <key (left arrow v) pressed> then
move left
```

--- /collapse ---

`Οι Εντολές μου`{:class="block3myblocks"} είναι παρόμοιες με τις 'διαδικασίες', 'συναρτήσεις' ή 'μεθόδους' σε άλλες γλώσσες προγραμματισμού.
