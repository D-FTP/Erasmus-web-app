# University project for third year's Design of Web Applications & Services class
**Team:** 3-Student Team

### 1. Εγκατάσταση XAMPP
Η έκδοση του προγράμματος πρέπει να είναι συμβατή με το λειτουργικό σας σύστημα.
* **Λήψη:** [Apache Friends - XAMPP](https://www.apachefriends.org/index.html)
* **Απαιτούμενα Components:** Apache, PHP, MySQL, phpMyAdmin.

### 2. Ρύθμιση `config.inc.php`
Πρέπει να ορίσετε τον κωδικό πρόσβασης για τον MySQL server στο αρχείο ρυθμίσεων του phpMyAdmin.

1. Μεταβείτε στον φάκελο: `C:\xampp\phpMyAdmin\` (ή εκεί που εγκαταστήσατε το XAMPP).
2. Ανοίξτε το αρχείο **config.inc.php**.
3. Στη **γραμμή 21**, αλλάξτε τον κωδικό:

**Αρχικό:**
$cfg['Servers'][$i]['password'] = '';

**Τελικό:**
$cfg['Servers'][$i]['password'] = 'admin123';

### 3. Εκκίνηση Apache Server & Βάσης δεδομένων

1. Από το **XAMPP Control Panel**, εκκινήστε (Start) τους servers **Apache** και **MySQL**.
2. Ανοίξτε το Terminal (γραμμή εντολών) και εκτελέστε τις παρακάτω εντολές:

mysql –u root

ALTER USER 'root'@'localhost' IDENTIFIED BY 'admin123';

FLUSH PRIVILEGES;

### 4. Εγκατάσταση Εφαρμογής

1. Εντοπίστε τον φάκελο **htdocs** (default: `C:\xampp\htdocs`).
2. Επικολλήστε εκεί τον φάκελο του έργου **erasmus portal**.

### Πρόσβαση
Η ιστοσελίδα είναι διαθέσιμη στο:
👉 [http://localhost/erasmus portal/index.php](http://localhost/erasmus%20portal/index.php)

---
> [!IMPORTANT]
> Βεβαιωθείτε ότι ο φάκελος στο htdocs ονομάζεται ακριβώς **erasmus portal** για να λειτουργούν σωστά τα links.
