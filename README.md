# Niri dotfiles

Fedora üzerinde kullanılan kişisel Niri yapılandırması.

## İçerik

- `config.kdl`: ekranlar, çalışma alanları, pencere kuralları ve kısayollar.
- `.gitignore`: yalnız yapılandırma, README ve ignore dosyasını takip eder; yerel yedekleri dışlar.

## Bağımlılıklar ve kişisel ayarlar

Yapılandırma Noctalia, Ghostty, Dolphin, `hyprpolkitagent.service`,
`wl-paste`, cliphist, Solaar, wpctl ve playerctl çağırır. Uygulama
kısayollarında Brave Origin, Zed ve Flatpak uygulamaları da bulunur.
Bu uygulamaların kendi ayarları bu depoya dahil değildir.

Ekran ayarları DP-1 (2560×1440, yaklaşık 180 Hz) ve DP-3
(1920×1080, yaklaşık 120 Hz) için hazırlanmıştır. Başka bir makinede
çıkış adlarını ve modları uyarlayın.

`Mod+W`, `/home/savpavi/.local/bin/start-windows-looking-glass`
kişisel başlatıcısını çağırır; bu script ve VM dosyaları depoya dahil değildir.
Başka bir makinede bu kısayolu uyarlayın veya kaldırın.

## Kullanım

Mevcut `~/.config/niri/config.kdl` dosyanızı yedekledikten sonra bu depodaki
`config.kdl` dosyasını aynı konuma kopyalayın. Oturum açmadan önce doğrulayın:

```bash
niri validate --config ~/.config/niri/config.kdl
```

Bu makinede depo doğrudan `~/.config/niri` içindedir; aktif yapılandırma
değişiklikleri `git diff` ile görülebilir. Güncellemeleri göndermeden önce
doğrulama ve diff kontrolü yapın.
