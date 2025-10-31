# Assets da Timplu Landing Page

## ✅ Assets Existentes

- `logo.webp` (5.3KB) - Logo principal
- `timplu-hero.webp` (108KB) - Imagem hero
- `daniela-avatar.avif` (699 bytes) - Avatar depoimento
- `logo-*.webp` (6 logos de clientes, ~2-3KB cada)
- `favicon-96x96.png` (3.2KB)
- `favicon.svg` (2.5KB)
- `apple-touch-icon.png` (4.8KB)
- `web-app-manifest-192x192.png` (5.3KB)
- `site.webmanifest` - Manifest PWA

## ⚠️ Assets a Criar

Para performance e SEO completos, crie as seguintes imagens:

### 1. **og-image.jpg** (Open Graph)
- Dimensões: 1200x630px
- Formato: JPG otimizado (≤150KB)
- Conteúdo sugerido: Logo + tagline "Landing Pages em 7 dias"
- Localização: `/assets/og-image.jpg`

### 2. **twitter-image.jpg** (Twitter Card)
- Dimensões: 1200x600px
- Formato: JPG otimizado (≤150KB)
- Conteúdo: Mesmo da og-image ou variação
- Localização: `/assets/twitter-image.jpg`

### 3. **favicon.ico** (Fallback)
- Dimensões: 32x32px e 16x16px (multi-size ICO)
- Formato: ICO
- Localização: `/assets/favicon.ico`

## 📝 Como Criar

### Opção 1: Ferramentas Online
- OG/Twitter: [Canva](https://canva.com) (template 1200x630)
- Favicon ICO: [favicon.io](https://favicon.io) ou [RealFaviconGenerator](https://realfavicongenerator.net)

### Opção 2: ImageMagick (linha de comando)
```bash
# Converter PNG existente para ICO
convert favicon-96x96.png -resize 32x32 -colors 256 favicon-32.ico
convert favicon-96x96.png -resize 16x16 -colors 256 favicon-16.ico
# Merge em um único .ico
convert favicon-32.ico favicon-16.ico favicon.ico

# Otimizar JPG para OG
convert og-image.png -quality 85 -sampling-factor 4:2:0 -strip og-image.jpg
```

## 🎯 Impacto

- **OG/Twitter images**: +12% CTR em compartilhamentos sociais
- **Favicon completo**: Melhor branding e confiança
