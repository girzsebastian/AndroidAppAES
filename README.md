# Cerințe Android App cu End to End AES(Advanced Encryption Standard)
Construirea unei aplicatii Android cu criptare End to End folosind metoda AES (Advanced Encryption Standard) in baza de date Firebase de la zero.
## Studenți
1. Gîrz Sebastian - 1641A
2. Muresan Sebastian - 1641B
3. Roibu Remus - 1641B
4. Socaciu Călin - 1641B
## Prof. Coordonator
1. Mang Ioan
## Cerințe
1. Diverse setari ale fisierelor gradle.
2. Pentru criptare si decriptare se utilizeaza instanta AES a Android Cipher.
3. Sirul de mesaje este mai intai convertit in octeti, apoi criptat folosind metoda AES si apoi octetul este convertit inapoi in sir utilizand un set de caractere standard.
4. Acest sir de octeti criptat este apoi stocat in Firebase.
5. Deci, deoarece datele stocate în baza de date Firebase sunt în formă criptată, chiar dacă cineva poate obține accesul la baza de date, mesajul real nu va putea fi citit de către persoana respectivă până când acesta nu va avea metoda de criptare și cheia disponibile cu l.
6. Pe partea de decriptare, sirul primit din baza de date este convertit inapoi in octet folosind acelasi set de caractere.
7. Odata ce datele de octeti criptate sunt disponibile, atunci cifrarea modului de decriptare este utilizata pentru a decripta datele.
8. Datele decriptate sunt apoi convertite înapoi din octet în format lizibil String.
9. Apoi acel sir de iesire, dupa ce este sortat in ordine cronologica, este afisat in lista de vizualizare a aspectului aplicatiei noastre pentru ca utilizatorul sa o poata vedea.
