# 🛠️ Övning: TypeScript och DOM-manipulation i Praktiken

Denna övning syftar till att ge dig praktisk erfarenhet av att kombinera TypeScript med DOM-manipulation i en webbmiljö. Du kommer att skapa och använda interfaces, hämta och manipulera HTML-element, samt dynamiskt generera innehåll med hjälp av `Array.map()`.

## ✅ Uppgifter

### 1. Definiera ett Interface
Skapa ett interface `Book` med följande egenskaper:
- `title: string`
- `author: string`
- `year: number`
- `isAvailable: boolean`

### 2. Skapa Objekt med Interface
Deklarera **två objekt** av typen `Book` som följer interfacet ovan.

### 3. Hämta och Ändra Text i DOM
I din HTML-fil:
```html
<p id="status-message">Laddar...</p>
````

I din TypeScript-kod:

* Hämta elementet med `getElementById`
* Ändra dess `textContent` till `"Sidan är redo!"`

### 4. Hämta Inputfält med Type Assertion

I din HTML-fil:

```html
<input type="text" id="user-name-input">
```

I TypeScript:

* Hämta elementet med `getElementById`
* Använd `as HTMLInputElement` för att komma åt `value`
* Skriv ut `value` till konsolen

### 5. Skapa och Lägg till Element

I TypeScript:

* Skapa ett nytt `<div>`-element med texten: `"Detta är en dynamisk div!"`
* Lägg till detta element till `<body>` i HTML-sidan

### 6. Dynamisk Lista med `Array.map()`

* Skapa en array av student-objekt:

```ts
const students = [
  { name: "Erik", age: 20 },
  { name: "Sara", age: 22 }
];
```

* I HTML:

```html
<ul id="student-list"></ul>
```

* I TypeScript:

  * Använd `Array.map()` för att omvandla varje objekt till ett `<li>`-element med namn och ålder
  * Lägg till dessa `<li>`-element till `#student-list` i DOM\:en

---

💡 *Tips:* Se till att köra din TypeScript-kompilator för att se ändringar i JavaScript och ladda om webbsidan för att se effekterna i webbläsaren.
