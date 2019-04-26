
Oma kompileeritava rakenduse tegin React Native raamistikule, mille tegemiseks kasutasin järgnevat videot: https://www.youtube.com/watch?v=6ZnfsJ6mM5c&t=23s. 
Seadistamiseks tuleb Githubist repositoorium (https://github.com/kaidil/SharePlaces) omale arvutisse kloonida ja kas emulaatoris või Android telefonis käivitada.
1. Klooni repo
2. Ava projekt
3. Cmd-s liigu õigesse kausta, kus on projekt
4. Ühenda telefon arvutiga või käivita emulaator
5. Jooksuta käsku react-native run-android

Antud juhend oli minu arvates väga hea ja siiamaani üks asjalikumaid React Native raamistikku kirjeldavaid videosid. Pärast mitmeid hindude videosid oli meeldiv kuulda vahelduseks minu jaoks paremini mõistetavat Inglise keelt, tänu milllele olid ilmselt ka selgitused paremini arusaadavad. Video ise oli minu meelest profesionaalne, kus seletati detailselt, mida tehakse ning ka tempo oli mõõdukas. Võibolla oleks võinud olla rohkem selgitusi testimise jaoks.  Arendajale ilmselt elementaarsed võtted ei pruugi algaja jaoks olla nii iseenesestmõistetavad. Näiteks pikalt rakenduse kallal pusides jooksis äpp vahepeal kokku ning andis imelikke erroreid, mille lahendus oli tegelikult väga lihtne – taaskäivitada kogu rakendus, kuid mille välja selgitamiseks pidin errorit googeldama. Kuigi vlogger ise kasutas rakenduse testimiseks emulaatorit, siis tegelikult, vähemasti Nexus 5 ja Galaxy peal testimiseks emulaator ei sobinud ja ka see oleks võinud kohe alguses öeldud olla. 

Meeldiv oli, et kuigi RN raamistik uueneb sellise tempoga, et isegi alla aasta vana video võib juba olla aegunud, siis oli video all kaasa antud lingid RN-i dokumentatsioonile, millest oli kokkuvõttes palju abi. Siiski oli kõvasti nuputamist, kuidas lahendada timeout ja premission erroreid, mis tekkisid „Get Location“ nuppu vajutades, mis oleks pidanud leidma kasutaja asukoha, kuid video õpetuste järgi andsid erroreid. Selle lahendamiseks vahetasin getCurrentLocation() watchPosition() meetodi vastu.

Kuna tegemist oli oma funktsionaalsuse mõttes küllaltki lihtsa rakendusega, siis oli keeruline midagi väga originaalset (ja samal ajal teostatavat!) juurde mõelda. Siiski sai videos tehtud rakendust muudetud selle võrra, et äppi avades on nö default asukoht kaardil Tallinn. Kui kasutaja vajutab nupule „Get Location“ siis mitte lihtsalt ei tähistata kasutaja asukohta punase märgiga (marker) vaid suumitakse ka tänava vaatesse sisse.
