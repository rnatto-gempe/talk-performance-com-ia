# Assets

Esta pasta guarda recursos visuais usados no deck.

## Pendentes

- [ ] `renato-foto.jpg` — foto do palestrante usada no círculo da capa (slide 1). Recomendado: 600×600px, JPG otimizado
- [ ] `qr-linkedin.png` — QR code do LinkedIn (slide 27)
- [ ] `qr-ralph-console.png` — QR code da waitlist do Ralph Console (slide 27)
- [ ] `qr-bussola.png` — QR code da Bússola Executiva de IA (slide 27)

## Como usar

### Foto da capa

Trocar o placeholder no `index.html`:

```html
<!-- ANTES -->
<div class="cover-photo-circle fade-in-d3">
  <span class="placeholder">FOTO<br>RENATO</span>
</div>

<!-- DEPOIS -->
<div class="cover-photo-circle fade-in-d3">
  <img src="assets/renato-foto.jpg" alt="Renato Barbosa">
</div>
```

### QR codes

No slide 27, substituir os `.qr-pic` (que renderizam padrão xadrez como placeholder):

```html
<!-- ANTES -->
<div class="qr-pic"></div>

<!-- DEPOIS -->
<img src="assets/qr-linkedin.png" alt="QR LinkedIn" class="qr-pic" style="background:none;border:2px solid var(--green)">
```

Recomendado: gerar QRs com fundo branco e cor `#00d9ff` ou `#ffc233` pra combinar com a paleta.
