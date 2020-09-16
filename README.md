# Tvořím web A–Z: lekce 01

- lektoři
    - Tomáš Kout
    - Tomáš Kazatel
- kouči
    - Pavla Havránková
    - Yana Taran
    - Jan Čuma
- workshopistka Czechitas
    - Markéta Vajčnerová 
- role koučů
    - pomáhají při lekcích
    - opravují úkoly
    - radí na FB 

---

## Témata

Box Model, DevTools, Float, Pozicování, Rozvržení stránky, Flexbox, Responsivní web, Media queries, CSS transformace, Přechody, Animace, Centrování prvků, CSS specificita, Pseudotřídy, Pseudoelementy, Formuláře, Tabulky, CSS custom properties (CSS proměnné), Vkládání prvků 3. stran (mapa, video z YT), Generátor statických stránek (Netlify) 

---

## Zkušenosti

Předpokladem účasti bylo osvojit si základy:

- úvodní kurz Czechitas
- online kurz Luďka Rolečka

---

## Nástroje

1. Visual Studio Code (VS Code)
1. GitHub.com
1. GitHub Desktop
1. prohlížeč: Google Chrome, Firefox (a jejich DevTools)

- my si tyto nástroje propojíme

---

# 1. VS Code

- textový editor pro psaní kódu v nejrůznějších jazycích
- ulehčuje nám psaní kódu
- osvojte si klávesové zkratky
    - `Ctrl/Cmd+S`
    - `Ctrl+šipky vlevo/vpravo`, `Ctrl+Shift+šipky vlevo/vpravo`
    - `Alt+šipky nahoru/dolů`
- [Psaní hravě](https://www.psanihrave.cz/) – pište všemi 10
- projekty

---

#### VS Code: projekty

```
Czechitas 
└── podzim 2020
   ├── lekce_01
   │   ├── cviceni_01
   │   │    ├── index.html
   │   │    └── style.css
   │   └── cviceni_02     
   ├── lekce_02
   └── lekce_03
```        

- v průzkumníku vytvořit adresář
- VS Code: _Add to workspace_
- vytvořit soubor `index.html`

---

#### VS Code: emmet

- kouzelná klávesa `Tab`
- `!` + `Tab` = 

- HTML i CSS, stačí napsat začátek značky nebo vlatnosti a zmáčknout `Tab`
- `ul>li*3>a` + `Tab`
- `lorem ipsum` + `Tab`
- [Nápověda](https://docs.emmet.io/cheat-sheet/)

---

## Cvičení 01

1. vytvoř stránku
2. přidej své jméno jako nadpis
3. přidej odkaz na svůj e-mail

---

#### VS Code: Live Server

- jedno ze stovek možných rozšíření VS Code
- aby fungoval, musíte mít vytvořený _workspace/projekt_ a mít soubor `index.html`
- přidáme rozšíření a zobrazíme si naši stránečku
    - na spodní liště okna s VS Code se vpravo objeví „Go Live“, klikni a otevře se prohlížeč s rozpracovanou stránkou
- **Propojili jsme si editor a prohlížeč!**
- při uložení se obnoví stránka => `Ctrl/Cmd+S` (lze nastavit automatické ukládání)

---

## Cvičení 02

1. přidej odstavec s _lorem ipsum_
2. vytvoř soubor CSS
3. podbarvi stránku třeba na růžovo
4. změň písmo nadpisů na bezpatkové (bezserifové)

---

## 2. GitHub

---

## 2. GitHub.com

- webová nadstavba nástroje _Git_

---

### GitHub: Git

- nástroj pro správu verzí vašeho projektu

- obdoba revizí ve Wordu, jen preciznější
- týmová spolupráce
- údržba a rozvoj projektu
- ovládá se psanými příkazy, ale toho vás ušetříme => GitHub Desktop

---

## 3. GitHub Desktop

note: 

- reprezentace GitHubu ve vašem počítači
- přihlásíme se _File | Options_ přihlašovacími údaji pro GitHub
- **Propojili jsme si GitHub.com a GitHub Desktop!!**
- zbývá nám propojit editor s projekty s GitHubem

---

### Git: slovníček

- repozitář
- klonovat
- commit
- push

- vývojářská latina, jíž se neubráníme, proto si raději jednotlivé termity vysvětlíme – postupně

---

### Git: repozitář/repository

- úložiště právě jednoho projektu

- de facto složka s vaším projektem

---

### Git: (na)klonovat/clone

- vytvořit duplikát repozitáře

- typicky si naklonujeme repozitář z GitHubu k sobě na počítač
- můžeme si ale naklonovat nějaký veřejně dostupný projekt
- **úkol**: _Vytvoříme si na GitHubu nový repozitář a naklonujeme si ho k sobě do počítače._
- kouzelné tlačítko _Set up in Desktop_ – tím se míní GitHub Desktop

---

![](https://i.imgur.com/qQ5bT5d.png)

- v Github Desktop můžeme svůj projekt otevřít
    - v průzkumníku jako adresář
    - na GitHub.com (v prohlížeči)
    - ve VS Code
- **Propojili jsme si VS Code s GitHubem!!!**

---

### Git: commit

- commit = souhrn změn v našem projektu
- commit message: popis těchto změn

- commit ~ závazat se, spáchat, předat
- doporučuje se commitovat často, nicméně záleží na vás
- commit message stručně, při týmové spolupráci kolegové ocení vysvětlení, proč jste ty změny provedly
- kolegou, který to ocení, můžeš být i ty sama – za 2 měsíce

---

### Git: push

- odeslání commitů na vzdálený server (pro nás GitHub.com)

note:

- Dokud jsou soubory u mě na počítači, mám nad nimi plnou kontrolu.
- Jakmile je _pushnu_ už se případné opravy a výmazy provádějí mnohem hůř.
- Tím se ale netrapte, commitujte a pushujte jak libo.
- _push_ je svým způsobem záloha

---

### Git: shrnutí

```
změny v repozitáři => 

    commit (více commitů) => 
    
        push (na GitHub.com) =>
        
            změny v repozitáři…
```

- a tak pořád dokola

---

### GitHub Pages

- svůj repozitář můžeme za určitých okolností rovnou vystavit na web

- musí být veřejný (public)
- v _Settings_ v sekci _GitHub Pages_ vyberu _branch/master_ a dám _Save_
- stránka se obnoví a na témže místě naleznu odkaz na web se svým projektem
- kdykoli pushnu, automaticky se (po chvíli) změny propíšou i do webu (nasadí se, anglicky deploy)
- na úvodní stránce repozitáře (záložka _Code_) přibyde v pravé liště _Environments_, kliknu na _view deployment_

---

# GitHub Classroom

- odevzdávání úkolů 
- jejich kontrola formou _codereview_, tj. připomínky přímo v kódu
- zadání přes FB (tím se propojí vše)
- zadání = repozitář, který si naklonujete k sobě do počítače a hotový ho pushnete na GitHub.com

---

# Domácí úkoly

- 4 + 2 nepovinné
- do sobotní půlnoci (nikoli striktně)

- přinejmenším první nepovinný si vypracujte, ať si ověříte propojení nástrojů, které stejně budete potřebovat pro úkoly povinné
- sobotní půlnoc: pokud chcete opravy od koučů před následující lekcí; pokud později, musíte počkat

---

## 4. prohlížeč: Google Chrome nebo Firefox

- dodržují nejvíce webových standardů
- mají nejkvalitnější nástroje pro vývojáře (devTools)

- pro práci používáme kvalitní nástroje
- Safari, Edge a nedejbože IE jsou vázány na konkrétní operační systém. Abychom vám mohli co nejpružněji pomáhat, ve vlastním zájmu používejte multiplatformní a populární prohlížeče.
- Naše webové stránky by samozřejmě měly fungovat (alespoň v základní podobě) ve všech prohlížečích. Proto je dobré si je ve všech prohlížečích před publikováním otestovat. To není předmětem tohoto kurzu, ale připomeňte si to, až narazíte na rozdíly.

