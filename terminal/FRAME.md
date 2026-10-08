# 🔴 GTK 4 Pencerelerine Kırmızı Çerçeve Ekleme
# Adding a Red Border to GTK 4 Windows

## 🇹🇷 Türkçe Anlatım

### Amaç
Ubuntu GNOME masaüstünde GTK 4 kullanan uygulama pencerelerinin etrafına kırmızı renkli, köşeleri yuvarlatılmış bir çerçeve eklemek.

### Adım 1 — Terminali aç

Ubuntu'da `Ctrl + Alt + T` tuşlarına basarak terminali aç.

### Adım 2 — GTK 4 yapılandırma klasörünü oluştur

```bash
mkdir -p ~/.config/gtk-4.0
```

Bu komut GTK 4 için kullanıcıya özel yapılandırma klasörünü oluşturur. Klasör zaten varsa mevcut dosyalara dokunmaz.

### Adım 3 — CSS dosyasını aç

```bash
nano ~/.config/gtk-4.0/gtk.css
```

Dosya mevcutsa açılır, yoksa yeni bir dosya oluşturulur.

**Not:** Dosyada önceden CSS kuralları varsa bunları silmeden yeni kuralları ekle.

### Adım 4 — Kırmızı çerçeve kodunu ekle

Aşağıdaki CSS kodunu dosyaya ekle:

```css
window {
    border: 2px solid #c50000;
    border-radius: 10px;
}
```

**Kodun açıklaması:**

- `window`: GTK pencere öğelerini hedefler.
- `border: 2px solid #c50000`: İki piksel kalınlığında düz kırmızı kenarlık oluşturur.
- `border-radius: 10px`: Kenarlığın köşelerini yuvarlatır.
- `#c50000`: Kırmızı rengin hexadecimal (onaltılık) kodudur.

### Adım 5 — Dosyayı kaydet

Nano editöründe:

1. `Ctrl + O` tuşlarına bas.
2. `Enter` ile kaydet.
3. `Ctrl + X` ile çık.

### Adım 6 — Sonucu kontrol et

GTK 4 kullanan uygulamaları kapatıp yeniden aç.

Ardından CSS dosyasını kontrol etmek için:

```bash
cat ~/.config/gtk-4.0/gtk.css
```

**Önemli:** Sonuç uygulamanın GTK sürümüne, temasına ve pencere yapısına göre değişebilir. GNOME Terminal gibi GTK 3 kullanan uygulamalar bu dosyadan etkilenmez.

---

## 🇬🇧 English Instructions

### Objective

Add a red border with rounded corners around GTK 4 application windows on Ubuntu GNOME.

### Step 1 — Open the terminal

Press `Ctrl + Alt + T` to open a terminal.

### Step 2 — Create the GTK 4 configuration directory

```bash
mkdir -p ~/.config/gtk-4.0
```

This creates the user-specific GTK 4 configuration directory if it does not already exist.

### Step 3 — Open the CSS file

```bash
nano ~/.config/gtk-4.0/gtk.css
```

If the file already exists, preserve its existing rules when adding the new CSS.

### Step 4 — Add the red border

Insert the following code:

```css
window {
    border: 2px solid #c50000;
    border-radius: 10px;
}
```

**CSS explanation:**

- `window`: Targets GTK window widgets.
- `border: 2px solid #c50000`: Applies a solid, two-pixel-wide red border.
- `border-radius: 10px`: Rounds the border corners.
- `#c50000`: The hexadecimal color value for the red border.

### Step 5 — Save the file

In Nano:

1. Press `Ctrl + O`.
2. Press `Enter` to confirm.
3. Press `Ctrl + X` to exit.

### Step 6 — Verify the result

Close and reopen the GTK 4 applications you want to customize.

To inspect the saved configuration:

```bash
cat ~/.config/gtk-4.0/gtk.css
```

**Note:** The effect depends on the application's GTK version and styling. Applications built with GTK 3 or other UI toolkits may not be affected.

---

## 🔴 Benim Kullandığım Orijinal CSS / My Original CSS

Ubuntu sistemimde kullandığım kırmızı çerçeve yapılandırması:

```css
window {
    border: 2px solid #c50000;
    border-radius: 10px;
}
```

**Dosya yolu / File path:** `~/.config/gtk-4.0/gtk.css`
