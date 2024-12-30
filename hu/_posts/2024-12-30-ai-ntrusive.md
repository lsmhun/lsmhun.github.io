---
layout: post
title: AI-ntruzív gondolatok
lang: hu
lang-ref: ai-ntusive
tags:  [ai, generative programming]
---

Nemrégiben találkoztam az alábbi ábrával, ami szerintem igencsak elgondolkodtató.
Az összes manapság népszerű generatív modell lényegében a tág értelemben vett 
Internetet "tanulja meg". A technológiáról magáról 
[javax0](https://javax0.github.io/2024/07/22/llm-and-rag-hu.html) blogján szép 
összefoglalót lehet olvasni. 

Az képen látható a StackOverflow látogatási és ezzel párhuzamosan a 
felhasználói aktivitás zuhanása látható. Igen ám, csakhogy az összes model
összes programozáshoz kapcsolódó témájának legfontosabb forrása maga a
StackOverflow oldala! Ha onnan eltűnik a tartalom, akkor miből fog tanulni
a robot? És a jövőbeli technológiákkal mi lesz?

![stackoverflow-after-chatgpt-tom-alder.jpg](/artifacts/stackoverflow-after-chatgpt-tom-alder.jpg)

Ez a kérdés kicsit a tyúk és tojás problematikája, de ez most nyilván 
egyre égetőbb lesz, hiszen a 
[GitHub copilot](https://github.blog/news-insights/product-news/github-copilot-in-vscode-free/)
ingyenessége után még többen fogják használni kódolásra is az asszisztenst.

<!-- more -->


## Személyes meglátás

A fentieknek a saját blogom kapcsán is van hatása. Itt ugyanis olyan dolgokat 
próbáltam/próbálok körüljárni, ami valamennyire érdekel vagy szembe jött,
de munka közben nem fontos annyira. És közben a saját tapasztalatomat megosztani,
hogy mibe ütköztem bele. 

Ezzel mások is hasonlóan vannak, 
akik nálam sokszorosan tehetségesebbek, ügyesebbek, jártasabbak.
Nyilvánvalóan az ő motivációjukat is csökkenti, hogyha a 
"ChatGPT úgyis megmondja". Azonnali, prompt választ kaphat bárki
bármiről.

Minek írjak le bármit is, egyáltalán ki fogja elolvasni? 

Így elfogy a robot által feldolgozható releváns tartalom, és 
beáll egy fixen közepes minőségre. A menedzserek örülnek, amíg őket is
ki nem rúgják a következő leépítési hullámban, mert bizonyos 
szinten ők még könnyebben helyettesíthetőek egy jól fogalmazó chat-bottal.


## Számítógép és az elvárt válasz

A másik véleményt Sallai Tamástól olvastam, és bár rég találkoztunk, egyet kell
értsek a felvetett problémakörrel. Ebben a bejegyzésben olvasható:
[Thoughts on unreliable computing](https://advancedweb.hu/shorts/thoughts-on-unreliable-computing/), de ő is 
[Rob Bowley](https://www.linkedin.com/posts/robertbowley_is-computer-says-maybe-the-new-computer-activity-7272155588271255552-wfOi/)
posztja alapján indult el.

Ez a kérdéskör bár rokon az előzővel, mégis nagyon más.
Felhasználói oldalról ugyanis nagyon nem mindegy, hogy mi az elvárás!
Eddig egy géptől azt vártuk, hogy egzakt kérdésre pontos választ adjon.
Ezek után nem így lesz.

A felhasználók (azaz mi) megszokják, hogy a ChatGPT majd válaszol valamit,
ami ugyan többnyire igaz, de egyáltalán nem biztosan az. Költ verset
Vörösmarty Mihálynak, ami ugyan az ő stílusa, de nem ő írta. 
Kérünk tőle valamit, és valami hasonlót ad vissza, csak tök más aspektusból.


## Kép generálás

A kép generálás egy másik témakör a deepface és társai mellett. Az utóbbiakat már
választási kampányokban használják egész alacsony szinten is. 
Engem meglepett, hogy még egy kis falu polgármester választási kampányában is
bevetették, hogy lejárathassák a regnáló jelöltet, és általa sosem mondottakat
terjesztettek FB-n. Fura világ, hogy már ilyen kicsiben is mi megy. :)

Képet alkotni, festeni, rajzolni egy valódi kreatív tevékenység, de most
egy mezei billentyű-nyomogató is képes "bármire".
Először csak szórakozás szintjén, majd már aktív tartalom generálásban is
hamarosan megelőzik a humán munkatársat.

A [Dall-e 3](https://openai.com/index/dall-e-3/), [Stable Diffusion](https://stability.ai/stable-image) és társai elárasztották az Internetet és mostanra tényleg nehéz megmondani 
egyik másik képről, hogy valódi művész áll-e mögötte, vagy csak jól paraméterezett
generatív AI köpte ki magából.

Mostanra már letölthető modellekkel átlagos konfigurációval is percek alatt bármi
előállítható. Így tettem én is, letöltöttem a 
[stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
plusz néhány előre tanított modellt és már készült is egyik kép a másik után.

Mottó: "korean girl with flower in her hand"

StableDiffusion alap model: 
![korean-girl-with-flower-in-her-hand-001.png](/artifacts/korean-girl-with-flower-in-her-hand-001.png)

Jól láthatóak a kezdetleges modell hibái: ujjak száma nem stimmel, 
a virágok nem (csak) a kezében vannak, a szájnál összekeverednek a 
vonalak. De azért alapvetően mégis felismerhető.

Aztán a [Google Gemini](https://gemini.google.com) segítségével már kérhettem
mást is. 
Ennyi volt a prompt: "Generálj nekem egy képet egy szivárvány színű nyolc fejű macskáról".

Gemini 1.5 Flash model:

![Gemini_Generated_Image_q4bt3rq4bt3rq4bt.jpg](/artifacts/Gemini_Generated_Image_q4bt3rq4bt3rq4bt.jpg)

Ugyanez Gemini 2.0 Flash beta model:

![Gemini_Generated_Image_q4bt3rq4bt3rq4bt.jpg](/artifacts/Gemini_Generated_Image_v8vh5xv8vh5xv8vh.jpg)

Hát... Számolni azért még nem tud, bár az újabb model már 
eljutott háromtól hatig, de a 
[Nyolcas szám szörnye](https://discworld.fandom.com/wiki/Bel-Shamharoth)
úgy tűnik még egy robotot is megijeszt.

## Zárszó

Bár kicsit szétszórt lett ez a poszt és nem is mindenütt pozitív, 
de senki se vegye magára. 

__Boldog új esztendőt kívánok!__