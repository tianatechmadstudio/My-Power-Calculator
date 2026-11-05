# My Power Calculator

**Version 1.0** · © 2026 Tiana TechMad Studio

[Malagasy](#malagasy) · [Français](#français) · [English](#english)

---

## Malagasy

Calculatrice scientifique miaraka amin'ny **caisse** sy **facturation** ho an'ny Android.
Mandeha **hors ligne** tanteraka, ary tsy mila internet.

### Fiasa

- **Calculatrice scientifique**: `+ − × ÷`, `xⁿ`, `%`, `±`, `√`, `1/x`, `π`, sin / cos / tan / cotan (amin'ny degré), →rad / →deg, mémoire (M+, M−, MR, MC). Safidy roa ho an'ny fomba kajy: laharan'ny operasiona (2+3×4 = 14) na mifandimby avy ankavia (= 20).
- **Stocks** (lisitry ny vokatra): Désignation sy P.U.
- **Caisse**: misafidy vokatra sy QTE, **Total**, **Rendu**, **Reste**, ary **Terminer**.
- **Facture**: N° mandeha ho azy (`A0000001`, `A0000002`…), daty sy ora (jj/mm/aaaa hh:mm), tahiry rehetra ary total ankapobeny.
- **Paramètre impression**: A4, A5, Ticket 80 mm, Ticket 58 mm; portrait na paysage; marges; haben'ny soratra; isan'ny kopia; soratra ambany; Rendu/Reste azo asehoy na afenina. Azo atao PDF ihany koa.
- Mombamomba ny orinasa (Nom société, Adresse, Contact, NIF, Stat) hita ao amin'ny facture.

### Fametrahana (Android 7.0 na vaovao kokoa)

1. Alaivo ny rakitra **`app-release.apk`** ao amin'ny pejy *Releases*.
2. Alefaso ao amin'ny finday (USB, Drive, WhatsApp…) ary sokafy.
3. Raha angatahana, ekeo ny **"Install unknown apps"** ho an'ilay application nampiasaina.
4. Raha miseho ny fampitandremana **Play Protect**, tsindrio ny **Install anyway** (mahazatra ho an'ny APK tsy avy amin'ny Play Store).
5. Sokafy ny **My Power Calculator**.

### Fanamarinana ny rakitra (SHA-256)

```
9e4de88d0f93897e1a1d7215f27c63ee93eeef4de893ce04ea3e3b967706222f  MyPower-v1.0.apk
```

Jereo hoe mitovy ny valiny ao amin'ny solosainao:

- Windows (PowerShell / CMD): `certutil -hashfile MyPower-v1.0.apk SHA256`
- Linux: `sha256sum MyPower-v1.0.apk`
- macOS: `shasum -a 256 MyPower-v1.0.apk`

Raha tsy mitovy ny valiny dia **aza apetraka** ny rakitra: mety nopotehina na novana izy.

**Sonia (certificat)**, SHA-256 fingerprint:
`7D:DD:CE:A0:96:E8:8A:8D:36:C4:3A:D9:97:31:48:9D:1D:75:B0:D9:73:C0:CF:22:97:28:1C:51:24:B5:87:A1`
(RSA 2048, SHA-256; manan-kery hatramin'ny 29/10/2051). Azo jerena amin'ny:
`apksigner verify --print-certs MyPower-v1.0.apk` (Android SDK build-tools).

### Fampahalalana ara-teknika

| | |
|---|---|
| Package | `com.tianatechmad.mypower` |
| Version | 1.0 (`versionCode` 1) |
| Android | minSdk 24 (7.0), targetSdk 34 |
| Teknolojia | Kotlin + WebView (pejy HTML/JS anatiny) |
| Habe | ≈ 2,5 MB |
| Fahazoan-dalana (permissions) | tsy misy fahazoan-dalana internet |

### Fifanarahana (Android)

- **Android 7.0 (API 24) na vaovao kokoa**; kendrena: Android 14 (API 34); mandeha ihany koa amin'ny Android 15 sy ny aoriana.
- Processeur ARM sy x86 (tsy misy code natif).
- Miankina amin'ny **Android System WebView** ny fanehoana: ataovy **vaovao** izy ao amin'ny Play Store (Android System WebView na Chrome), indrindra amin'ny finday Android 7 hatramin'ny 9.
- Miankina amin'ny service fanontana an'ny Android ny fanontana: mety miovaova arakaraky ny finday ny fanehoana ny habe ticket.

### Angona sy tsiambaratelo

Ny angona rehetra (vokatra, facture, paramètre) dia voatahiry **ao amin'ny finday ihany**.
Tsy misy fanangonana, fandefasana na fanarahana ho an'ny Tiana TechMad Studio. Mifafa ny angona
rehefa esorina ny application na fafana ny angony ao amin'ny paramètres an'ny Android.
Tsara ny mitahiry (impression/PDF) ny facture manan-danja.

### Fanamboarana avy amin'ny source

1. Android Studio → **File → Open** → lahatahiry `MyPower` (misy `settings.gradle.kts`).
2. Gradle JDK = **17** (na 21); andraso ny Gradle Sync.
3. **Build → Build APK(s)** (debug) na **Generate Signed Bundle / APK** (release).

### Fahazoan-dalana (License)

Jereo ny rakitra [`LICENSE`](LICENSE). Maimaim-poana ny fampiasana, ary tsy azo amidy na ovaina ny
application raha tsy misy alalana an-tsoratra avy amin'ny Tiana TechMad Studio.

---

## Français

Calculatrice scientifique avec **caisse** et **facturation** pour Android.
Fonctionne entièrement **hors ligne**, sans connexion internet.

### Fonctionnalités

- **Calculatrice scientifique** : `+ − × ÷`, `xⁿ`, `%`, `±`, `√`, `1/x`, `π`, sin / cos / tan / cotan (en degrés), →rad / →deg, mémoire (M+, M−, MR, MC). Deux modes de calcul au choix : priorité des opérations (2+3×4 = 14) ou séquentiel de gauche à droite (= 20).
- **Stocks** (liste des produits) : désignation et prix unitaire (P.U).
- **Caisse** : choix du produit et de la quantité (QTE), **Total**, **Rendu**, **Reste**, puis **Terminer**.
- **Factures** : numéro automatique (`A0000001`, `A0000002`…), date et heure (jj/mm/aaaa hh:mm), historique et total général.
- **Paramètres d'impression** : A4, A5, ticket 80 mm, ticket 58 mm ; portrait ou paysage ; marges ; taille du texte ; nombre de copies ; texte de pied de page ; affichage ou masquage du Rendu/Reste. Export PDF possible.
- Informations de l'entreprise (nom de la société, adresse, contact, NIF, Stat) imprimées sur la facture.

### Installation (Android 7.0 ou plus récent)

1. Téléchargez le fichier **`app-release.apk`** depuis la page *Releases*.
2. Transférez-le sur le téléphone (USB, Drive, WhatsApp…) et ouvrez-le.
3. Si demandé, autorisez **« Installer des applications inconnues »** pour l'application utilisée.
4. Si **Play Protect** affiche un avertissement, touchez **« Installer quand même »** (normal pour un APK hors Play Store).
5. Ouvrez **My Power Calculator**.

### Vérification du fichier (SHA-256)

```
9e4de88d0f93897e1a1d7215f27c63ee93eeef4de893ce04ea3e3b967706222f  MyPower-v1.0.apk
```

Vérifiez que le résultat est identique sur votre ordinateur :

- Windows (PowerShell / CMD) : `certutil -hashfile MyPower-v1.0.apk SHA256`
- Linux : `sha256sum MyPower-v1.0.apk`
- macOS : `shasum -a 256 MyPower-v1.0.apk`

Si le résultat diffère, **n'installez pas** le fichier : il a pu être corrompu ou modifié.

**Signature (certificat)**, empreinte SHA-256 :
`7D:DD:CE:A0:96:E8:8A:8D:36:C4:3A:D9:97:31:48:9D:1D:75:B0:D9:73:C0:CF:22:97:28:1C:51:24:B5:87:A1`
(RSA 2048, SHA-256 ; valide jusqu'au 29/10/2051). À vérifier avec :
`apksigner verify --print-certs MyPower-v1.0.apk` (Android SDK build-tools).

### Informations techniques

| | |
|---|---|
| Package | `com.tianatechmad.mypower` |
| Version | 1.0 (`versionCode` 1) |
| Android | minSdk 24 (7.0), targetSdk 34 |
| Technologie | Kotlin + WebView (page HTML/JS intégrée) |
| Taille | ≈ 2,5 Mo |
| Autorisations | aucune autorisation internet |

### Compatibilité (Android)

- **Android 7.0 (API 24) ou plus récent** ; cible : Android 14 (API 34) ; fonctionne aussi sous Android 15 et versions ultérieures.
- Processeurs ARM et x86 (pas de code natif).
- L'affichage dépend d'**Android System WebView** : gardez-le **à jour** via le Play Store (Android System WebView ou Chrome), surtout sur les téléphones Android 7 à 9.
- L'impression dépend du service d'impression d'Android : le rendu des formats ticket peut varier selon le téléphone.

### Données et confidentialité

Toutes les données (produits, factures, paramètres) sont enregistrées **uniquement sur le téléphone**.
Tiana TechMad Studio ne collecte, ne reçoit et ne suit aucune donnée. Les données sont supprimées
lorsque l'application est désinstallée ou que ses données sont effacées dans les paramètres Android.
Pensez à conserver (impression/PDF) les factures importantes.

### Compilation depuis les sources

1. Android Studio → **File → Open** → dossier `MyPower` (contenant `settings.gradle.kts`).
2. Gradle JDK = **17** (ou 21) ; attendez la fin de la synchronisation Gradle.
3. **Build → Build APK(s)** (debug) ou **Generate Signed Bundle / APK** (release).

### Licence

Voir le fichier [`LICENSE`](LICENSE) (en anglais). L'utilisation est gratuite ; l'application ne peut être
ni vendue ni modifiée sans autorisation écrite de Tiana TechMad Studio.

---

## English

Scientific calculator with a built-in **cash register** and **invoicing** for Android.
Works fully **offline**; no internet connection required.

### Features

- **Scientific calculator**: `+ − × ÷`, `xⁿ`, `%`, `±`, `√`, `1/x`, `π`, sin / cos / tan / cotan (in degrees), →rad / →deg, memory (M+, M−, MR, MC). Two calculation modes: operator precedence (2+3×4 = 14) or sequential left-to-right (= 20).
- **Stocks** (product list): designation and unit price (P.U).
- **Cash register**: pick a product and quantity (QTE), **Total**, amount paid (**Rendu**), change (**Reste**), then **Terminer** (finish).
- **Invoices**: automatic numbering (`A0000001`, `A0000002`…), date and time (dd/mm/yyyy hh:mm), history and grand total.
- **Print settings**: A4, A5, 80 mm ticket, 58 mm ticket; portrait or landscape; margins; font size; number of copies; footer text; show or hide the amount paid / change. PDF export supported.
- Company details (company name, address, contact, NIF, Stat) shown on the invoice.

### Installation (Android 7.0 or later)

1. Download **`app-release.apk`** from the *Releases* page.
2. Copy it to your phone (USB, Drive, WhatsApp…) and open it.
3. If prompted, allow **"Install unknown apps"** for the app you used to open the file.
4. If **Play Protect** shows a warning, tap **"Install anyway"** (normal for an APK distributed outside the Play Store).
5. Open **My Power Calculator**.

### Verify the file (SHA-256)

```
9e4de88d0f93897e1a1d7215f27c63ee93eeef4de893ce04ea3e3b967706222f  MyPower-v1.0.apk
```

Check that the result on your computer is identical:

- Windows (PowerShell / CMD): `certutil -hashfile MyPower-v1.0.apk SHA256`
- Linux: `sha256sum MyPower-v1.0.apk`
- macOS: `shasum -a 256 MyPower-v1.0.apk`

If the result differs, **do not install** the file: it may be corrupted or tampered with.

**Signing certificate**, SHA-256 fingerprint:
`7D:DD:CE:A0:96:E8:8A:8D:36:C4:3A:D9:97:31:48:9D:1D:75:B0:D9:73:C0:CF:22:97:28:1C:51:24:B5:87:A1`
(RSA 2048, SHA-256; valid until 29/10/2051). Verify with:
`apksigner verify --print-certs MyPower-v1.0.apk` (Android SDK build-tools).

### Technical information

| | |
|---|---|
| Package | `com.tianatechmad.mypower` |
| Version | 1.0 (`versionCode` 1) |
| Android | minSdk 24 (7.0), targetSdk 34 |
| Technology | Kotlin + WebView (bundled HTML/JS page) |
| Size | ≈ 2.5 MB |
| Permissions | no internet permission |

### Compatibility (Android)

- **Android 7.0 (API 24) or later**; target: Android 14 (API 34); also runs on Android 15 and newer.
- ARM and x86 processors (no native code).
- Display depends on **Android System WebView**: keep it **up to date** through the Play Store (Android System WebView or Chrome), especially on Android 7 to 9 phones.
- Printing relies on Android's print service: ticket-size rendering may vary between devices.

### Data and privacy

All data (products, invoices, settings) is stored **on the device only**.
Tiana TechMad Studio does not collect, receive or track any data. Data is deleted when the app is
uninstalled or its data is cleared in Android settings. Keep a copy (print/PDF) of important invoices.

### Build from source

1. Android Studio → **File → Open** → the `MyPower` folder (the one containing `settings.gradle.kts`).
2. Gradle JDK = **17** (or 21); wait for the Gradle sync to finish.
3. **Build → Build APK(s)** (debug) or **Generate Signed Bundle / APK** (release).

### License

See the [`LICENSE`](LICENSE) file. Free to use; the app may not be sold or modified without prior
written permission from Tiana TechMad Studio.

---

© 2026 Tiana TechMad Studio · v1.0
