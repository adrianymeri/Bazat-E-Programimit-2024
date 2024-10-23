# C++ në Visual Studio Code

---

## Shkarkimi

1. Vizitojmë [code.visualstudio.com](https://code.visualstudio.com/) dhe e shkarkojmë versionin stabil.
2. Ndjekim hapat e instaluesit dhe e startojmë VS Code.

---

E hapim VS Code, dhe na shfaqet pamja në vijim:

![](/lendet/gjuhe-programuese/vs-code/screen-1.png)

---

<!-- .slide: style="font-size:0.8em" -->

Për të na lehtësuar punën me C++, na nevojiten dy extensions (zgjerime). Extensions instalohen duke shkuar te paneli Extensions (Ctrl+Shift+X), si në vijim:

![](/lendet/gjuhe-programuese/vs-code/screen-2.png)

---

<!-- .slide: style="font-size:0.8em" -->

**Extension 1: C/C++**

Në shiritin për kërkim e shkruajmë `C++`, dhe instalojmë `C/C++` si në pamjen në vijim:

![](/lendet/gjuhe-programuese/vs-code/screen-3.png)

---

<!-- .slide: style="font-size:0.8em" -->

**Extension 2: Code Runner**

Në shiritin për kërkim e shkruajmë `code runner`, dhe instalojmë `Code Runner` si në pamjen në vijim:

![](/lendet/gjuhe-programuese/vs-code/screen-4.png)

---

<!-- .slide: style="font-size:0.8em" -->

**Konfigurimi i Code Runner**

1. Hapim shiritin për komanda, përmes njërës mënyrë:
    - `View > Command Palette`
    - `Ctrl+Shift+P`
    - `F1`
2. E shkruajmë settings dhe zgjedhim opsionin `Preferences: Open User Settings (JSON)`, si në pamjen e mëposhtme:

![](/lendet/gjuhe-programuese/vs-code/screen-5.png)

---

Në settings e shkruajmë këtë konfigurim:

```json
{
  "code-runner.runInTerminal": true,
  "code-runner.preserveFocus": false,
  "code-runner.saveFileBeforeRun": true,
  "C_Cpp.debugShortcut": false
}
```

Dhe shtypim `Ctrl+S` për t'i ruajtur ndryshimet.

![](/lendet/gjuhe-programuese/vs-code/screen-6.png)

---

Me këto hapa e përgatitëm VS Code për punë me C++.

Hapi tjetër është instalimi i kompajllerit MinGW.

---

**Instalimi i MinGW në Windows**

1. Vizitojmë faqen e [mingw](https://sourceforge.net/projects/mingw/) dhe e shtypim Download si në foton vijuese.
2. Hapim setup që e shkarkuam dhe ndjekim hapat e instalimit.
3. Pas instalimit shtypim `Continue`.

![](/lendet/gjuhe-programuese/vs-code/screen-7.png)

---

<!-- .slide: style="font-size:0.8em" -->

1. Kur na hapet MinGW Installation Manager, e zgjedhim `mingw32-gcc-g++-bin`.
2. E shtypim me tastin e djathtë dhe klikojmë `Mark for Installation`.
3. Shkojmë te menyja `Installation > Apply Changes > Apply`, dhe presim deri të mbarojë.

![](/lendet/gjuhe-programuese/vs-code/screen-8.png)

---

Pas instalimit, na nevojitet ta regjistrojmë kompajllerin në PATH variablën.

Variablës PATH duhet t'i shtohet pjesa `C:\MinGW\bin`

1. Për Windows 7 ndjekni [këta hapa](https://www.rose-hulman.edu/class/csse/resources/MinGW/installation.htm).
2. Për Windows 10, ndjekni hapat në vazhdim.

---

<!-- .slide: style="font-size:0.8em" -->

1. Klikojmë `This PC` me të djathtën.
    - Shkurtesë: `WinKey + Pause`.
2. Shkojmë te `Properties > Advanced system settings`.

![](/lendet/gjuhe-programuese/vs-code/screen-9.png)

---

<!-- .slide: style="font-size:0.8em" -->

1. Klikojmë `Advanced system settings`
2. Klikojmë `Environment Variables...`

![](/lendet/gjuhe-programuese/vs-code/screen-10.png)

---

<!-- .slide: style="font-size:0.7em" -->

1. Zgjedhim `Path`.
2. Klikojmë `Edit...`.
3. Shtypim `New`.
4. Japim vlerën `C:\MinGW\bin`
5. Shtypim OK për të gjitha dritaret e hapura.

![](/lendet/gjuhe-programuese/vs-code/screen-11.png)

---

Nëse keni arritur në këtë hap është mirë të restartohet PC ose së paku të mbyllen të gjitha dritaret e VS Code dhe të rihapen.

---

**Hapja e folderit në VS Code**

1. Krijojmë ndonjë folder, psh. `Desktop > Ushtrime`.
2. E hapim në VS Code `File > Open Folder...`.

---

<!-- .slide: style="font-size:0.6em" -->

**Shkruarja e programeve në VS Code**

1. Krijojmë fajllin burimor, i cili duhet të mbarojë me prapashtesën `.cpp`.
2. E klikojmë fajllin dhe na hapet editori.
3. Te editori shkruajmë kodin dhe shtypim `File > Save` ose `Ctrl+S` për ta ruajtur.
4. Klikojmë ikonën për startimin e programit.
5. Na hapet konzola në të cilën e shohim rezultatin e ekzekutimit.
6. Procesi përsëritet për secilën detyrë.

![](/lendet/gjuhe-programuese/vs-code/screen-12.png) <!-- .element: style="max-width:640px;" -->
