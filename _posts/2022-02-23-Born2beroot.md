---
layout: post
title: "Kök olmak için doğmuş"
categories: [Linux Born2beroot]
tag: [born2beroot]
author: a_furkan
=======

---
<img src="https://art.pixilart.com/3e3fc9c4c42536a.gif" align="right" height="550">

# :robot: Born2beroot

Bu proje bir Born2beroot yönergesidir. Bonus görevleri ve CentOS'u içermez.

## 🧭 Yol Haritası

1.  [Bölüm 1 (Debian'ı İndir)](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#one-episode-1-install-debian)

2. [Bölüm 2 (İndirmeler ve Ayarlamalar ve ve Konfigürasyonlar  )](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#two-episode-2-downloads-and-adjustments-and-and-configurations)
   - [SSH için](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#-for-ssh)
   - [UFW için](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#for-ufw)
   - [Sudo için](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#for-sudo)
   - [Şifre Politikalama](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#password-policy-)

3. [Bölüm 3 (Monitoring.sh ve Crontab Konfigürasyonları)](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#3%EF%B8%8F%E2%83%A3-episode-3-monitoringsh-and-crontab-configurations)

4. [Bölüm 4 (Teslim ve Ön Değerlendirme)](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#four-episode-4-submission-and-peer-evaluation)

5. [Ekstralar ve Kaynaklar](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/README.md#5%EF%B8%8F%E2%83%A3-extras-and-resources)
  
## :one: Bölüm 1 (Debian'ı İndir)

Önce VirtualBox'ı indirin ve ardından Debian'nın .iso dosyasını. İşte bağlantılar:

- ✅ [VirtualBox](https://www.virtualbox.org/)

- ✅ [Debian](https://www.debian.org/)

VirtualBox'ı kurduktan sonra açın:

Ve yukarıda ki yeni tuşuna basın!

<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/1..png?raw=true" align="center" height="325">

Devam devam devam.. ve 'Makine Klasörü' makine klasörünüzün yolu '/goinfre'nin altı olacaktır. Sonra ki kısımda ise disk imajını soracaktır bu **'.vdi'** olacaktır.

Ardından **'.iso'** Debian dosyasını seçin. Oluşturduğunuz sanal makineye tıklayın ve yukarıdaki **'ayarlar'a** tıklayın. ve oradan **'Depolama'ya** tıklayın, **'Empty'a** tıklayın ve sağ pencerede **'Optik Sürücü'** seçeneğinin yanındaki CD işaretine basın. Oradan, **'Disk Dosyasını Seç'e** tıklayın ve indirdiğiniz debian **'.iso'** dosyanızı seçin.

<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/2..png?raw=true" align="center" height="325">

Bunları yaptıktan sonra sanal makinenizi başlatın ve şu ekranı göreceksiniz:

<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/3.png?raw=true" align="center" height="350">

**'Grapichal Install'** seçeneğini seçin. (Endişelenmeyin, bu seçenek Debian'ı GUI olarak kurmaz. Sadece kurulum aşaması için bir seçenektir.)

Sonra ki kısım kurulum için bütün resimleri içerir:

<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/4..png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/5..png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/6.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/7.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/8.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/9.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/10.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/11.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/12.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/13.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/14.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/15.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/16.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/17.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/18.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/19.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/20.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/21.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/22.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/23.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/24.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/25.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/26.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/27.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/28.png?raw=true" align="left" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/29.png?raw=true" align="right" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode1/30.png?raw=true" align="center" height="300">

🏁 **Ve sonunda 1. Bölüm burada biter** 🏁

## :two: Bölüm 2 (İndirmeler ve Ayarlamalar ve ve Konfigürasyonlar)

Bu ekranı göreceksiniz. Sanırım bu giriş ekranı. :d

<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode2/1.png?raw=true" align="center" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode2/2.png?raw=true" align="center" height="300">

Bu komutu çalıştırarak diskinizin bölümlerini ve şifreli bölümlerini görebilirsiniz:

````lsblk````

İndirmelere ve yapılandırmalara devam etmeden önce şunları bilmekte fayda var:

- Root olmak:

```` su -````

- Güncellenmesi gereken bir paket var mı yok mu arar ve varsa bulur yoksa bulmaz:

````apt update````

- Güncellenmesi gereken bir paket varsa onu bu komut yapıyor ve güncelliyor:

````apt upgrade````

#### 🤸 Kullanıcı Komutları

Bunların haricinde, sanal makinenizde ki bütün kullanıcıları görme komutu:

````getent passwd````

Kullanıcı ekleme ve silme komutları **(root olmalısın)**:

````adduser <user_name>```` - ````deluser <username>````

#### 🍇 Grup Komutları

Sanal makinenizdeki grupları görme komutu:

````getent group```` or ````getent group <group_name>```` -> **Bir grup altındaki kullanıcılar**

Grup ekleme ve silme komutları **(root olmalısın)**:

````groupadd <group_name>```` - ````groupdel <group_name>````

#### 🤝 Kullanıcılar ve Grupların Birlikten Doğan Komutları

Bir kullanıcının hangi grupta olduğunu görmek için bu komut:

````groups <user_name>````

Bir gruba kullanıcı ekleme ve bir kullanıcıyı gruptan çıkarma komutu **(root olmalısın)**:

````usermod -aG <group_name> <user_name>```` - ````gpasswd --delete <group_name> <user_name>````

## 🛠️Paketleri İndirme ve Dosyaları Konfigüre Etme

### 🧰 SSH için

SSH'ı yükleme komutu:

````apt install openssh-server````

SSH etkinlik sorgu komutu ve SSH başlatma komutları:

````systemctl status ssh```` - ````systemctl start ssh```` - ````systemctl enable ssh````

#### :dna: SSH Port Değiştirme

Şu dizine gitmelisin:

```bash
  nano /etc/ssh/sshd_config
```
Bu ayarları değiştirmelisin:

- #Port 22 -> Port 4242
- #PermitRootLogin prohibit-password -> PermitRootLogin no
- Ve evet, '#' işaretini de kaldırın, yazdıklarınızı yorum satırı haline getirir '#' bu işaret. :)
- He bu arada o işaret sadece o iki ayar için. Sakın hepsi için kaldırma. :d

<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode2/3.png?raw=true" align="center" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode2/4.png?raw=true" align="center" height="300">

Tamam, bu ayarları yaptıktan sonra şu komutla yeniden başlatın:

````service sshd restart````

Ardından VirtualBox'ınıza gelin ve üst kısımdaki **'ayarlar'a**, ardından **'Ağ'a** basın,
daha sonra altta bir **'Gelişmiş'** bölmesi olacak, oraya tıklayın ve **'Port Yönlendirme'ye** basın.
Sağda yeşil **'+'** işareti olan bir düğme göreceksiniz, evet ona basın ve
tablo görünecektir. **‘Ana Makine Port’u ve ‘Misafir Port’u** bölümlerinde resimdeki gibi yapın.
Zaten resim ekliyorum, neden açıklama gereği duydum bilmiyorum. Her neyse, tamam ve tamam'a basın ve bitirin işi.

<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode2/5.png?raw=true" align="center" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode2/6.png?raw=true" align="center" height="300">

Bunları yaptıktan sonra sanal makineyi yeniden başlatın **(root olmalısın)**:

````reboot````

Bu ayarlardan sonra artık fiziksel makineden sanal makineye bağlanabilirsiniz.
Nasıl mı? İşte bu kadar:

- Terminalinizi fiziksel makineden açın ve aşağıdaki komutu yazın

```bash
  ssh your_42user_name@localhost -p 4242
```
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode2/7.png?raw=true" align="center" height="300">
<img src="https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/Episode2/8.png?raw=true" align="center" height="300">

Ve sanal makinenizdeki kullanıcının şifresini girerek fiziksel makinenin terminalinden sanal makineye erişebilirsiniz.

🚩**Evet, SSH bu kadardı..** 🚩

### 🛡️UFW İçin

UFW'yi İndirme:

````apt install ufw````

**UFW ile ilgili bazı komutlar**

Bize gelen tüm istekleri reddedin:

````ufw default deny incoming````

Tüm giden isteklere izin ver:

````ufw default allow outgoing````

Sistem başlangıcında UFW'yi etkinleştirin (Bunu yaptıktan sonra sanal makinenizi yeniden başlatın):

````ufw enable````

UFW'nin durumunu kontrol edin:

````ufw status```` - ````ufw status numbered```` -> kuralları numaralandır

4242 numaralı bağlantı noktasına gelen isteklere izin verin veya bu bağlantı noktasını (4242) reddedin:

````ufw allow 4242```` - ````ufw deny 4242````

<img src="https://raw.githubusercontent.com/Fartomy/42-Kickoff/master/Born2beroot/Episode2/9.png" align="center" height="300">

Kural silmek için:

````ufw delete allow 4242```` -> bu komut 'izin verilen' 4242 kuralını siler  ````ufw delete deny 4242```` -> bu da 'reddedilen' 4242 kuralını siler <br/>
````ufw delete 1```` -> 1. kuralı siler

🚩**Evet, UFW bu kadardı..** 🚩

### :godmode: Sudo için:

Sudo'yu çok çok katı kurallara göre yapılandırma (soğuk espri :/)

Sudo'yu indirin:

````apt install sudo````

Konfigürasyon ayarlarına geçmeden önce kullanıcınızı 'sudo' grubu altına ekleyin:

````usermod -aG sudo <user_name>````

Tamam, çok şey yaptık, şimdi yapılandırma ayarlarına geçelim: :d

````visudo```` -> Bu komutla konfigürasyon dosyasına girelim

Böyle bir ekran gelmeli:

<img src="https://raw.githubusercontent.com/Fartomy/42-Kickoff/master/Born2beroot/Episode2/10.png" align="center" height="300">

Buraya bazı katı kurallar ekleyin:
 
 ```bash
  Defaults     passwd_tries=3 -> 3 kere yanlış girme hakkı
  Defaults     badpass_message="Çok Yalnış Bir Şifre" -> yanlış girilirse hata mesajı
  (yanlız o yalnış değil 'yanlış') -> (yalnız o yanlız değil 'yalnız') -> sürekli okuyunca dilim sürsştü (kendi çapımda gereksiz bir eğlenmeydi kusura bakmayın)
  Defaults     requiretty -> sudo komutu için terminal gerekliliği
  Defaults     log_file="/var/log/sudo/sudo.log" -> girilen her sudo komutunun tutulacağı kayıt yeri
  Defaults     log_input, log_output -> sudo komutunun girdi ve çıktıları
  Defaults     iolog_dir="/var/log/sudo/" -> girdi ve çıktıların yolu
```

Sonuç olarak şu şekilde görünmeli:

<img src="https://raw.githubusercontent.com/Fartomy/42-Kickoff/master/Born2beroot/Episode2/11.png" align="center" height="300">

Bunları doğrulamak için 'root'tan çıkıp sudo komutu ile neler yapılabileceğini deneyebilirsiniz...

🚩**Evet, Sudo bu kadardı..** 🚩

### ⛓️ Şifre Politikası
**İlk olarak, parola değiştirme sıklığını yapılandırın:**

```bash
  nano /etc/login.defs
```
Şu ayarı bulmalısın 'pass aging control':

<img src="https://raw.githubusercontent.com/Fartomy/42-Kickoff/master/Born2beroot/Episode2/12.png" align="center" height="300">

Sonra bunu yap:

```bash
   PASS_MAX_DAYS   30
   PASS_MIN_DAYS   2
   PASS_WARN_AGE   7
```
**⚠️Evet, hepsi bu, ancak bu ayar root ve sizden (usr) sonraki kullanıcılar için geçerlidir. Kullanıcınızı ve kökünüzü değiştirmek için bunu yapın️**

Önce sana bu olayı kanıtlayayım:

````chage -l root```` ve ````chage -l <user_name>```` -> Bu yeterli bir kanıttı :d

Değiştirmek için:

````chage root```` ve ````chage <user_name>````

<img src="https://raw.githubusercontent.com/Fartomy/42-Kickoff/master/Born2beroot/Episode2/13.png" align="center" height="300">

Ne yapacağını biliyorsun..

**Şimdi şifre oluşturma kurallarımızı ekleyelim**

Bunu indirelim:

````apt install libpam-pwquality````

Bu yolu takip et:

```bash
   nano/etc/security/pwquality.conf
```
Böyle bir şeyle karşılaşacaksınız:

<img src="https://raw.githubusercontent.com/Fartomy/42-Kickoff/master/Born2beroot/Episode2/14.png" align="center" height="300">

İşte değiştirmeniz gerekenler:

```bash
   difok = 7
   minlen = 10
   dcredit= -1
   ucredit= -1
   enforce_for_root
   enforcing= 1
   maxrepeat= 3
   usercheck = 1
   dictcheck = 1
```

Açıklamalarını yazmayacağım, zaten yazılmış…

⚠️Evet, hepsi bu, ancak bunları yaptıktan sonra root, kullanıcınız ve oluşturduysanız diğer tüm kullanıcılar için şifreleri değiştirmeniz gerekiyor.

Nasıl mı?

````passwd root```` ve ````passwd <user_name>````

🏁**Ve Sonunda 2. Bölüm Biter ** 🏁

## 3️⃣ Bölüm 3 (Monitoring.sh ve Crontab Konfigürasyonları

### 🗒️ Monitoring.sh

İncelemek isterseniz yukarıda 'monitoring.sh' dosyasını paylaştım.

[Monitoring.sh](https://github.com/Fartomy/42-Kickoff/blob/master/Born2beroot/monitoring.sh)

### ⏰ Crontab (cron)

Bu komutu yazın:

````crontab -e````

Ve en alta bunu yaz:

```bash
*/10 * * * * bash /your/monitoring.sh_path
```

Açıklama yapmayacağım, dosya da yine açıklaması var..

<img src="https://raw.githubusercontent.com/Fartomy/42-Kickoff/master/Born2beroot/Episode2/15.png" align="center" height="300">

🏁 **Ve Sonunda 3. Bölüm Tüm Zorluklarla Biter ..** 🏁

## :four: Bölüm 4 (Teslim ve Ön Değerlendirme)

Artık her şey bittiğine göre, disk imzanızı alma zamanı:

Öncelikle '/goinfre' içerisine kurduğumuz dosyanın içine girip sanal makinenizi bulmalısınız. Nerede olduğunu bilmediğim için oraya gittiğini varsayıyorum.

Şunu yazmalısın:

````shasum <your_virtual_machine>.vdi```` -> Çıkması biraz vakit alabilir.

Disk imzanız geldiğinde 'signature.txt' dosyası oluşturun içine bu imzayı yapıştırın ardından ve push'layın. Bu kadar. Buraya kadar geldiyseniz 🥳TEBRİKLER!!!🥳

🏁**Ve Sonunda 4. Bölüm Burada Biter..** 🏁

## 5️⃣ Ekstralar ve Kaynaklar

### ➕  Ekstralar

1. SSH kullanarak arkadaşlarınızın sanal makinesine bağlanabilirsiniz.

2. Netchat ile arkadaşlarınızla terminal üzerinden sohbet edebilirsiniz..

Malzemeler:

- ````ifconfig```` -> yok ise ````apt install net-tools```` -> IPv4 adresi

ve

- Port

````netstat -anvp tcp | awk 'NR<3 || /LISTEN/'````

**NetChat'i Nasıl Kullanılır?**

Her şeyden önce, arkadaşınızın bilgisayarının açık olan portunu terminale yazın::

````nc -l <port>```` -> ve ENTER, ve bekle..

Ardından arkadaşınızın IPv4 adresini yazıp kendi bilgisayarınızdan port numarasını açın ve mesajlaşmaya başlayın :d

````nc <arkadaşının_IPv4_adresi> <port>````

### :brain: Kaynaklar

1. [Aptitude vs apt](https://dijitalders.net/icerik/22/2369/apt_get_ve_aptitude.html)
2. [Sudo](https://medium.com/@gokhansengun/sudo-nas%C4%B1l-kullan%C4%B1l%C4%B1r-ve-incelikleri-nelerdir-52db87d74ba)
3. [SElinux](https://www.redhat.com/en/topics/linux/what-is-selinux)
4. [AppArmor](https://apparmor.net/)
5. [SSH](https://www.hostinger.web.tr/rehberler/ssh-nedir)
6. [awk command](https://www.howtogeek.com/562941/how-to-use-the-awk-command-on-linux/)
7. [sudo config](https://www.tecmint.com/sudoers-configurations-for-setting-sudo-in-linux/)
8. [List Users Commands](https://devconnected.com/how-to-list-users-and-groups-on-linux/#:~:text=In%20order%20to%20list%20users,navigate%20within%20the%20username%20list)

🏁**Ve Sonunda README.md Burada Biter..**🏁

### Son olarak Debian Kullanıcı ve root şifrelerinizi unutursanız

🛰️ [Debian Şifre Reset'leme](https://www.youtube.com/watch?v=3Hrm3_CFKic)

<img src="https://img-s1.onedio.com/id-588fe8b2433fbcd62e12507b/rev-0/w-600/h-321/f-gif/s-f7c0954a159e38b92a9d0b67684b570b9632c14b.gif" align="right" height="550">
