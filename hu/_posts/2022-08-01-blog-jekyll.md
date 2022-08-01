---
layout: post
title: Jekyll és github pages
lang: hu
lang-ref: jekyll-github-pages
tags:  [jekyll, github pages]
---

A [GitHub pages](https://pages.github.com/) egy gyors, kényelmes és praktikus
megoldás, ha valami egyszerű oldalt szeretnénk összeállítani. Ráadásul szépen 
integrált is a github környezéhez.

A kezdéshez elég egy *$username.github.io* nevű repositoryt létrehozni és már
működik is. De ennél jóval többre képes! A [jekyll](https://jekyllrb.com/)
site generátor segítségével dinamikus oldalak is létrehozhatóak.

Ez a blog is ennek a segítségével készült.

<!-- more -->
[A blog forrása a github-on](https://github.com/lsmhun/lsmhun.github.io)

Az alapja [Viczián István](www.jtechlog.hu) blogja, de mivel
két nyelvű honlapot szerettem volna látni, egy kicsit változtattam.

A Jekyll-hez számos modul elérhető, azonban a Github Pages nem támogat, csak 
[néhányat](https://pages.github.com/versions/). Természetesen a több nyelvűséget
támogató [plugin](https://github.com/kurtsson/jekyll-multiple-languages-plugin) nincs a listán.

A témában több blog bejegyzés is született: 
- [KlaasNotFound](https://www.klaasnotfound.com/2017/02/16/proper-multilingual-site-with-github-pages-and-jekyll/)
- [brendamour](https://brendamour.net/2014/08/03/multilingual-jekyll-how-to-post-in-more-than-one-language/)

Véleményem szerint a dokumentáció akkor jó, ha minél közelebb van a kódhoz és lehetőség
szerint minél inkább generált kéne legyen. Ezért a legtöbb szösszenetet, amit elkövettem, inkább a
saját repojukban, a docs könyvtár alá tettem. Reméltem, hogy lesz erre is valami megoldás.
Van is: [remote include plugin](https://github.com/netrics/jekyll-remote-include) Csakhogy ez sem
támogatott. Úgyhogy végül maradt a copy-paste. :( Nem írok azért olyan sokat, hogy ne tudnám 
kezelni. 

Lehetett volna még egy harmadik, profibb megoldás: saját CI pipeline építése az oldalhoz. 
Van is hozzá [leírás](https://github.blog/2022-02-02-build-ci-cd-pipeline-github-actions-four-steps/),
nem is bonyolult. Valamint lehet szegény ember pipeline formátumaként, lokálisan generáltatni
annyi pluginnel, amennyivel csak akarunk és a végeredmény *_site* könyvtárat felküldözgetni... De 
ez már mindennél csúnyább.

A nyelvi linkeket is lehetne szebben, nem csak a jelenlegi főlapra mutató megoldással. Erre remekül megfelel
a meta adatok között a *lang-ref* elem, és már mehetne is a link a direkt fordításra. (ezt a 
[plugin](https://github.com/kurtsson/jekyll-multiple-languages-plugin) szépen
támogatja is). De az az érzésem, hogy akik ezt elolvassák, azok vagy egyik vagy másik nyelvet
preferálják, nem fogják ugyanazt kétszer is megnézni. Így csak a főlapra tettem egy böngésző
nyelvbeállításától függő továbbítást. Jelzem, ezt a SEO nagyon nem ajánlja, mert a kereső robotok büntetik...

Ha esetleg saját domain-t regisztrálnék az egyik címre, akkor a *CNAME* fájlt kell létrehozni, amibe 
fel kell vésni a saját címet. Ettől kezdve a {{ BASE_PATH }} változó értékének már ezt fogja használni.
Sok mindent már szépen megoldottak előttünk. 


