# Robuino

**Ομάδα ρομποτικής 8ου Γυμνασίου Περιστερίου**

**To Προτεινόμενο Έργο μας για το 1ο Πανελλήνιο Διαγωνισμό Εκπαιδευτικής Ρομποτικής & Physical Computing Ανοιχτών Τεχνολογιών**

Η πρότασή μας περιλαμβάνει τη δημιουργία/προγράμματος παιχνιδιού (σε προγραμματιστικό περιβάλλον Scratch 2.00 με εγκατεστημένη την επέκταση s2aio με AGPL-3.0) καθώς και αντίστοιχου χειριστηρίου μέσω του οποίου θα παίζεται το παιχνίδι (με χρήση Arduino uno). Το παιχνίδι περιλαμβάνει αεροπλάνο το οποίο θα κινείται δεξιά αριστερά στη σκηνή με τη περιστροφή του **ποτενσιομέτρου** το οποίο θα υπάρχει στο κύκλωμα του χειριστηρίου. Στόχος μας είναι η αποφυγή της σύγκρουσης με εχθρικό αεροπλάνο που έρχεται από την αντίθετη κατεύθυνση. Κατά την έναρξη του παιχνιδιού στο χειριστήριο θα είναι αναμμένα τρία λαμπάκια (**leds**) που δείχνουν ότι έχουμε τρεις ζωές. Με απώλειά κάθε ζωής (σύγκρουση με εχθρικό αεροπλάνο) θα σβήνει και από ένα λαμπάκι στο χειριστήριο ενώ παράλληλα θα ακούγεται και ήχος από **piezo buzzer**. Όταν σβήσουν όλα τα λαμπάκια (απώλεια όλων των ζωών) το παιχνίδι θα τερματίζεται. 

Στο χειριστήριο επιπλέον θα υπάρχουν δύο πλήκτρα (buttons): 

• με πάτημα στο **ένα πλήκτρο (button1)** θα μπορεί το αεροπλάνο μας να πυροβολεί προς το εχθρικό αεροπλάνο και όταν τα πυρά μας το πετυχαίνουν θα κερδίζουμε 20 πόντους οπότε το σκορ μας θα αυξάνεται

• με πάτημα **στο δεύτερο πλήκτρο (button2)** θα αυξάνεται ο βαθμός δυσκολίας του παιχνιδιού με εμφάνιση δύο εχθρικών αεροπλάνων ταυτόχρονα.

Παρακάτω εικονίζονται:

**α)** Στην εικόνα 1 το παράθυρο του Scratch 2.0 με εγκατεστημένη την επέκταση s2aio (https://github.com/MrYsLab/s2aio/wiki). Στο παράθυρο φαίνεται η σκηνή επί της οποίας βλέπουμε το αεροπλάνο μας (κόκκινο/πορτοκαλί) καθώς και εχθρικό αεροπλάνο (πράσινο/λευκό) επίσης διακρίνεται και τμήμα από τον κώδικα του παιχνιδιού.

**Εικόνα 1**
![Github Robuino](/plane-project.png)
                                                       

**β)** Στην εικόνα 2, το κύκλωμα από το χειριστήριο με χρήση Arduino uno: 

**Εικόνα 2**
![Github Robuino](/circuit.png)
                                                           

Για το κύκλωμα του χειριστηρίου, όπως φαίνεται στην εικόνα απαιτούνται τα εξής υλικά:

• 1 board Arduino uno

• 1 Breadboard για τη δημιουργία κυκλώματος

• 3 Αντιστάσεις 220 Ω

• 2 Αντιστάσεις 10 ΚΩ

• 3 κόκκινα leds (5mm)

• 1 περιστροφικό ποτενσιόμετρο

• 2 buttons (διακόπτες)

• 1 piezo buzzer 


**Λογισμικό**

 Το Arduino uno του παραπάνω κυκλώματος συνδέεται στη usb θύρα υπολογιστή (με λειτουργικό σύστημα κατά προτίμηση linux Ubuntu/ελεύθερο και ανοικτό λογισμικό) στόν οποίο είναι εγκατεστημένο το περιβάλλον οπτικού προγραμματισμού Scratch 2.0 με την επέκταση s2aio, και στο οποίο θα έχει φορτωθεί το προς εκτέλεση πρόγραμμα του παιχνιδιού. Εναλλακτικά η πρόταση θα μπορούσε να υλοποιηθεί με το λογισμικό S4A (http://s4a.cat/).
 
 **Ο σκοπός και η ένταξη της πρότασης στο πρόγραμμα σπουδών / Πρότερες και Προαπαιτούμενες γνώσεις των μαθητών / Τρόπος οργάνωσης** 

Θεωρούμε ότι η πρότασή μας είναι συμβατή με το γνωστικό επίπεδο των μαθητών, διότι:

**α)** Όσον αφορά το προγραμματιστικό τμήμα του έργου, οι μαθητές, είναι ήδη εξοικειωμένοι με το περιβάλλον του Scratch 2.0. Η μόνη διαφοροποίηση, συναντάται στην παλέτα εντολών **«Άλλες εντολές»** στην οποία έχουν προστεθεί εντολές οι οποίες αφορούν στην επικοινωνία με την πλακέτα του Arduino μέσω των ψηφιακών και αναλογικών εισόδων/εξόδων. Για την διδασκαλία αυτών των νέων εντολών σχετικά με το προγραμματισμό του Arduino, και την εξοικείωσή τους με την κατασκευή απλών κυκλωμάτων, οι μαθητές θα υλοποιήσουν φύλλα εργασίας με δραστηριότητες κατάλληλες ώστε να οικοδομήσουν τις απαραίτητες γνώσεις και ν’ αποκτήσουν τις κατάλληλες δεξιότητες που θα τους οδηγήσουν στην υλοποίηση του τελικού τους έργου.

**β)** ήδη, έχουν προσεγγίσει τις βασικές έννοιες του ηλεκτρισμού στο μάθημα της Φυσικής και την δημιουργία απλών ηλεκτρικών κυκλωμάτων.

Για την υλοποίηση της πρότασης αυτής προτείνεται μια εναλλακτική προσέγγιση της διδασκαλίας των βασικών αρχών του προγραμματισμού, εννοιών της Φυσικής (απλά ηλεκτρικά κυκλώματα, νόμος ohm), απλών μαθηματικών, με παιγνιώδη τρόπο, χρησιμοποιώντας την πλακέτα Arduino και τη γλώσσα προγραμματισμού Scratch 2.0 (με εγκατεστημένη την επέκταση s2aio για Arduino).

Μέσω συνεργατικής μάθησης θα αναπτυχθούν στους μαθητές ειδικές δεξιότητες, όπως η ανάληψη ρόλων και αρμοδιοτήτων, η υπευθυνότητα, η παρατήρηση, η συνομιλία, η συν-κατασκευή της γνώσης, ο σεβασμός,κ.ά.. Με αυτή τη προσέγγιση, οι μαθητές θα κατασκευάσουν κύκλωμα (χειριστήριο) και θα προγραμματίσουν, συνδυάζοντας όπως αναφέραμε παραπάνω, γνώσεις και δεξιότητες από διαφορετικά γνωστικά αντικείμενα. 

Σκοπός μας είναι να αισθανθούν οι μαθητές εκτός από απλοί χρήστες και καταναλωτές της τεχνολογίας, ότι μπορούν να είναι και οι ίδιοι δημιουργοί. Θεωρούμε ότι η εμπλοκή των μαθητών θα είναι ισχυρή, αφού στο πλαίσιο διδασκαλίας θα τροφοδοτούνται από θέματα που θα έχουν άμεσο ενδιαφέρον γι’ αυτούς.

Ο ρόλος του εκπαιδευτικού θα είναι ο συντονιστικός και η καθοδηγητικός των μαθητών προκειμένου να οικοδομήσουν την γνώση και ολοκληρώσουν το έργο τους. Είναι σημαντικό να εξηγεί στους μαθητές και να ενισχύει τους κανόνες και τις κοινωνικές δεξιότητες της συνεργατικής μάθησης, να αναπτύσσει την υπευθυνότητα των μαθητών και να τους διδάσκει πώς να μαθαίνουν. Ως καθοδηγητής θα πρέπει να φροντίσει να μην δίνει έτοιμες απαντήσεις, αλλά να δημιουργεί κατάλληλες μαθησιακές καταστάσεις και προβληματισμούς ώστε οι ίδιοι οι μαθητές ν’ ανακαλύπτουν την λύση. Επίσης, ο εκπαιδευτικός οφείλει να επαινεί και να ενθαρρύνει κάθε προσπάθεια που γίνεται καθώς και να ωθεί τους μαθητές στην έρευνα και τον προβληματισμό και εκτός της σχολικής αίθουσας.
Στην επίτευξη των παραπάνω θα συμβάλλει η αξιοποίηση πλατφόρμας **Μoodle** εγκατεστημένης στο Πανελλήνιο Σχολικό Δίκτυο.
