# Frontend fiktív megrendelés - feladatmegoldás menete

## 1. GIT
- Git repó létrehozása.
- Ha üres repót hozol létre és az angular projekteddel szeretnéd később összekötni, akkor leghamarabb a - 03-as pont után tedd meg az alábbiak szerint:
```terminal
echo "# maszkmester-angular" >> README.md  // ha üres, vagy nem létezik a README.md fájlod
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/felhasznalonev/reponev.git  // figyelj, hogy jó neveket használj!
git push -u origin main
```

## 2. ANGULAR
- Telepítjuk az Angulart, ha még nem tettük.
```terminal
npm i @angular/cli -g 
```

## 3. ÚJ PROJEKT
- Létrehozunk egy új Aggular projektet, majd belépünk a mappába.
```terminal
ng new projektneve
cd projektneve
code . -r
```

## 4. TELEPÍTÉSEK
- Bootstrap, jquery telepítése
```terminal
npm i bootstrap jquery
```

## 5. KONFIGURÁLÁS
- A bootstrap css-ét, valamint a bootstrap és a jquery javascript fájlját fel kell venni az angular.json fájlban.
```json
    "styles": [
        "./node_modules/bootstrap/dist/css/bootstrap.css", 
        "src/styles.scss"
    ],
    "scripts": [
        "./node_modules/jquery/dist/jquery.js", 
        "./node_modules/bootstrap/dist/js/bootstrap.js"
    ]
```

## 6. TERVEZÉS
- Tervezd meg akár papíron, hogy miként építed fel majd az alkalmazásodat!
- Milyen osztályok, servicek, komponensek szükségesek és azok hogyan kapcsolódnak majd egymáshoz.

## 7. KÓDOLÁS - HTML - CSS
- Létrehozzuk a szükséges komponenseket.
- Összeállítjuk az alkalmazás vázát képező html-t és az alap designt css-ben, majd kiszervezzük a megfelelő kódrészeteket a megfeleő komponensekbe.

## 8. KÓDOLÁS - Typescript
- Létrehozzuk a szükséges osztályokat, serviceket.
- A komponensek .ts fájljaiban megvalósítjuk az alkalmazás logikáját a tervünk alapján.

## 9. FINOMÍTÁS
- Logikai és design finomítások.
    
## 10. TESZTELÉS