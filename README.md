Flutrack.org
============

Οδηγίες εγκατάστασης
============

Αρχικά πρέπει να εκτελεστεί το αρχείο db.php μέσω ενός browser, ώστε να δημιουργηθούν οι πίνακες με τα πεδία στη βάση δεδομένων. 
Προϋπόθεση είναι να υπάρχει κάποιο Apache distribution που περιέχει MySQL και PHP (προτείνεται ως η πιο απλή λύση και όχι ως μοναδική).

Αμέσως μετά και ενώ δεν έχει εμφανιστεί κάποιο error καλείτε το http://127.0.0.1/φακελος-εφαρμογης/db.php?secretinstall=secretpassword-που εχετε βαλει στο db.php


Έπειτα πρέπει να εκτελεστεί το αρχείο backend.php. Για να γίνει αυτό σωστά πρέπει πρώτα να αντικατασταθούν οι αστερίσκοι στο αρχείο
auth.php. Η αντικατάσταση πρέπει να γίνει με τα κλειδιά που παρέχει το API του Twitter (https://dev.twitter.com/docs/auth/application-only-auth). 
Κάθε πιθανός χρήστης θα πρέπει να δημιουργήσει μια εφαρμογή στο API του Twitter ώστε να πάρει τα αντίστοιχα κλειδιά.


Το αρχείο results.json αποτελεί ένα ενδεικτικό παράδειγμα αρχείου οπτικοποίησης για το front-end τμήμα, όπως αυτό εξάγεται από τη βάση δεδομένων.
Μπορεί να χρησιμοποιηθεί από το index.html για να οπτικοποιήσει τα tweets. Ο χάρτης στο index.html δεν θα δείξει τίποτα καθώς 
λείπουν τα εικονίδια που θα αναπαραστούν τα Tweets. Δημιουργείστε ένα φάκελο images και μέσα βάλτε 2 εικονίδια της αρεσκίας σας (http://mapicons.nicolasmollet.com/) 


Τα αρχεία gennaw.php, gennhtriajson.php χρησιμοποιούνται για να εξάγουν τα αρχεία json από τη βάση δεδομένων και αρχικά δεν έχουν καμία χρησιμότητα.
Πρέπει να τονιστεί ότι τα tweets μπορούν να εξαχθούν από τη βάση με πολλούς άλλους τρόπους (π.χ. xml).

Στο αρχείο style.css μπορούν να αλλάξουν οι διαστάσεις του χάρτη και από το αρχείο map.js μπορεί να γίνει η παραμετροποίησή του. Εκεί πρέπει να αλλαχτούν και τα ονόματα
των markers, που θα οπτικοποιούν τα tweets, ανάλογα με τις εικόνες που θα χρησιμοποιηθούν. Μπορεί ακόμα να γίνει η διαμόρφωση των παραμέτρων
του χάρτη και ποιων χαρακτηριστικών θα εμφανίζονται (ή όχι).

ΠΡΟΣΟΧΗ:

Στη σελίδα που δημιουργείτε account στο twitter για να πάρετε τα credentials, πρέπει να προσθέσετε ως website/application-url, to url του localhost. Δηλαδή http://127.0.0.1 .Μόνο έτσι θα μπορεί η εφαρμογή σας να συνδέεται στον server του Twitter.

Για να δουλέψει η εφαρμογή τα παρακάτω πρέπει να είναι ενεργοποιημένα και να υποστηρίζονται από τον localhost server. *
 
[PHP Modules]
apc,
bcmath,
bz2,
calendar,
Core,
ctype,
curl,
date,
dba,
dom,
ereg,
exif,
fileinfo,
filter,
ftp,
gd,
gettext,
hash,
iconv,
json,
libxml,
mbstring,
mhash,
mysql,
mysqli,
mysqlnd,
openssl,
pcntl,
pcre,
PDO,
pdo_mysql,
Phar,
posix,
readline,
Reflection,
session,
shmop,
SimpleXML,
soap,
sockets,
SPL,
standard,
suhosin,
sysvmsg,
sysvsem,
sysvshm,
tokenizer,
wddx,
xml,
xmlreader,
xmlwriter,
zip,
zlib

Για οποιαδήποτε ερώτηση, προβληματισμό ή ιδέα επικοινωνήστε στο: sckarolos@yahoo.com
