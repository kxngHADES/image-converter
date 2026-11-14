<div align="center">

<img src="assets/banner.svg" alt="FLIP/ - Drop it. Flip it. Take it." width="100%">

<img src="assets/ticker.svg" alt="HEIC to JPG, PNG to WEBP, AVIF to PNG" width="100%">

<br>

**HEIC off your iPhone. WEBP from the web. PNG, AVIF, GIF, BMP.**
<br>
**Flip any of them into JPG, PNG or WEBP, right in your browser.**

<br>

<img src="assets/badges.svg" alt="No uploads, no build step, zero servers, one HTML file">

<br>

[`PREVIEW`](#preview) &nbsp;&middot;&nbsp; [`HOW IT WORKS`](#how-it-works) &nbsp;&middot;&nbsp; [`FEATURES`](#features) &nbsp;&middot;&nbsp; [`FORMATS`](#formats) &nbsp;&middot;&nbsp; [`QUICK START`](#quick-start) &nbsp;&middot;&nbsp; [`STACK`](#stack) &nbsp;&middot;&nbsp; [`FAQ`](#faq)

</div>

<br>

<img src="assets/h-preview.svg" alt="Preview" width="100%">

<div align="center">

<img src="assets/preview.svg" alt="Animated preview of the FLIP/ interface" width="100%">

<sub>Polaroids drop in, the dial slides between steps, and the percentage fills with volt.</sub>

</div>

<br>

<img src="assets/h-how.svg" alt="How it works" width="100%">

<img src="assets/flow.svg" alt="Drop, flip, take" width="100%">

<table>
<tr>
<td width="33%" valign="top">

**DROP IT**

Throw files at the page, click to browse, or paste from your clipboard. The whole window is a drop zone.

</td>
<td width="33%" valign="top">

**FLIP IT**

Pick a format, quality and max size. Your browser decodes and re-encodes every image on a canvas.

</td>
<td width="33%" valign="top">

**TAKE IT**

Download files one by one, or take the whole pile as a single `.zip`.

</td>
</tr>
</table>

<br>

<img src="assets/h-features.svg" alt="Features" width="100%">

<img src="assets/features.svg" alt="Local only, HEIC and HEIF, batch, quality, max size, drag and paste, zip, stats" width="100%">

<br>

<img src="assets/h-formats.svg" alt="Formats" width="100%">

<table>
<tr>
<td align="center" width="50%">

#### IN

`HEIC` &nbsp; `HEIF` &nbsp; `JPG` &nbsp; `PNG`
<br>
`WEBP` &nbsp; `AVIF` &nbsp; `GIF` &nbsp; `BMP`

<sub>Anything your browser can decode also works.</sub>

</td>
<td align="center" width="50%">

#### OUT

`JPG` &nbsp; `PNG` &nbsp; `WEBP`

<sub>Pick one per batch.</sub>

</td>
</tr>
</table>

<sub>Animated GIFs are flattened to a single frame. HEIC and HEIF are decoded by `heic2any`. Everything else uses the browser's native decoder, so AVIF and WEBP input depends on your browser version.</sub>

<br>

<img src="assets/h-start.svg" alt="Quick start" width="100%">

```bash
git clone https://github.com/kxngHADES/image-converter.git
cd image-converter
```

Then open `index.html` in your browser. There is no `npm install`, no bundler and no config.

<br>

<img src="assets/h-stack.svg" alt="Stack" width="100%">

<div align="center">

<img src="assets/stack.svg" alt="HTML5, CSS3, Vanilla JS, GSAP, JSZip, heic2any, Canvas API">

</div>

<br>

| Piece | Job |
|---|---|
| **GSAP and Draggable** | The loader, the rail dial, magnetic buttons and draggable polaroids |
| **JSZip** | Bundles the download |
| **heic2any** | HEIC and HEIF decoding, loaded from a CDN |
| **Canvas API** | Resizing and encoding |
| **Anton, Permanent Marker, Space Grotesk** | Type, with neumorphic shadows, film grain and a lot of tape |

<br>

<img src="assets/h-palette.svg" alt="Palette" width="100%">

<img src="assets/palette.svg" alt="Volt D7FF3A, orange FF5B23, pink FF8FC7, blue 4D7CFF, charcoal 1B1D23" width="100%">

<br>

<img src="assets/h-faq.svg" alt="FAQ" width="100%">

<details>
<summary><b>Do my photos get uploaded anywhere?</b></summary>
<br>
No. There is no server. Decoding, resizing, encoding and zipping all happen in your browser tab. The only network requests are the libraries and fonts loaded from CDNs.
</details>

<details>
<summary><b>Why is the first HEIC conversion slow?</b></summary>
<br>
The HEIC decoder loads from a CDN the first time. On a slow connection that can take a few seconds. After that it is cached.
</details>

<details>
<summary><b>Why did my PNG ignore the quality slider?</b></summary>
<br>
PNG is lossless, so there is nothing to trade off. The slider greys out when PNG is selected.
</details>

<details>
<summary><b>Does it work on a phone?</b></summary>
<br>
Yes. The rail turns into a bottom bar. The parallax stickers, custom cursor and magnetic buttons need a mouse, so they only appear on desktop.
</details>

<details>
<summary><b>Does it respect reduced motion?</b></summary>
<br>
Yes. With <code>prefers-reduced-motion</code> on, the grain and looping animations switch off and the rest speeds up.
</details>

<br>

<img src="assets/footer.svg" alt="Your files never left this tab" width="100%">

<div align="center">

<sub>Free to use, remix and flip. &nbsp;&middot;&nbsp; **FLIP/**</sub>

</div>
