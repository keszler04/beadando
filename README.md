# beadando
Keszler Bálint Máté {XVG9QZ}


A program egy egyszerű To-Do lista alkalmazást valósít meg a Tkinter könyvtár segítségével, amely lehetővé teszi a felhasználó számára teendők hozzáadását, törlését, listázását és mentését egy szövegfájlba. Az alkalmazás két osztályt tartalmaz: `ToDoList` és `ToDoListApp`.

### ToDoList osztály:

1. **`__init__(self)`**: Az osztály inicializálja a teendők listáját.

2. **`hozzaad(self, teendo)`**: Hozzáad egy új teendőt a listához.

3. **`torles(self, index)`**: Törli a kiválasztott teendőt a listából.

4. **`mentes(self, file_path)`**: Elmenti a teendőket egy fájlba.

5. **`betoltes(self, file_path)`**: Betölti a teendőket egy fájlból.

### ToDoListApp osztály:

1. **`__init__(self, root)`**: Az osztály inicializálja az alkalmazást és a GUI-t. Létrehoz egy beviteli mezőt a teendők hozzáadásához, gombokat a hozzáadáshoz, törléshez, mentéshez, valamint egy Listbox-ot a teendők megjelenítéséhez.

2. **`hozzaad(self)`**: Hozzáadja a beírt teendőt a listához, majd frissíti a Listbox-ot.

3. **`torles(self)`**: Törli a kiválasztott teendőt a listából, majd frissíti a Listbox-ot.

4. **`mentes(self)`**: Elmenti a teendőket egy szövegfájlba, és megjelenít egy felugró ablakot a mentés sikerességéről.

5. **`frissit_listbox(self)`**: Frissíti a Listbox-ot az aktuális teendőkkel.

### `main` függvény:

Az alkalmazás fő része, amely létrehozza a Tkinter főablakát és inicializálja az `ToDoListApp` objektumot.

### Főprogram:

A főprogram meghívja a `main` függvényt, és így indítja el az alkalmazást.

### Megjegyzés:

- Az alkalmazás az alapértelmezett fájlnevet "teendok.txt" használja a teendők mentéséhez.
- A teendők szövegei a Listbox-ban jelennek meg.
- A gombokat és az ablakot a Tkinter könyvtár segítségével hozza létre.
