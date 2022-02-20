---
layout: post
title: "42 Notları indirip nasıl kendi bilgisayarınızda çalıştırabilirsiniz"
author: akarah
category: Örnek Taslağı
tag: Örnek Taslağı

---

Diyelim 42 Notlara yazı eklemek istiyorsunuz bunun için fork atıp ana repo'yu klonladınız,
yazıyı da yazdınız ama pull request atmadan önce yazının website'de nasıl gözükeceğine
bakmak istiyorsunuz.

Problem şu ki pull request atıp sonra hataları düzeltirim deyip terkar pull
request açmak. Bunu sürekli yaptığınızı düşünün, artık pull request atmaktan sıkılırsınız.

Bunun çözümü repo'yu indirip kendi bilgisayarınızda website'yi lokal olarak çalıştırmak. Bunu da bu
yazıda yeterince açıklamayı çalışırım.

## Not
Kurulum aşaması şuan sadece Linux içindir

---
# 0. Repo'yu klonlayın
Burası basit [**repo'yu**](https://github.com/42resources/42resources.github.io) istediğiniz yere klonlayın.

---
# 1. Ruby ve gem kurulumu
## Linux

Eğer debian veya ubuntu kullanıyorsanız aşağıdaki komutu yazmanız yeterli

```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
```

Diğer linux sistemler için [**bu sayfaya**](https://jekyllrb.com/docs/installation/other-linux/) danışabilirsiniz

Gem'ler için kurulucayı klasörü bashrc'ye eklemeniz gerekiyor:
```bash
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

---
# 2. Jekyll ve bundler kurulumu

Tek komutla çözülüyor
```bash
gem install jekyll bundler
```

---
# 3. Websiteyi lokal olarak çalıştırma
Klonladığınız repo'nun içinde şu komutu çalıştırın

```bash
bundle install
```

ve son komut olarak bunu yazdığınız zaman artık website'yi lokal olarak çalıştırabilirsiniz!
```bash
bundle exec jekyll serve --livereload
```

Sonuç:
[![vim ve jekyll](/assets/tutorial_images/jekyll-local.png)](/assets/tutorial_images/jekyll-local.png)
