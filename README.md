## Despre ce e vorba?

Acesta este un driver Windows pentru [tastatura Bluetooth Q.8912 cu diactritice de la Qilive](http://www.qilive.com/ro/produit/tastatura-compacta-bluetooth), distribuită prin lanțul de magazine Auchan. Îl poți descărca de [aici](https://github.com/icflorescu/qilive-q8912-kbd-driver-win-ro/releases/download/1.0.0/q8912ro.zip), iar dacă ai nevoie de instrucțiuni de instalare, le găsești [mai jos](#cum-instalez).

![Tastatură Bluetooth Q.8912 de la Qilive - foto 1](https://cloud.githubusercontent.com/assets/581999/21957827/7a028862-daa8-11e6-8102-705b6fa59dce.jpg)

![Tastatură Bluetooth Q.8912 de la Qilive - foto 2](https://cloud.githubusercontent.com/assets/581999/21957831/7a1b7e12-daa8-11e6-854b-82ddc5386772.jpg)

## De ce?

Pentru că producătorul a "omis" să includă un driver pentru Windows care să mapeze corespunzător codurile caracterelor de pe tastatură și livrează un **produs nefuncțional**.

Există o serie de motive pentru care Q.8912 de la Qilive ar putea fi un produs interesant pentru piața din România.

În primul rând este **una dintre puținele tastaturi cu diacritice**, deci ar putea fi un accesoriu interesant pentru jurnaliști, *blogger*-i, scriitori și în general pentru orice fel de autori de conținut pentru care diferențele dintre *ras* și *râs* sau *fata*, *față* și *fâță* sunt importante.

În al doilea rând, produsul poate fi achiziționat la un preț relativ accesibil: pe 13 ianuarie 2017 am găsit-o într-un centrul comercial Auchan la aproximativ 61 de lei.

![Tastatură Bluetooth Q.8912 de la Qilive - vândută de Auchan](https://cloud.githubusercontent.com/assets/581999/21957829/7a03a2ce-daa8-11e6-95b6-20b512d5824b.jpg)

După părerea mea, din punct de vedere ergonomic, cele mai bune tastaturi cu suport pentru limba română sunt cele fabricate de Apple (vezi informații [aici](https://support.apple.com/ro-ro/HT201794)), însă realitatea este că nu oricine își permite să plătească prețul acestora în România, în special în rândul celor din categoriile profesionale enumerate mai sus.

În aceste condiții, produsul "*brand*-uit" sub marca Qilive de la Auchan ar putea fi o alternativă interesantă: calitatea construcției nu este rea (deși nu se apropie de cea a produselor Apple), formatul *low-profile* "îndrăzneț" de asemănător cu cel al produselor Apple este foarte ergonomic iar *layout*-ul nu este de loc rău: există taste dedicate pentru *ă*, *â*, *î*, *ș*, *ț*, iar formatul de bază este *qwerty* (cu alte cuvinte, *y* și *z* sunt în pozițiile "corecte" cu care ne-am obișnuit).

Există însă o problemă majoră: **în Windows există trei layout-uri de tastaturi românești — Legacy, Standard și Programmers — iar produsul vândut de Auchan nu respectă nici unul dintre acestea și nici nu oferă posibilitatea descărcării unui driver care să remedieze această problemă**.

Un driver poate fi construit folosind un vechi utilitar de la Microsoft, [Keyboard Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=22339), însă acest lucru nu este la îndemâna unui utilizator normal, și realitatea este că, fiind vorba despre un produs comercial, **ar fi trebuit să o facă producătorul, nu clienții**.

Nu-i nimic, l-am făcut eu. L-am testat pe Windows 10, dar ar trebui să funcționeze fără probleme și pe Vista sau 2000 (nu sunt foarte sigur despre XP, dar oricum ar fi bine să nu-l mai folosești). Îl poți descărca de [aici](https://github.com/icflorescu/qilive-q8912-kbd-driver-win-ro/releases/download/1.0.0/q8912ro.zip), iar în continuare găseși câteva instrucțiuni simple de instalare.

## Cum instalez?

### Pasul 0

Dacă nu ai făcut-o deja, împerechează tastatura prin Bluetooth conform instrucțiunilor din [ghidul  producătorului](http://www.qilive.com/sites/default/files/content/notice/pdf/im_q.8912_qilive_bluetooth_keyboard_2.pdf). :no_mouth:

### Pasul 1

Dacă nu ai făcut-o deja, descarcă arhiva de [aici](https://github.com/icflorescu/qilive-q8912-kbd-driver-win-ro/releases/download/1.0.0/q8912ro.zip), deschide-o și rulează `setup.exe`.

![Instalare driver pentru tastatură Bluetooth Q.8912 de la Qilive - pasul 1.1](https://cloud.githubusercontent.com/assets/581999/21957825/7a01c558-daa8-11e6-9fed-cf3ad3ce40e4.jpg)

Windows-ul îți va cere să confirmi că vrei să rulezi programul, însă în noua tradiție a lipsei de logică în construirea interfețelor Microsoft, fereastra de confirmare va fi cel mai probabil vizibilă inițial doar în *taskbar*. Apasă pe ea pentru a o activa (este scutul care pâlpăie gălbui).

![Instalare driver pentru tastatură Bluetooth Q.8912 de la Qilive - pasul 1.2](https://cloud.githubusercontent.com/assets/581999/21957826/7a028b00-daa8-11e6-802e-67ba972cbb89.jpg)

Confirmă că vrei să instalezi programul.

![Instalare driver pentru tastatură Bluetooth Q.8912 de la Qilive - pasul 1.3](https://cloud.githubusercontent.com/assets/581999/21957830/7a07ad42-daa8-11e6-8f33-759cff85e6b7.jpg)

### Pasul 2

Dă un restart. La urma urmei, e Windows.

### Pasul 3

În partea din dreapta jos a *taskbar*-ului ar trebui să ai un meniu cu *input methods*. Apasă pe el și selectează Romanian (Q.8912-RO).

![Instalare driver pentru tastatură Bluetooth Q.8912 de la Qilive - pasul 3, gata!](https://cloud.githubusercontent.com/assets/581999/21957828/7a036a84-daa8-11e6-8d62-a92b4f988a05.jpg)

Gata.

## *Bonus*-uri

Pentru a îmbunătăți funcționalitatea, am adăugat coduri pentru următoarele caractere:

- `AltGr` + `E` => `€`, `euro sign`, pentru că România este o țară europeană și folosim destul de mult moneda unică;
- `AltGr` + `-` => `—`, `em dash`, pentru că poate fi folosit ca linie de dialog (mai multe informații găsiți în [acest document](http://www.secarica.ro/std/InstitLingvTastatura-20031008.pdf) din arhiva Academiei Române).

## *Tips & tricks* pentru alte scenarii de utilizare

### macOS

Nu văd de ce ai vrea s-o folosești pe Mac. Dar dacă insiști, probabil că ar trebui să-ți construiești un *layout* corect cu [Ukelele](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=ukelele).

### Linux

Dacă vrei să folosești tastatura Q.8912 pe Ubuntu, Linux Mint sau altă distribuție de Linux, mai mult ca sigur că știi deja ce ai de făcut, dar uite [aici](https://help.ubuntu.com/community/Custom%20keyboard%20layout%20definitions) un bun punct de pornire.

### Android

Bineînțeles că poți lega tastatura Q.8912 la orice tabletă cu Android care dispune de conexiune Bluetooth. Va trebui să folosești însă o aplicație comercială — [External Keyboard Helper Pro](https://play.google.com/store/apps/details?id=com.apedroid.hwkeyboardhelper&hl=en) de la Apedroid — pentru a remapa corespunzător codurile caracterelor. Aplicația nu e scumpă (9,99 RON pe 14 ianuarie 2017) și am folosit-o cu succes pentru Q.8912 + [Samsung Galaxy Tab S 8.4](http://www.gsmarena.com/samsung_galaxy_tab_s_8_4_lte-6435.php) cu Android 5 și ulterior 6. E foarte posibil s-o poți face și tu cu tableta ta.

![Tastatură Bluetooth Q.8912 de la Qilive, folosită împreună cu o tabletă Android](https://cloud.githubusercontent.com/assets/581999/21958113/1aa0ec1e-daae-11e6-9ab7-351d3f4cbbf2.jpg)

Ideal ar fi fost să poți descărca gratuit un app făcut de Qilive; la ora actuală în Google Play există vreo 13 aplicații făcute de ei, dar — ghinion — nici unul pentru tastaturi.

## Disclaimer

Nu am nici o relație comercială cu Qilive sau Auchan, și am decis să distribui gratuit acest driver pentru că producătorul nu a făcut-o și continuă să vândă un produs etichetat incorect "Română tastatură" (nu știu exact ce vrea să înseamne, dar exact așa scrie pe ambalaj). :astonished:

## Sprijină autorul

Sunt un full-stack web developer independent din București, România.

Dacă găsești acest produs util, nu ezita să dai un [*tweet*](http://twitter.com/share?text=Driver%20Windows%20pentru%20tastatură%20Bluetooth%20Qilive%20Q.8912%20de%20la%20Auchan!&amp;url=http%3A%2F%2Fgithub.com/icflorescu/qilive-q8912-kbd-driver-win-ro&amp;hashtags=tastatura,română,qilive&amp;via=icflorescu), [*share* pe FB](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Ficflorescu%2Fqilive-q8912-kbd-driver-win-ro) sau să-mi dai un [*endorse* pe LinkedIn](https://www.linkedin.com/in/icflorescu). Și dacă ai cont pe GitHub, *please star this repo*.

## Licență

Codul sursă este distribuit sub [licență MIT](https://github.com/icflorescu/qilive-q8912-kbd-driver-win-ro/blob/master/LICENSE).    
