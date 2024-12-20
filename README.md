---

## **Övning 3: Kombinera Container Queries och `clamp()`**

### **Beskrivning**
Nu ska du kombinera **Container Queries** och **clamp()** för att skapa en responsiv kortkomponent med flexibel textstorlek.

---

### **Mål**
1. Använd `container: inline-size;` för att definiera containern.  
2. Skapa olika stilar för kortet med **Container Queries**.  
3. Använd `clamp()` för textstorlek så att den är responsiv oavsett containerns storlek.

---

### **Steg-för-steg**
1. Använd följande HTML-struktur:

```html
<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8">
  <title>Övning 3 - Kombinera Container Queries & clamp()</title>
  <style>
    /* Din CSS här */

  </style>
</head>
<body>
  <div class="card-container">
    <div class="card">
      <h2>Flexibelt kort</h2>
      <p>Texten är både responsiv och container-anpassad.</p>
    </div>
  </div>
</body>
</html>
```

2. I CSS:  
   - Definiera `.card-container` som en **container** med `container: inline-size;`.  
   - Använd **Container Queries** för att:  
     - Ändra bakgrundsfärg och padding på `.card`.  
   - Använd **`clamp()`** för att:  
     - Styra textstorleken på `<h2>` och `<p>`.

---

### **Exempeloutput**
- När containern är **smal (<400px)**:  
  - Bakgrund: **ljusgul**.  
  - Textstorlek: **Mindre** tack vare `clamp()`.  
- När containern är **bred (>400px)**:  
  - Bakgrund: **ljusgrön**.  
  - Textstorlek: **Större**, men maxgräns från `clamp()`.

---
