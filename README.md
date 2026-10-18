# FigCraft Web (Figma Alternative)

Wersja przeglądarkowa **FigCraft** (Rust + WebAssembly + WebGPU/WebGL2 + egui) — profesjonalne środowisko do projektowania interfejsów UI/UX, wektorowego prototypowania oraz natywnej obsługi plików Figma (`.fig`).

## Dostęp online

Aplikacja jest serwowana bezpośrednio pod adresami:
- **[https://fig.lmk.one/](https://fig.lmk.one/)**
- **[https://figcraft.lmk.one/](https://figcraft.lmk.one/)**
- Kopia GitHub Pages: **[https://lukasz-sklad.github.io/fig-web/](https://lukasz-sklad.github.io/fig-web/)**

## Kluczowe możliwości i domyślna konfiguracja

- **Silnik:** Rust `wasm32-unknown-unknown` z optymalizacjami `wasm-opt -Oz` i prekompresją Gzip.
- **Domyślna konfiguracja:**
  - Język interfejsu: **Polski (PL)**
  - Motyw: **Ciemny (Dark mode)**
  - Akceleracja graficzna: **WebGPU** (z płynnym fallbackiem do **WebGL2**)
- **Obsługa parametrów URL:**
  - `?file=<url>` — automatyczne pobieranie projektu z zewnętrznego adresu URL (z mostkiem CORS `https://lmk.one/api/cors`), import na płótno i automatyczne otwarcie.
  - `?lang=pl` / `?lang=en` — dynamiczny wybór języka interfejsu.
  - `#join=<link_or_code>` — bezpośrednie dołączenie do sesji kolaboracji na żywo (Live collaboration).
- **Formaty:** `.fig` (Figma), `.figcraft`, `.svg`, `.json`, `.png`, `.jpg`, `.webp`.
