# Wormsik_by_Karol
Worms_game

Krok č.1 stiahnuť súborov ZIP:
Pre spustiteľnú hru je potrebné nasledujúće:
Stiahnutie súborov: "others", "others_num2", "Worms_game_Copy_Data", 
                    "Worms_game_Copy_BurstDebugInformation_DoNotShip",
                    "MonoBleedingEdge", 
1.Krok: Je potrebné rozbaliť vsšetky súbory do jednoho "hlavného" súboru. 
2.Krok: Následne je potrebné všetky súbory/položky zo súborov 
        "others" a "others_num2" presnúť do "hlavného" súboru. 
3.krok: Po presune možte prázdne súbory "others" a "others_num2" zmazať.
4.Krok: Hra sa spúšťa pomocou .exe súboru ktorý by sa po vykonaní kroku č.2 mal 
        nachádzať v "hlavnom" súbore. Meno tohto exe súboru je Worms_game_Copy.exe
 
Po tomto kroku by mala byť hra plne funkčná.
V hlavnom menu si môže uživatel vybrať počet tímov (2-4) a počet wormsíkov v tíme (1-4). Po nastavení týchto parametrov a klíknutím na tlačítko "Play"
sa hra spustí s požadovanými parametrami. 
Ovládanie je zase zobrazené na scéne na ktorú sa dokáže uživatel dostať z hlavného menu pomocou tlačítka "How to play".

5.Krok: Stihnutie a rozbalenie ZIP položky/súboru "Assets".

Nastavenie hry:
  Na začiatku resp. na "Vstupnej scéne" si uživateľ môže nastaviť počet hráčov v hre a počet wormsíkov v každom tíme pomocou "slidebarov".
  Maximálny počet hráčov a počet wormsíkov v každom tíme je 4 (obmedzené dlžkou slide baru). Po nastavení týchto paramtrov môže uživateľ začať hru
  kliknutím tlačítka "Play".
  
  
Ovládanie hry:
  Na "Vstupnej obrazovke je aj tlačítko s názvom "How to play". Po kliknutí na toto tlačitko sa uživateľ dostane na scénu na ktorej je graficky znázornené,
  akými klávesami je možné ovladať hru.
  
  
  Klavesa Num1: klavesa pre spustenie jetpacku. Po opätovnom kliknutí sa jetpack automaticky vypne a hračovy tým pádom skončí kolo. Tato "abilita" môže byť každým       wormsíkom použitá iba 1 krát.
  
  
  Klavesa Num2: Klavesa pre zbraň "ďelo". Po kliknutí klávesy wormsík vytiahne ďelo. Ďalej je možno uhol výstrelu ovládať pomocou pohybu myšky na 
  obrazovke (uhol mierenia je možné vidieť z animácie wormsíka - pohybuje delom podľa pozície myšky). Ďalej podržaním klávesy "medzerník" hráč udeľuje 
  potrebnú energiu výstrelu. To akú veľkú energiu doteraz hráč udelil je možné vidieť z lišty nad wormsíkom, ktorá sa bude predlžovať úmerne s časom držania 
  klávesy "medzerník". Ak dlžka lišty dosiahne určitej kritickej hodnoty (ak je rovnako dlhá ako lišta života wormsíka) tak je bomba automaticky vystrelená.
  Bomba však môže byť vystrelená predčasne pomocou uvolnenia klávesy "medzerník".
  
  
  Klavesa Num3: Klavesa pre spustenie zbrane "vertical flame". Po kliknutí tejto klávesy wormsík nad niektorým nepriateľským týmom (vybraný náhodne) spustí 
  sériu ohnivých "gulí", ktoré vertikálne padajú smerom dole k zemi, a tým pádom môžu poškodiť životy nepriateľských wormsíkov (ale i vlastných ak sa nachádzajú v       blízkosti dopadu). Táto zbraň môže byť každým wormsíkom použitá iba 1 krát.
  
  
  Klavesa Num4: Klavesa pre spustenie schopnosti "punch". Wormsík v určitom svojom okolí "udrie" všetkých okolitých wormsíkov (i z rovnakého týmu) a vezme im polku ich života. Úder udeľuje určitú kinetiku, ktorá spôsobí odmrštenie wormsíkov od epicentra.
  
  
  Klavesa C: klavesa pre zmenu wormsíka v jednom týme. Hráč ktorý je práve na "ťahu" môže pomocou tejto klávesy zmeniť wormsíka (v svojom tíme), ktorého práve kontroluje.
  
  
  Klavesa Z: Zoom IN/OUT: Klávesa pomocou ktorej môže hráč ktorý je práve na "ťahu" meniť veľkosť kamery. Sú možné 2 réžimy: Réžim veľkej a malej kamery. 
  
  
  Šípka hore/do prava/do ľava: Pohyb wormsíkom (ktorého si hráč vybral) do strán (do prava / do ľava) + výskok (šípka hore).
  
  
  Klavesa medzerník: Udeľuje energiu výstrelu. 
  
  
 Priebeh hry:
 Každý hráč ma na dokončenie svojho kola 20s. Po uplynutí tohto času sa tým automaticky prepne na ďalší. Hrač môže za svoje "kolo" využiť maximálne 1 "schopnosť" wormsíka. Po využití schopnosti sa kolo taktiež automaticky skončí. Niketoré schopnosti je možné využívať opakovane (delo) a iné môže použiť každý wormsík len 1 krát (vertical flame). V niektorých častiach hry hráč nemá kontrolu nad ovládaním. To sú časti hry kedy kamera sleduje určité "následky" použitia schopností, alebo keď končí/začína hra. Cieľom hry je zvíťaziť nad ostatnými hráčmi (maximálne 4 hráči), vyradením všetkých nepriateľských wormsíkov z hry (vynulovaním života wormsíkov). 
  
  
Jednotlívé C# skripty pre jednotlivé scény sa nachádzaju v súbore "Scripts" s cestou: Assets\Scripts
Každá scnéna má svoje skripty uložené zvlášť v súbore s menom ktoré vystihuje danú scénu. Takže napríklad všetky skripty,
ktoré sú nejko spojené s logikou hry sú uložene v súbore "Game_scripts" s cestou: Worms_first_version\Assets\Scripts\Game_scripts
(a podbne pre ostatné scény: "How_to_play_scripts", "Loading_scripts", "Main_menu_scripts"

Poznámky:
Fyzika je naprogramovaná mnou. Nepoužival som na to žiadnu knihovňu. Za logiku fyziky a objektov na ktorých pôsobí je zodpovedná trieda "Ph_engine" (detekcia kolízií, udeľovanie zrýchlenia, kontrola stability ..).
Kvôli tejto fyzike som musel využiť abstraktné triedy, aby som mohol jednoducho "pôsobiť fyzikou" na všetky objekty aj keď sú odlišného typu.
Preto je v mojom programe abstraktná trieda "Physics_object", ktorá má parametre a metody ktoré potrebuje "Ph_engine" (rýchlosť, zrýchlenie, poloha, metoda posunu), a od tejto abstraktnej triedy "Physics_object" sú potom odvodené triedy (pomocou dedičnosti) pre wormsíka "WORM", pre úlomky "Debri_object", pre bombu "Bomb_object", ktoré majú svoje vlastné metody a atributy.


Trieda "Main_function" zodpovedá za logiku hry, za to v akom stave je kamera, či ma hráč "v ruke ovládanie", či sú splnené podmienky pre použitie určitej schopnosti.
za zmenu týmu a podobne... Táto trieda komuniku s triedou "Ph_engine" a s triedou "Procedural_Gen" (generácia zeme, ostrovčekov, jaskýň).

Trieda "Procedural_Gen" ma za úlohu generaovať (pomocou funkcie prelinoise) rôzne typy zeme, jaskyne, ostrovčeky a zapisať to do prislušnej matice (potrebná hlavne pre kontrolu kolízií).

Trieda "camera_fllow_script" zodpovedá za logiku kamery, za presuvanie časovača, líšt života, tlačítka spolu s kamerou. Za zmenu réžimu kamery atd...
P.S. za gramatické chyby v skriptoch sa vopred ospravedlňujem
