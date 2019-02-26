# Emacs-k-sayollar-
Emacs özet kısayol açıklamaları

Emacs Öğrenirken yardımcı olması amacıyla Emacs Tutorial'dan aldığım komutları listeleyip özetledim </br>
<br />
<br />
<br />
Emacs kullanımını öğrenmek amaçlı oluşturduğum Özet Emacs komutları:<br />
<br />
<br />
NOT:<br />
--  C = ctrl tuşu anlamına gelmektedir.<br />
--  M = alt tuşu anlamına gelmektedir.<br />
<br />
<br />
C-x C-c            ->  Emacs ten çıkar.<br />
C-v                ->  Aşağı doğru bir ekran boyunca scroll kaydırır.<br />
M-v                ->  Yukarı doğru bir ekran boyunca scroll kaydırır.<br />
C-l (ı değil L )   ->  İmleci bulunduğu yerde sabit tutarak scroll kaydırır.<br />
<br />
Tuş kombinasyonları:<br />
<br />
.........................................<br />
..................C-p....................<br />
...............________..................<br />
...............|..._...|.................<br />
...............|../ ..|.................<br />
...............|...|...|.................<br />
...............|_______|.................<br />
......._________________________.........<br />
......|.......||.......||.......|........<br />
..C-b.|./____.||...|...||.____.|.C-f....<br />
......|......||..\_/..||...../.|........<br />
......|_______||_______||_______|........<br />
..................C-n....................<br />
.........................................<br />
<br />
M-f                ->  İleri doğru sözcük sözcük ilerleme yapar.<br />
M-b                ->  Geriye doğru sözcük sözcük ilerleme yapar.<br />
C-a                ->  Satır başına gider.<br />
C-e                ->  Satır sonuna gider.<br />
M-a                ->  Cümle başına gider.<br />
M-e                ->  Cümle sonuna gider.<br />
M->                ->  Bütün yazının en sonuna gider.<br />
M-<                ->  Bütün yazının en başına gider.<br />
C-u                ->  Komutun kaç kere çalışacağnı belirler.<br />
<br />
ÖRN: C-u 10 C-f    -> C-f komutunu 10 kere çalıştırır.<br />
ÖRN: C-u 5 a       -> ekrana 5 kere a yazar.<br />
!!İSTİSNA : C-v ve M-v komutlarında imleci satır kaydırmak olarak çalıştırır.<br />
ÖRN: C-u 6 C-v     -> İmleci 8 satır aşağı kaydırır.<br />
<br />
C-g                ->  İşlem iptal eder.<br />
<br />
NOT: Emacs komuta yanıt vermediğinde vey yanlışlıkla ESC tuşuna bastığınızdada<br />
kullanılabilir.<br />
C-u 100 C-g C-f şeklinde kullanımda ise sayısal değeri iptal ederek C-f komutunu<br />
birkere çalıştırır.<br />
<br />
Kapalı Komut Kullanımı:<br />
-----------------------<br />
Emacs e yeni başlayanlar için sorunlar yaşanmaması adına bazı komutların kullanımı<br />
engellenmiştir. bu tür komutlara kapalı komut ismi verilir. kapalı komut kullandığınızda<br />
Emacs size komutu kullanmanıza ilişkin bir soru sorar. Cevabınız evet ise space (boşluk)<br />
tuşuna basın hayır ise n yazıp enter tuşuna basın.<br />
<br />
C-x 1              ->  İmlecin seçili olduğu ekran hariç bütün ekranları kapatır.<br />
<br />
_______<br />
| <-- | Backspace tuşu gösterimi "<--" için;<br />
<br />
<--                ->  İmlecin bir sağındaki karakteri siler.<br />
C-d                ->  İmlecin bir solundaki karakteri siler.<br />
M-<--              ->  İmlecten önceki sözcüğü yok eder.(Silmekle aynı değil)<br />
<br />
!!=> Emacs yok edilen demek bir nevi kes demek denebilir. belli sınıra kadar yok edilen<br />
harf,rakam,sözcük ya da cümle Emacs in geçici hafızasında tutulur. istenilen yere istenilen<br />
zamanda geri getirme işlemi yapılabilir. Silinen bir sözcük ise geri getirelemez.Ancak geri alma<br />
işlemi ile getirilebilir ki bu da yaptığınız diğer işlemleride geri getirir.Özetle yok edilen işlem<br />
bir nevi kesilmiş yapıştırılmak üzere beklemededir.<br />
<br />
M-d                ->  İmleçten sonraki sözcüğü yok eder.<br />
C-k                ->  İmleçten satır sonuna kadar yok eder.<br />
M-k                ->  İmleçten cümle sonuna kadar yok eder.<br />
C-space ya da C-@  ->  Seçme işlemi yapar. (Yön tuşlarıyla birlikte kullanılır)<br />
C-y                ->  En son yok edilen yazıyı geri getirir(geri alma değildir..)<br />
M-y                ->  Önceki yok edilenleri geri getirir. (ilk geri getirmeden daha öncelerinide)<br />
<br />
Özet Ana işlem<br />
------------------------------------------<br />
<br />
M-w                ->  Seçileni kopyalar.<br />
C-w                ->  Seçileni keser.<br />
C-y                ->  Seçileni yapıştırır.<br />
-------------------------------------------<br />
C-x u    -----<br />
C-_          |------> Geri alma işlemi<br />
C-/      -----<br />
<br />
C-x C-f isim       ->  Var olan ya da yeni dosya yaratır.<br />
C-x C-s            ->  Kaydetme işlemi<br />
<br />
!!-> Emacs yeni dosya kaydettiğinde eskisini saklar. Böylece her zaman dosyanızın<br />
yedeği alınmış olur.<br />
Ayrıca Emacs her açtığınız dosya için bir ara bellek oluşturur.<br />
C-x C-b            ->  Arabellek listesini gösterir.<br />
C-x b isim         ->  Adı yazılan ara belleği açar. bir nevi C-x C-f komutu ile aynıdır.<br />
C-x s              ->  Ara belleği kaydeder. bir nevi C-x C-s ile aynıdır.<br />
C-z                ->  Emacs ı geçici olarak kapatır.(şimdiki sistemlerde<br />
simge durumuna küçültür.)<br />
M-x                ->  Uzun komut girişi için kullanılır.<br />
ÖRN :<br />
--  M-x replace-string<br />
--  M-x fundamental-mode<br />
--  M-x text mode<br />
--  M-x auto fill gibi;<br />
NOT: komutu tam hatırlamadığınızda M-x repl yazıp TAB tuşuna bastığınızda komutu otomatik tamamlar.<br />
<br />
Emacs bilgisayarda oluşabilecek sorunlara karşı (ani kapanma,çökme,donma v.b) otomatik kaydet<br />
işlemi yapar.<br />
deneme.txt adlı bir doyada çalışıyorunuz.<br />
Emacs ise #deneme.txt adında otomatik kayıt oluşturur.<br />
Bilgisayarınız aniden kapandı.<br />
Bilgisayarınız açıp Emacs i açıp tekrar deneme.txt doyasını açtıpınızda<br />
verileriniz yok olmuş ise ;<br />
deneme.txt açıkken (#deneme.txt değil)<br />
M-x recovery-file komutunu girin ve enter a basın.<br />
otomatik kayıt ile oluşturulmuş yedek ile dosyanız kurtarılmış olacak.<br />
<br />
C-s isim               ->  Yazılan sözcüğü ilk harfinden itibaren ileri doğru aramaya başlar.<br />
C-r isim               ->  Yazılan sözcüğü ilk harfinden itibaren geriye doğru aramaya başlar.<br />
C-x 2                  ->  Ekranı ikiye böler.<br />
C-x o                  ->  Ekranlar arası imleç geçişi yapar.(ekranı seçer)<br />
C-M-v                  ->  Diğer ekrana geçemeden o erkana göz atmanı sağlar.<br />
C-h c karakter         ->  Komutu ya da karakteri özetle açıklar.<br />
C-h k karakter         ->  Komutu ya da karakteri ayrıntılı açıklar.<br />
C-h a                  ->  Benzer karakterleri listeleyerek açıklar.<br />
ÖRN: C-h a file komutu yazıldığında içinde file geçen bütün komutları listeler.<br />
<br />
|---------------------------------------------------------------------|<br />
| --:**-TUTORIAL...............4%...............L80...........(text)..|<br />
|---------|--------------------|-----------------|--------------|-----|<br />
..........|....................|.................|..............|........<br />
....hangi dosyada......sayfanın yukarından..İmlecin kaçıncı..hangi modda..      <br />
....işlem yapıldığını..yüzde kaçı görüntü-..satırda olduğu-..çalışıldığını<br />
....gösterir...........lendiğini söyler.....nu açıklar.......söyler.......<br />
<br />
<br />
<br />
<br />
<br />
<br />
