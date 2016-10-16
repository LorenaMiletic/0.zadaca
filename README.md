# JMBAG
0036484323

# Pitanje 1
Nakon dodavanja Class Library kao reference, u bin/debug folderu Konzolne Aplikacije pojavile su se dvije nove datoteke: ClassLibrary1.dll, ClassLibrary1.pdb. U slučaju brisanja .dll datoteke nemoguće je pokrenuti izvršnu .exe datoteku. To se događa jer izvršna datoteka koristi Class Library biblioteku kao referencu, a CLR ne može pronaći odgovarajući međukod. U slučaju da je potrebno poslati upotrebljivu aplikaciju, dovoljno je poslati izvršnu .exe datoteku i Classlibrary1.dll, jer ostale datoteke nisu nužne za pokretanje aplikacije.

# Pitanje 2
Pokretanjem konzolne aplikacije bez prevođenja class library projekta ispisao se novi string. Razlog tome je što se pokretanjem konzolne aplikacije automatski pokreće build class library projekta.

# Pitanje 3
Ispisalo se Pero: Hello World. 

# Pitanje 4
Nakon dodavanja pero class library kao reference, u bin/debug folder konzolne aplikacije pojavila se datoteka PeroClassLibrary.dll.

# Pitanje 5
Nakon brisanja originalnog .dll-a aplikacija i dalje radi. Razlog tome je što se sada PeroClassLibrary.dll traži unutar debug foldera.

# Pitanje 6
Unatoč brisanju NodaTime foldera unutar package foldera, build se uspješno izvršio. Nakon build-a, u package folderu se ponovo nalazi NodaTime folder.
