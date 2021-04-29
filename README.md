# Olympští bohové
App Mockup pro předmět WEB

## Popis hry
Aplikace je založena na karetní hře Černý Petr s tématikou Olympských bohů. Původně vyšla v časopise Junior.

## Pravidla hry

### Co hra obsahuje
POČET KARET: 29 (14 párů a karta Černý Petr)

POČET HRÁČŮ: 1 až 4

CÍL HRY: odložit všechny své karty a zbavit se Černého Petra (Krónos).

### Postup při hře
Všechny karty se promíchají a náhodně rozdělí stejným počtem mezi hráče. Jeden z hráčů musí mít jednu kartu navíc. Všichni hráči si zkontrolují, zda nemají ve svých kartách
logické dvojice (dají se rozlišit i podle barvy). Pokud ano, takové karty odloží stranou.

Hráč, který má nejvíce karet, nabídne dalšímu hráči, aby si od něj vzal jednu z karet. Hráč, který si vybral kartu, ji založí mezi své. Pokud tak získal logickou dvojici,
odloží ji stranou.

Ve hře je nutné udržovat stále stejné pořadí. Hra tak pokračuje až do doby, kdy jeden z hráčů odloží všechny své karty. Tím se stává vítězem. Hra tím ale nekončí.
Pokračuje se dál, až do chvíle, kdy jednomu z hráčů zbyde jediná karta, a to právě Krónos. Tento hráč prohrál.


## Dokumentace
### Přihlášení login.html
- Na této stránce se hráč může přihlásit pomocí Google nebo Facebook účtu.
- Následně je pak automaticky připojen do hry s dalšími hráči.
- Jakýkoli jiný počet hráčů než 4 musí být do čtveřice doplněn počítačem (kvůli lepší hratelnosti).

### Domovská obrazovka .index.html
- Stránka index.html je domovská obrazovka. Hráči zde vidí, kdo je zrovna na řadě.
- Čílso uvedené u každého z hráčů udává, kolik mu zbývá karet.
- Pokud je hráč zrovna na řadě, ikonky ostatních hráčů se změní na obrázky s příponou choose ze složky images.
- Pokud je hráč zrovna na řadě, klikne na jednoho z dalších hráčů a náhodně mu tak sebere jednu kartu, která se přesune do jeho přeledu karet.
- Pomocí tlačítka ,,ukázat karty" se hráč dostane do svého přehledu karet.

![image](https://user-images.githubusercontent.com/70745566/116578284-8c668800-a911-11eb-8708-b1e92093f35f.png)
![image](https://user-images.githubusercontent.com/70745566/116579631-dc921a00-a912-11eb-9389-e591e59ee46f.png)


### Přehled karet cards.html
- V přehledu karet se zobrazují pouze karty, které danému hráči zbývají (žádné prázdné sloty).
- Pokud hráč usoudí, že dané dvě karty patří k sobě, přetáhne je postupně do boxu s názvem ,,Vložit dvojici"
- Zde se zobrazí pouze miniatura každé karty, obsahující jen její název a obrázek. Miniaturu lze zobrazit pomocí přidání třídy . mini k divu karty.
  - Pokud karty skutečně patří k sobě, rámeček se zbarví do zelené barvy a po odezvě 1s karty zmizí.
  - Pokud k sobě karty nepatří, rámeček se zbarví do červené barvy a po odezvě 1s se karty opět vrátí do přehledu karet.

![image](https://user-images.githubusercontent.com/70745566/116518705-e5fa9280-a8d0-11eb-911a-2f102ebd9d62.png)
![image](https://user-images.githubusercontent.com/70745566/116518970-37a31d00-a8d1-11eb-9b30-b1a36194c9e0.png)


- Pokud hráč usoudí, že v přehledu karet identifikoval všechny dvojice, vrátí se pomocí tlačítka ,,hotovo'' zpět na domovskou obrazovku.
- *V desktopové verzi se v boxu zobrazí celá karta.*

### Knihovna karet library.html
- Tato sránka nijak nesouvisí s průběhem hry.
- Slouží pouze jako úložiště pro všechny karty ve hře.
- Každá dvojice karet je označena stejnou třídou, jako např. one + one, two + two, ...












