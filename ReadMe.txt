Zadatak je bio izraditi aplikaciju koja prikazuje trenutnu lokaciju tekstualno i na karti. Potrebno je omoguciti postavljanje markera na kartu prilikom cega se ispušta zvuk.
Klikom na gumb pokrece se kamera i omogucuje se slikanje jedne slike koja se sprema u galeriju pod nazivom koji je vezan za trenutnu korisnikovu lokaciju.
Nakon što se slika spremi, dolazi notifikacija na koju se može kliknuti i otvoriti zadnja spremljena slika u galeriji.

Gumb "Uslikati" pokrece kameru i omogucuje korisniku slikanje i spremanje slike. Nakon što se spremi, slika ce se prikazati na MainActivity-u. Slika dobiva naziv po trenutnoj lokaciji.
Karta se prikazuje pomocu fragmenta koji sadrži GoogleMap. Omoguceno je zumiranje i postavljanje na trenutnu lokaciju korisnika.

Kako bi slikanje i lociranje radili korisnik mora aplikaciji dati permissione za kameru, lokaciju i spremanje. Ako aplikacija nema neki od permissiona gumb "Uslikati" ce biti onemogucen jer su aplikaciji potrebne sve dozvole kako bi spremila sliku i imenovala ju po trenutnoj lokaciji.

Tokom izrade ove zadace naišla sam na nekoliko problema.
Pokretanje kamera i spremanje slike.
Problem je bio spremiti sliku s posebno dodjeljenim imenom. Rješenje sam pronašla na službenoj Android stranici i jedan blog post je detaljno objasnio postupak. Uz to, bilo je potrebno korisiti i FileProvider za koji sam objašnjenjepronašla na SO.
https://developer.android.com/training/camera/photobasics.html
https://androidkennel.org/android-camera-access-tutorial/
http://stackoverflow.com/questions/38200282/android-os-fileuriexposedexception-file-storage-emulated-0-test-txt-exposed
Klik na notifikaciju koji otvara sliku u galeriji.
http://stackoverflow.com/questions/21486415/open-gallery-folder-by-click-on-notification
Kojem treba dodati flag.
http://stackoverflow.com/questions/43168024/android-fileprovider-cannot-find-file
U to, korišteni su predlošci za laboratorijske vježbe.

ikone http://www.flaticon.com/
zvukovi http://soundbible.com/