# siberyildiz2019-writeup
Siber Yıldız -2019 | CTF (Capture The Flag)  Write-Up


<p>Merhaba arkadaşlar bu sene ikincisi d&uuml;zenlenen T&uuml;rkiye&#39;nin Siber Yıldızları yarışmasına WWarriors takımı olarak bizde katıldık ve 7. olarak tamamladık. (Kesin sonu&ccedil;lar Hen&uuml;z A&ccedil;ıklanmadı)</p>

<p>&nbsp;Takım arkadaşlarıma gayretlerinden ve &ccedil;alışmalarından dolayı teşekk&uuml;r ederim.<br />
&nbsp;<br />
&nbsp;&Ccedil;&ouml;z&uuml;mlerimizi sizlerle de paylaşayım istedim , faydalı olması dileğiyle...<br />
<em>&Ccedil;&ouml;z&uuml;mlere dair dosyaları en alttan indirebilirsiniz.</em></p>

<ol>
	<li><strong>--- Hazırlık Soruları</strong></li>
</ol>

<p>Bu sorular yarışma başlamadan &ouml;nce flag formatları nasıl olabilir anlaşılabilsin amacıyla sorulmuş sorulardı.</p>

<ul>
	<li><strong>--Hazırlık Sorusu - 1 | Bilişim şirketimizde &ccedil;alışmak ister misin ?</strong></li>
</ul>

<p>Soruyu a&ccedil;tığımızda bizi bir site karşılamış oluyor<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/hazirlik1-1.png" style="height:361px; width:640px" /><br />
&nbsp;&nbsp; &nbsp;<br />
Sağında solunda biraz gezindikten sonra kaynak kodunu g&ouml;r&uuml;nt&uuml;le yapıyoruz ve bizi bir yorum satırı karşılıyor<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/hazirlik1-2.png" style="height:394px; width:532px" />&nbsp;&nbsp; &nbsp;<br />
&nbsp;&nbsp; &nbsp;<br />
Bizde hemen dizin tarama ara&ccedil;larından birini &ccedil;alıştırıp panel adresine ulaşmaya &ccedil;alışıyoruz bu konuda dirb veya gobuster tercih edilebilir.<br />
Sonu&ccedil; olarak dizin adresini bulup girdiğimizde Flag doğrudan karşımıza geliyor<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/hazirlik1-3.png" style="height:116px; width:961px" /><br />
&nbsp;&nbsp; &nbsp;<br />
<strong>FLAG:</strong> RUp2cWFJNHNmekYvQVUyemZXQXRYbFV6Tll4cEQ0UFJGYTVLb25MN 3EwdW8ra3VxNncrVFNtRFRNenJ1VlVEVFJBQlRySklHWkU5eGw4Z3o0dWlKSEE9PQ==<br />
&nbsp;&nbsp; &nbsp;</p>

<ul>
	<li><strong>--Hazırlık Sorusu - 2 | Dikkatle incelersen cevabı bulabilirsin.&nbsp;&nbsp; &nbsp;</strong></li>
</ul>

<p>Soruyu a&ccedil;tığımızda bizi bir yazı karşılamış oluyor.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/hazirlik2-1.png" style="height:62px; width:577px" /><br />
&nbsp;Hemen ilk olarak kaynak koduna g&ouml;z atıyoruz.<br />
&nbsp;&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/hazirlik2-2.png" style="height:189px; width:640px" /><br />
İpucu olarak verilen dosyayı inceliyoruz.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/hazirlik2-3.png" style="height:225px; width:640px" />&nbsp;&nbsp; &nbsp;<br />
Karşımıza &ccedil;ıkan algoritmayı incelediğimizde, bize 4. anahtardan sonraki kısım bize bayrağı vereceğini belirtiyor.&nbsp;<br />
Bizde hemen split yapıp saydık ve karşımıza &quot;<strong>87habythi15ng151.php</strong>&quot; &ccedil;ıkmış oldu. Siz isterseniz split fonksiyonu yazabilirsiniz veya online split kullanabilirsiniz ben uğraşmadım o kadar bakınca anlaşılıyor zaten :)</p>

<p>87habythi15ng151.php cevabını md5 ile hash değerini alıyoruz ve sonucu bulmuş oluyoruz.<br />
<strong>FLAG:</strong> 28833db32bb4def17138de776fe2156a</p>

<ol>
	<li><strong>--- Yarışma Soruları</strong></li>
</ol>

<p>Şimdi ise asıl yarışma sorularına bakalım.</p>

<ul>
	<li><strong>--Soru - 1 | Bu ger&ccedil;ekten kolay</strong></li>
</ul>

<p>İndirdiğimiz <strong>dikkatli.bak.dms</strong> adında dosyayı herhangi bir text edit&ouml;r ile a&ccedil;tığımızda cevap karşımızda duruyordu.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru1-1.png" style="height:728px; width:1366px" /><br />
&nbsp;&nbsp; &nbsp;<br />
<strong>FLAG:</strong> RDcxVWV3SUFLM29RazBGV1Rnb0dsbURpWDJnckg1MUgvZ09WWFZ mbkFBWXpsNCt5K2ZBMjI2TnRKKzJvZ29xV0lEZ0NSK1lIMklWRkRyOC9XbWpOcEE9PQ==</p>

<ul>
	<li><strong>--Soru - 2 | Hala ısınmalardasın</strong></li>
</ul>

<p>A&ccedil;ılan sayfada doğrudan kaynak kodunu g&ouml;r&uuml;nt&uuml;le yaptık ve script kodu oldupğunu g&ouml;rd&uuml;k.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru2-1.png" style="height:728px; width:1366px" /><br />
&nbsp;&nbsp; &nbsp;<br />
Zamandan tasarruf etmek i&ccedil;in decode etmeye &ccedil;alışmadan &ouml;nce kopyalayıp console.log() verelim.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru2-2.png" style="height:321px; width:1365px" /><br />
&nbsp;&nbsp; &nbsp;<br />
Bir hata karşıladı bizi hemen vazge&ccedil;medik ve hataya g&ouml;z atalım istedik ve bingoo.<br />
&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru2-3.png" style="height:307px; width:1137px" /><br />
&nbsp;&nbsp; &nbsp;<br />
<strong>FLAG:</strong> NjJJdTJZRzZkS2FTa1p4Wi91dFpsdWpMRmNyOExQTXdIYUFiMkY1ZEtsS3 gveUhGQkVyUFN5QWsxbUNIb2RZOTRyeGZiSHpUeGEyQ0puQ3NFSllENkE9PQ==</p>

<ul>
	<li><strong>--Soru - 3 | &nbsp;Herşey sanal, ağ ger&ccedil;ek</strong></li>
</ul>

<p>En gıcık sorulardan birisi bu bence , son saatlere girdiğimizde &ccedil;&ouml;zebildik Cisco bilsek belki daha kolay &ccedil;&ouml;zicez :D</p>

<p>İndirdiğimiz dosyanın i&ccedil;inden pcap dosyası &ccedil;ıkıyor, bizde WireShark ile incelemeye koyuluyoruz.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-1.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Paketi incelediğimizde url gezinmeleri nmap logları ve anlamsız paketler g&ouml;r&uuml;yorduk. İ&ccedil;erisindeki dosyaları export ettiğimizde de anlamsız dosyalar bulduk işimize yaramayacak bir d&uuml;nya şey...<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-2.png" style="height:728px; width:1366px" /><br />
&nbsp;&nbsp; &nbsp;<br />
Ancak i&ccedil;erisinde işimize yarayabilecek tek bir dosya dikkatimizi &ccedil;ekti sslkeylog.log vardı. Bu nedir derseniz, secret log dosyasına sahip isek sunucu anahtarına sahip olmasak bile ssl &uuml;zerinden ge&ccedil;en trafiğin şifresini &ccedil;&ouml;zebiliriz.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-3.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Artık bu dosyaya sahip olduğumuza g&ouml;re bunu Wireshark&rsquo;a ekleyebiliriz.<strong> Edit&gt;Preferences</strong>&rsquo;e tıklayıp sol men&uuml;den <strong>Protocols&gt;SSL</strong> &lsquo;i se&ccedil;iyoruz. <strong>(Pre)-Master-Secret log filename</strong> kısmından indirdiğimiz dosyayı se&ccedil;ip kaydediyoruz. Artık SSL &uuml;zerinden ge&ccedil;en trafiği de okuyabiliriz.<br />
&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-4.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Tekrar Wireshark&rsquo;a d&ouml;n&uuml;p incelemeye devam ediyoruz. İnceleme esnasında <strong>99037582138585721057129547823.pkt</strong> isminde bir dosyaya istekte bulunulmuş.&nbsp;<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-5.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
İsteği daha ayrıntılı g&ouml;rmek i&ccedil;in &uuml;zerine sağ tıklayıp<strong> Follow&gt;Http Stream</strong> derseniz giden Get isteğini g&ouml;rebilirsiniz.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-6" /><img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-6.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Yanıt olarak OK (200) d&ouml;nm&uuml;ş ama herhangi bir dosya gelmemiş. Bizde uzak sunucudan bu dosyayı indirdik. Dosyayı nasıl a&ccedil;abileceğimiz konusunda kısa bir araştırma yaptık ve Cisco&rsquo;nun kendi cihazları i&ccedil;in geliştirdiği bir network simulator olan <strong>Cisco Packet Tracer </strong>i&ccedil;in oluşturulan bir dosya olduğunu bulduk ve programı indirdik.</p>

<p>&nbsp;Programı a&ccedil;ıp dosyasımızı i&ccedil;erisine &ccedil;ağırdık.<br />
&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-7.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
&nbsp;&Ouml;yle aradık b&ouml;yle aradık programın girmediğimiz yeri kalmadı ama işimize yarar bir şey bulamadık.<br />
&nbsp;En son Router cihazının config ayarlarını kaydetmemiz bizi bir sonraki aşamaya taşıdı.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-8.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Kaydedilen dosyayı a&ccedil;tığımızda username ve password bulunuyordu.<br />
&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-9.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Bu şifreyi nasıl &ccedil;&ouml;zebiliriz araştırmasını yaparken online bir ara&ccedil; bulduk. (http://www.ifm.net.nz/cookbooks/passwordcracker.html)<br />
Şifreyi yazdığımızda &quot;<strong>flag md5(r0uterP@ss)</strong>&quot; şeklinde cevap d&ouml;nd&uuml; ve md5 alıp soruyu &ccedil;&ouml;zd&uuml;k.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru3-10.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
<strong>FLAG:</strong> be4a5b6e929ad88d4f88ad7435ed2eb9&nbsp;&nbsp; &nbsp;</p>

<ul>
	<li><strong>--Soru - 4 | OBURIX&rsquo;in şifresi</strong></li>
</ul>

<p>Karşımızda yine bir pcap dosyası &ccedil;ıkıyor, a&ccedil;ıyor ve incelemeye başlıyoruz.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru4-1.png" /><br />
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;<br />
Sorunun adında bir ipucu vardı ve inceleme esnasında OBEX protokol&uuml; dikkatimizi &ccedil;ekti. Bu protokol dosya alışverişinde kullanıldığından dolayı, bluetooth ile png dosyası g&ouml;nderilmiş oldugunu d&uuml;şenerek png.chunk.data filtresi kullanarak png datasına sahip paketi bulmayı d&uuml;ş&uuml;nd&uuml;k, gelen sonu&ccedil;larda info sekmesinde usom.png yazıyordu, doğru paketi bulmuştuk.</p>

<p>İlgili frame&rsquo;e <strong>OBEX Protocol&gt;Portable Network Graphics</strong>&rsquo;e sağ tıklıyoruz ve <strong>Show Packet Bytes</strong>&rsquo; a basıyoruz. Flag karşımıza geliyor.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru4-2.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
<strong>FLAG:</strong> KOJwaTdxRUoydk9Ea3VpTW8rRVM1UT09</p>

<p>&nbsp;</p>

<ul>
	<li><strong>--Soru - 5 | Emeğe saygı</strong></li>
</ul>

<p>Bizi &ccedil;ok uğraştıran sorulardan birisiydi. Ger&ccedil;ekten soruyu hazırlayan kişinin emeğine saygı duyulacak cinsten :)</p>

<p>Sayfayı a&ccedil;tığımızda &ldquo;Cok calistik,cok. Emege saygi gosterin, kaynak belirtin.&rdquo; şeklinde bir yazı karşılıyordu.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru5-1.png" /></p>

<p>Kaynak belirtin kısmı bize bir ipucu veriyordu, bende baştan &ouml;yle yaptım yazılarımdan birinin altına kaynak olarak koydum :) sonra tıkladığımızda başka sayfa hem yavaş a&ccedil;ılıyor hem değişiyordu.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru5-2.png" /></p>

<p>Ekrana &ccedil;ıkan yazı bizi heyecanlandırmıştı. Kaynak belirtenlere cevap g&ouml;nderdik diyor olması benim sunucuya bir giriş olduğunu s&ouml;yl&uuml;yordu. &Ouml;yleyse sunucuya gelen istekleri yakalamam gerekiyordu. Herhangi bir sniffer aracı işimi g&ouml;recekti bende snifferı a&ccedil;ıp beklemeye başladım. Kaynak g&ouml;sterdiğim yere girip linke tıkladığımda y&ouml;nlendirme yapıp geri referer isteği g&ouml;ndermiş oldu.&nbsp;<br />
&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru5-3.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
A&ccedil;ık&ccedil;ası sorunun b&ouml;yle &ccedil;&ouml;z&uuml;leceğini hi&ccedil; d&uuml;ş&uuml;nm&uuml;yordum :)</p>

<p><strong>FLAG:</strong> aFZPL0hkSjhvaThneGdIdkFMcUd1UFZLOGNhMGxGSG1lak1VbXlROFVG OFdxVWI3bjFYTW10bVVFMk5ZdTVQV3daRSsxWFZsbmZWZ3dLOFMveHZxQnc9PQ==</p>

<ul>
	<li><strong>--Soru - 6 | Reklam arası bitti film başlıyor</strong></li>
</ul>

<p>Soru bize &quot;<strong>dump.scm</strong>&quot; adlı dosyayı verdi. Biraz araştırma sonucu .scm uzantılı dosya eski TV kutularındaki kanal listesi d&uuml;zenleme formatıydı a&ccedil;mak i&ccedil;in uygun edit&ouml;r&uuml; bulup indirdik ve dosyayı a&ccedil;tık.<br />
&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru6-1.png" style="height:556px; width:1023px" /></p>

<p>Hızlıca linke giriyoruz ve &ccedil;ok sevdiğim filmlerden olan Interstellar filmini karşımızda buluyoruz. Filmin sahnesini izlerken arkadan k&ouml;t&uuml; bir cızırtı sesi geliyor. Hemen videoyu mp3 e &ccedil;evirip analiz ediyoruz.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru6-2.png" /></p>

<p><strong>FLAG</strong>: c6a107c3072414436a6acf122bf4f349</p>

<ul>
	<li><strong>--Soru - 7 | Bir bakan var bir de aranan&nbsp;&nbsp; </strong>&nbsp;</li>
</ul>

<p>Soruya girdiğimizde alttaki hash karşımıza &ccedil;ıktı.</p>

<p>0827206450376af3dce61d788ddeba21f58dba35257fdb43c1872c096a36287f</p>

<p>Virustotal &uuml;zerinden hashi arattığımızda yorumlar kısmında bize bir link vermişti.</p>

<p>https://www.virustotal.com/tr/file /0827206450376af3dce61d788ddeba21f58dba35257fdb43c1872c096a36287f/analysis/</p>

<p><strong>http://85.111.95.19/a5d8bccb8e1255fc72340eddab8be601-mobile01/cyb3rStar.zip (Pass: Cyberstar_2018!. )</strong></p>

<p>&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru7-1.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Dosyayı indirip i&ccedil;inden &ccedil;ıkan uygulamanın, bir kopyasının uzantısını zip yapıp kla&ouml;re &ccedil;ıkararak i&ccedil;indekileri incelemeye başladık. \res\drawable dizinindeki resimler dikkatimizi &ccedil;ekti birer birer incelemeye başladık.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru7-2.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Fotoğrafları analiz ettiğimizde i&ccedil;erisinde her birinde <strong>thankyoucyberstar.gif</strong> isminde yaklaşık 200 dosya vardı.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru7-3.png" /></p>

<p>Ancak sadece birinde farklı bir dosya bulunuyordu <strong>ortakoy.jpg</strong> i&ccedil;erisinde lakin oda şifreliydi.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru7-4.png" /></p>

<p>Bir başka resmin exif bilgilerinde ise karmaşık karakterlerden oluşan string dikkatimizi &ccedil;ekti ve şifreli dosya i&ccedil;in bu stringi kullandık şifre doğruydu ve bizi bir sonraki adıma g&ouml;t&uuml;rd&uuml;.</p>

<p><img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru7-5.png" /><br />
&nbsp;İ&ccedil;inden &ccedil;ıkan <strong>hadibul.b64</strong> dosyası base64 ile şifrelenmiş bir dosyaydı hemen online bir decoder bulup (http://base64converter.com/) decode ettik. Dosyayı incelediğimizde apk dosyası olduğunu farkettik telefona kurup &ccedil;alıştırdığımızda ise cevap karşımızdaydı.<br />
&nbsp;<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru7-6.png" /></p>

<p><strong>FLAG:</strong> 05a24ab2b3f6e4d8309575dca5388eeb</p>

<ul>
	<li><strong>--Soru - 8 | Karekod okuyucu</strong></li>
</ul>

<p>Giriş ekranı ve kullanıcıları listeleyen bir sayfa vardı, basit kombinasyonlarla giriş yapmayı denedik fakat bir sonuca ulaşamadık.</p>

<p>Ardından kullanıcıların bulunduğu sayfaya g&ouml;z attığımızda &quot;Y&ouml;neticiye &ouml;zel oluşturulan QR kodu giriniz&quot; ifadesi bulunuyordu.&nbsp;<br />
&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru8-1.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Hemen aklımıza SQL Inj. ile bir QR kodu oluşturmak geldi ve online bir siteden &nbsp;<strong>&#39; or 1=1#</strong> şeklinde bir QR kod oluşturduk.<br />
&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru8-2.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Oluşturduğumuz kodu servera g&ouml;nderdiğimizde beklediğimiz sonucu almıştık kullanıcıları listelemişti. Bir tane kullanıcı (admin) ve iki tane hash değeri vardı.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru8-3.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Hash değerlerini decode ettiğimizde, hashlerden birinin değeri <strong>admin0123456789 </strong>du ve giriş yaptığımızda flag karşımızdaydı.<br />
&nbsp;&nbsp; &nbsp;<img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru8-4.png" /></p>

<p><strong>FLAG:</strong> TWtCM1JTRVZydWpqekNVQzBNR09NUHM2SFh2VTNQbFA5WE5PenQx MWtHa3lDL21ydnJEVXFjZUQycHA1Vloxc0dockh1M28xZXBnd3FkUXJrdEd4REE9PQ==</p>

<ul>
	<li><strong>--Soru - 10 | Herşeyi de sana servis edecek değiliz</strong></li>
</ul>

<p>Servis gibi servis diye bir web uygulaması bizi karşılıyordu. Giriş yapma ve kayıt olma sayfaları vardı. Kayıt olma sayfasında kayıtların devre dışı bırakıldığı s&ouml;yleniyordu. Giris yap sayfasındada demo ile giris yap şeklinde bir link bulunuyordu.</p>

<p>Linkin Adresi: ws/ws.php<strong>?islem=girisYap&amp;kullaniciAdi=demo&amp;parola=demo</strong> şeklindeydi. Kullanıcı adını admin olacak şekilde değiştirdiğimizde kullanıcı mevcut değil şeklinde mesaj alıyorduk. Bizde islem paramteresini değiştirerek ws/ws.php<strong>?islem=kayitOL&amp;kullaniciAdi=admin&amp;parola=admin</strong> şeklinde bir request yaptık. Ancak sonu&ccedil; ge&ccedil;ersiz method şeklindeydi. &nbsp;Bu sefer y&ouml;ntem değiştirerek <strong>GET </strong>metodunu <strong>POST </strong>metoduyla değiştirince kayit olabildik.</p>

<pre class="brush:ps;">
POST /86d37fde1020e969eca3d6436bddb4f5-04/ws/ws.php?islem=kayitOl&amp;kullaniciAdi=admin&amp;parola=admin&amp;email=test HTTP/1.1
Host: 85.111.95.28
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:65.0) Gecko/20100101 Firefox/65.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8
Referer: http://85.111.95.28/86d37fde1020e969eca3d6436bddb4f5-04/giris.html
Accept-Language: en-US,en;q=0.9
Cookie: PHPSESSID=ttjj1d2lcpoagr63qp2596fqb4
Connection: close
Content-Type: application/x-www-form-urlencoded
Content-Length: 45

islem=kayitOl&amp;kullaniciAdi=admin&amp;parola=admin&amp;email=test</pre>

<p>Yani burada admin:admin şeklinde kayıt olduk. Giriş yaptığımızda admine &ouml;zel bir sayfa bizi karşılıyordu ve bizden kod istiyordu.</p>

<p>Buralar &ccedil;ok g&uuml;zel, giriş yap sen de gel bence.<br />
====================================<br />
Admin Kullanıcısı</p>

<p>Doğru cevabı girmen i&ccedil;in deneme hakkın 10 tane. Bulduğunda &ouml;d&uuml;l&uuml;n&uuml; de alacaksın. Ona g&ouml;re:&nbsp;&nbsp; <img alt="" src="http://mucahittopal.com/upload/dosya/SiberYildiz2019-Resimler/soru10-1.png" /><br />
&nbsp;&nbsp; &nbsp;<br />
Sayfanın kaynak kodunu g&ouml;r&uuml;nt&uuml;lediğimizde, yorum satırı olarak bir php kodu g&ouml;r&uuml;n&uuml;yordu.<br />
&nbsp;&nbsp; &nbsp;</p>

<pre class="brush:php;">

function generateRandomString($length = 6) {
&nbsp; &nbsp; $characters = &#39;0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ&#39;;
&nbsp; &nbsp; $charactersLength = strlen($characters);
&nbsp; &nbsp; $randomString = &#39;&#39;;
&nbsp; &nbsp; for ($i = 0; $i &lt;= $length; $i++) {
&nbsp; &nbsp; &nbsp; &nbsp; $randomString .= $characters[rand(0, $charactersLength - 1)];
&nbsp; &nbsp; }
&nbsp; &nbsp; return $randomString;
}

function decryptFile($source, $key, $dest)
{
&nbsp; &nbsp;
&nbsp; &nbsp; $key = substr(sha1($key, true), 0, 16);

&nbsp; &nbsp; $error = false;
&nbsp; &nbsp; if ($fpOut = fopen($destc, &#39;w&#39;)) {
&nbsp; &nbsp; &nbsp; &nbsp; if ($fpIn = fopen($source, &#39;rb&#39;)) {
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; // Get the initialzation vector from the beginning of the file
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; $iv = fread($fpIn, 16);
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; while (!feof($fpIn)) {
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; // we have to read one block more for decrypting than for encrypting
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; $ciphertext = fread($fpIn, 16 * (FILE_ENCRYPTION_BLOCKS + 1));&nbsp;
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; $plaintext = openssl_decrypt($ciphertext, &#39;AES-128-CBC&#39;, $key, OPENSSL_RAW_DATA, $iv);
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; // Use the first 16 bytes of the ciphertext as the next initialization vector
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; $iv = substr($ciphertext, 0, 16);
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; fwrite($fpOut, $plaintext);
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; }
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; fclose($fpIn);
&nbsp; &nbsp; &nbsp; &nbsp; } else {
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; $error = true;
&nbsp; &nbsp; &nbsp; &nbsp; }
&nbsp; &nbsp; &nbsp; &nbsp; fclose($fpOut);
&nbsp; &nbsp; } else {
&nbsp; &nbsp; &nbsp; &nbsp; $error = true;
&nbsp; &nbsp; }
&nbsp; &nbsp; //key gen with private algorithms&nbsp;
&nbsp; &nbsp; //same private algorithms used for check
&nbsp; &nbsp; if($keys=generateRandomString(6)) {
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;$k1 = strpos($key,$keys[0]);
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;if($k1===false) {
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;$errors=true;
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;} else {
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;if(strpos($key,$keys[1]) === false)
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;$errors=true;
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;else {
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;if(strpos($key,$keys[2]) === false)
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;$errors=true;
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;else {
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;if(intval($keys[5]) &lt; 9 and intval($keys[5]) &gt;= strlen(&#39;12345678&#39;)) {
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;if($keys[4] == $key[3]) {
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;if($keys[6] == rand(0,9)) {
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;return $keys;
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;}
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;}
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;}
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;}
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;}
&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;}
&nbsp;&nbsp; &nbsp;}
&nbsp;&nbsp; &nbsp;return false;
}

function doNotGenerateRandomString($lenght = 4 ){
&nbsp;&nbsp; &nbsp;...
}

function keyChecker($keys) {
&nbsp; &nbsp; ...
}

$pass = &#39;KENDI ADMIN PAROLANIZI BURAYA YAZIN&#39;;
$hash = md5($pass);
//anahtar uretiliyor
$key &nbsp;= decryptFile(PATH, $pass, DEST_PATH);
$rand = generateRandomString(6);
//gecerli bir anahtar mı diye kontrol ediliyor
if(keyChecker($key))
&nbsp;&nbsp; &nbsp;echo &#39;tebrikler&#39;;</pre>

<p>&nbsp;&nbsp; &nbsp;<br />
Kodu incelemeye koyulduk. Bizden istenen algoritmayı &ccedil;ıkarmaya &ccedil;alıştık. Bulduğumuz sonu&ccedil;lar ş&ouml;yleydi:</p>

<ul>
	<li>- sha1 ile kullanıcının şifresinin hashini al,</li>
	<li>- hashin ilk 16 karakterini &uuml;retici key olarak kullan,</li>
	<li>- keyin 1,2,3. karakterleri &uuml;retici key i&ccedil;inde olmalı,</li>
	<li>- keyin 6. karakteri 8 olmalı,</li>
	<li>- ge&ccedil;ici keyin 4 karakteri keyin 5. karakteri olmalı,</li>
	<li>- keyin 7. karakteri 0-9 arası random bir sayı olmalı (bunuda deneme yanılma y&ouml;ntemiyle bulabiliriz)</li>
</ul>

<p>Bu şartları sağlayan bir key oluşturmamız gerekiyordu.</p>

<p>Admin parolası i&ccedil;in ge&ccedil;erli anahtarı <strong>dddd38&lt;0-9&gt;</strong> şeklinde oluşturduk.<br />
Doğruluğu sağlandığında bize flagı vermiş oldu.<br />
&nbsp;<br />
<strong>FLAG:</strong> U1RpeWtYWWN6ZEw3b1VqRnhPcVhFVlZBbmtMdjJhRmRkTnFYUUV0Nkg 5MGRacDUwOXlBKyt6NXVwSG9OOXRhNzgzaSsvVWh5Y2c3UTNYb29kTmhpWXc9PQ==</p>

<p><br />
<a href="http://bc.vc/9yVt8iC" target="_blank">Siber Yıldız 2019 Soruları İndir / Download</a></p>									</p>
