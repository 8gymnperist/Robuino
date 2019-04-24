# Robuino

## Ομάδα ρομποτικής 8ου Γυμνασίου Περιστερίου

**Τα μέλη της ομάδας αποτελούν οι  μαθητές της Γ’ τάξης:**

**Κεφαλάς Αλέξανδρος – Μανουσάκης Γιάννης – Μίγκος Δημήτρης**

Διδάσκοντες / Σύμβουλοι Εκπαιδευτικοί:
 
Καλοδίκης Ανδρέας (ΠΕ86-Πληροφορικής) & Μουρελάτου Ζαχαρούλα (ΠΕ82-Μηχανολόγος)


### To Προτεινόμενο Έργο μας για το 1ο Πανελλήνιο Διαγωνισμό Εκπαιδευτικής Ρομποτικής & Physical Computing Ανοιχτών Τεχνολογιών

Η πρότασή μας περιλαμβάνει τη δημιουργία/προγράμματος παιχνιδιού (σε προγραμματιστικό περιβάλλον Scratch 2.0 με εγκατεστημένη την επέκταση s2aio) καθώς και αντίστοιχου χειριστηρίου μέσω του οποίου θα παίζεται το παιχνίδι (με χρήση Arduino uno). Το παιχνίδι περιλαμβάνει αεροπλάνο το οποίο θα κινείται δεξιά και αριστερά στη σκηνή με τη περιστροφή του **ποτενσιομέτρου** το οποίο θα υπάρχει στο κύκλωμα του χειριστηρίου. Στόχος μας είναι η αποφυγή της σύγκρουσης με εχθρικό αεροπλάνο που έρχεται από την αντίθετη κατεύθυνση. Κατά την έναρξη του παιχνιδιού στο χειριστήριο θα είναι αναμμένα τρία λαμπάκια (**leds**) που δείχνουν ότι έχουμε τρεις ζωές. Με απώλειά κάθε ζωής (σύγκρουση με εχθρικό αεροπλάνο) θα σβήνει και από ένα λαμπάκι στο χειριστήριο ενώ παράλληλα θα ακούγεται και ήχος από **piezo buzzer**. Όταν σβήσουν όλα τα λαμπάκια (απώλεια όλων των ζωών) το παιχνίδι θα τερματίζεται. 

Στο χειριστήριο επιπλέον θα υπάρχουν δύο πλήκτρα (buttons): 

• με πάτημα στο **ένα πλήκτρο (button1)** θα μπορεί το αεροπλάνο μας να πυροβολεί προς το εχθρικό αεροπλάνο και όταν τα πυρά μας το πετυχαίνουν θα κερδίζουμε 20 πόντους οπότε το σκορ μας θα αυξάνεται

• με πάτημα **στο δεύτερο πλήκτρο (button2)** θα αυξάνεται ο βαθμός δυσκολίας του παιχνιδιού με εμφάνιση δύο εχθρικών αεροπλάνων ταυτόχρονα.

![Github Robuino](/images/pcb-14.JPG) 

## Υλικό Αποθετηρίου

Σ' αυτό το αποθετήριο (https://github.com/8gymnperist/Robuino) γίνεται αναφορά στους στόχους του έργου, σε ποιους απευθύνεται, παρουσιάζεται η πλήρης πορεία ανάπτυξής του (λογισμικού και υλικού), το εκπαιδευτικό υλικό που χρησιμοποιήθηκε, αλλά και οπτικό υλικό με φωτογραφίες και βίντεο σχετικά με την τεκμηρίωση και την υλοποίησή του.

Το υλικό του αποθετηρίου επίσης παρουσιάζεται και στη σελίδα μας στο: https://robotics.ellak.gr/?post_type=robotics_participant&p=1710&preview=true


### Προαπαιτούμενες γνώσεις των μαθητών

Το έργο υλοποίησε η ομάδα μας αποτελούμενη από τρεις μαθητές της Γ’ Γυμνασίου. Θεωρούμε ότι μπορεί να  υλοποιηθεί γενικά από μαθητές αυτής της τάξης (με προϋποθέσεις βέβαια που αναφέρονται παρακάτω), αλλά και από μεγαλύτερους μαθητές των τάξεων Λυκείου.
Όσον αφορά το απαιτούμενο προγραμματιστικό τμήμα του έργου, οι μαθητές μας, είναι ήδη εξοικειωμένοι με βασικές έννοιες προγραμματισμού (όπως προβλέπεται από το αναλυτικό πρόγραμμα του μαθήματος της Πληροφορικής για το Γυμνάσιο). Η επιλογή του Scratch 2 (scratch.mit.edu) [1] ως προγραμματιστικό περιβάλλον έγινε γιατί αποτελεί μια γλώσσα προγραμματισμού η οποία δίνει έμφαση στην αλγοριθμική λογική και υποστηρίζει το μαθητή να προγραμματίσει με εύκολο τρόπο – drag and drop - χρησιμοποιώντας κατάλληλα blocks τα οποία αναπαριστούν έτοιμες βασικές προγραμματιστικές δομές. Επίσης ήταν η γλώσσα που γνώριζε η ομάδα μας  και παράλληλα με την επέκτασή του (s2aio με πλακίδια) δίνεται η δυνατότητα στον αρχάριο με ευκολία να προσεγγίσει το προγραμματισμό  του μικροελεγκτή του Arduino. Ακόμη, στα πλαίσια του περιβάλλοντος Scratch, μπορούν να υλοποιηθούν αυθεντικές, ευχάριστες και με νόημα για το μαθητή δραστηριότητες που αυξάνουν το ενδιαφέρον όπως δημιουργία κινούμενων γραφικών (animations), και διαδραστικών παιχνιδιών. Τα παιχνίδια θεωρούνται ένα παλιό και διαχρονικό εργαλείο για την εκπαίδευση και είναι μεταξύ των πιο ευχάριστων δραστηριοτήτων.. Απαιτείται βέβαια η οικοδόμηση γνώσεων σε σχέση με τη λειτουργία του μικροελεγκτή και ενός μικρού συνόλου εντολών για τον προγραμματισμό του. (s2aio: https://github.com/MrYsLab/s2aio ) [2].

Όσον αφορά τη γνώση Φυσικών εννοιών χρειάζεται οι εμπλεκόμενοι μαθητές να έχουν προσεγγίσει το νόμο του Ohm και να έχουν οικοδομήσει γνώσεις και δεξιότητες σχετικά με τη δημιουργία απλών κυκλωμάτων (Πηγή – αντίσταση – led). 

Από τα Μαθηματικά χρειάζεται η γνώση των αναλογιών και των συντεταγμένων σε ορθοκανονικό σύστημα αξόνων.

### Ο σκοπός και οι στόχοι σε σχέση με τη πρόταση και το πρόγραμμα σπουδών 

**Ο Σκοπός**

Σκοπός μας είναι μέσα από την ανάπτυξη του έργου (παιχνίδι Arduplane) να εμπεδωθούν και να οικοδομηθούν γνώσεις και δεξιότητες σχετικά με τους μικροελεγκτές και τον προγραμματισμό, την φυσική, τα μαθηματικά και την τεχνολογία. Οι εμπλεκόμενοι να αισθανθούν ότι εκτός από απλοί χρήστες και καταναλωτές της τεχνολογίας, μπορούν να είναι και οι ίδιοι δημιουργοί. 

**Οι Στόχοι**

**Α)  Ως προς το προγραμματισμό:**

    • να επιλέγουν και να χρησιμοποιούν κατάλληλες μεταβλητές 
    
    • να εμπεδώσουν τη λειτουργία και την εφαρμογή των  προγραμματιστικών δομών: α) της ακολουθίας, β) της επανάληψης και γ) της επιλογής 
    
    • να προγραμματίζουν  τον μικροελεγκτή του Arduino uno με το ρεπερτόριο εντολών της επέκτασης s2aio του προγραμματιστικού περιβάλλοντος Scratch 2
        
    
**B) Ως προς τη Φυσική:**

    • να γνωρίσουν και να χρησιμοποιούν για το σχεδιασμό και την κατασκευή ηλεκτρικών κυκλωμάτων  τα εξής ηλεκτρικά παθητικά στοιχεία: α)αντίσταση, διακόπτη (button), led, ποτενσιόμετρο.
    
    • να εφαρμόζουν το νόμο του Ohm σε κυκλώματα για τον υπολογισμό της έντασης του ηλεκτρικού ρεύματος 
    
    • να χρησιμοποιούν breadboard για την κατασκευή πρότυπων ηλεκτρονικών κυκλωμάτων.
    
**Γ) Ως προς τα Μαθηματικά:**

    •  να εφαρμόζουν και να χρησιμοποιούν αναλογίες για την επίλυση καθημερινών προβλημάτων. 
    
    • να γνωρίζουν την έννοια των συντεταγμένων και να προσδιορίζουν απ’ αυτές σημεία σε ορθοκανονικό σύστημα συντεταγμένων (όπως η σκηνή προγραμματιστικού περιβάλλοντος του Scratch 2)
    
**Δ) Ως προς την Τεχνολογία:**

    • η κατασκευή με ασφάλεια απλών ηλεκτρικών κυκλωμάτων 
    
    • η ανάπτυξη δεξιοτήτων συγκόλλησης ηλκετρονικών στοιχείων σε διάτρητη πλακέτα 
    
    • η σωστή και ασφαλείς χρήση των κατάλληλων εργαλείων (συγκόλλησης κ.α.)
    

### Τρόπος οργάνωσης και λειτουργίας της ομάδας / Ο ρόλος των εκπαιδευτικών

Οι μαθητές υλοποίησαν δραστηριότητες  γνωστικής προετοιμασίας για την οικοδόμηση των γνώσεων σχετικά με το μικροελεγκτή και το προγραμματισμό του αλλά και των απαιτούμενων εννοιών από τα αντικείμενα της Φυσικής και των  μαθηματικών και οι οποίες αναφέρονται στο τμήμα του εκπαιδευτικού υλικού αυτής της εργασίας. 
Οι δραστηριότητες υλοποιήθηκαν από την ομάδα αλλά και από άλλους εθελοντές μαθητές στα πλαίσια πολιτιστικού προγράμματος που εντάχθηκε στη θεματολογία “Τεχνολογικά επιτεύγματα & Ψηφιακά Παιχνίδια” με τίτλο: “Δημιουργώ με τον μικροελεγκτή Arduino και το Scratch”. Η ομάδα συνεργαζόταν κάθε Δευτέρα μετά το πέρας του σχολικού προγράμματος για δύο διδακτικές ώρες κάθε φορά.

Μέσω συνεργατικής μάθησης αναπτύχθηκαν στους μαθητές ειδικές δεξιότητες, όπως η ανάληψη ρόλων και αρμοδιοτήτων, η υπευθυνότητα, η παρατήρηση, η συνομιλία, η συν-κατασκευή της γνώσης, ο σεβασμός,κ.ά.. Με αυτή τη προσέγγιση, οι μαθητές κατασκεύασαν το κύκλωμα του χειριστηρίου και προγραμμάτισαν το παιχνίδι συνδυάζοντας, γνώσεις και δεξιότητες από διαφορετικά γνωστικά αντικείμενα όπως αναφέρθηκαν παραπάνω.

Ο ρόλος των εμπλεκόμενων εκπαιδευτικών ήταν κυρίως συντονιστικός και καθοδηγητικός των μαθητών προκειμένου να οικοδομήσουν την γνώση και να ολοκληρώσουν το έργο τους. Ως καθοδηγητές φρόντισαν να μην δίνουν έτοιμες απαντήσεις, αλλά να δημιουργούν κατάλληλες μαθησιακές καταστάσεις και προβληματισμούς ώστε οι ίδιοι οι μαθητές ν’ ανακαλύπτουν την λύση. Επίσης, ενθάρρυναν κάθε προσπάθεια για να ωθήσουν τους μαθητές στην έρευνα και τον προβληματισμό και εκτός της σχολικής αίθουσας. Στην επίτευξη των παραπάνω συνέβαλε και η αξιοποίηση πλατφόρμας Μoodle εγκατεστημένης στο Πανελλήνιο Σχολικό Δίκτυο http://users.sch.gr/kalodikis/moodle33/.

## Οργάνωση του έργου

### Βήμα 1

Οι μαθητές (η ομάδα μας και άλλοι μαθητές) όπως ήδη αναφέρθηκε πρώτα υλοποίησαν δραστηριότητες  γνωστικής προετοιμασίας για την οικοδόμηση των γνώσεων σχετικά με το μικροελεγκτή και το προγραμματισμό του αλλά και των απαιτούμενων εννοιών από τα αντικείμενα της Φυσικής και των  μαθηματικών και οι οποίες αναφέρονται στο τμήμα του εκπαιδευτικού υλικού αυτής της εργασίας. Υλικό στο αποθετήριο: https://github.com/8gymnperist/Robuino/blob/master/docs/support-docs.md (Περιλαμβάνει και τις εγκαταστάσεις των απαιτούμενων λογισμικών)


### Βήμα 2 

Η ομάδα σχεδίασε την επιφάνεια διεπαφής του παιχνιδιού Arduplane (interface) με τα διάφορα αντικείμενα που θα περιλαμβάνονται στην οθόνη και τους κανόνες για το χειρισμό και τη λειτουργία τους με το κύκλωμα του χειριστηρίου. Στη συνέχεια με βάση αυτά, σχεδίασε και υλοποίησε πρωτότυπο κύκλωμα με χρήση breadboard και Arduino uno. Παρουσίαση στο αποθετήριο στη σελίδα:
https://github.com/8gymnperist/Robuino/blob/master/hardware-design/sxediasmos.md 

![Github Robuino](/images/build-prot-teliko.png)

### Βήμα 3

Η ομάδα προγραμμάτισε στο περιβάλλον προγραμματισμού (Scratch 2 με την επέκταση s2aio) το παιχνίδι. Η Παρουσίαση και τεκμηρίωση γίνεται στο αποθετήριο στη σελίδα:
https://github.com/8gymnperist/Robuino/blob/master/code/code-directory.md 
Επίσης, έλεγξε και διόρθωσε σφάλματα σχετικά με λειτουργία του προγράμματος και σε συνδυασμό με αυτή του χειριστηρίου.


### Βήμα 4 
Στο στάδιο αυτό η ομάδα το δοκιμασμένο πλέον κύκλωμα  του πρωτότυπου χειριστηρίου το κατασκεύασε με διάτρητη πλακέτα και αντικατέστησε σ’ αυτό το Arduino uno με Arduino nano και το τοποθέτησε σε κουτί. Το έλεγξε για τη σωστή λειτουργία του σε συνδυασμό με το πρόγραμμα του παιχνιδιού σε διάφορα περιβάλλοντα όπως: α) Windows 7, β) Linux Ubuntu Mate 18.04 και γ) Raspian (Raspberry pi 3). Η παρουσίαση γίνεται στο αποθετήριο και συγκεκριμένα στο τέλος της σελίδας:
https://github.com/8gymnperist/Robuino/blob/master/hardware-design/sxediasmos.md 

![Github Robuino](/images/pcb-8.JPG)     ![Github Robuino](/images/pcb-12.JPG) 

![Github Robuino](/images/pcb-14.JPG) 



**Πηγές**

[1]. https://scratch.mit.edu/ 

[2]. https://github.com/MrYsLab/s2aio 

[3]. https://github.com/MrYsLab/s2aio/wiki

[4]. https://www.arduino.cc/en/Main/Software 

[5]. https://www.python.org/ 

[6]. https://www.youtube.com/watch?v=6_4EDcYAzRE 



