# Cudi-Final
 bilgi güvenliği ve kriptogafi final ödevi
 Cudi Şami 2012721308
------------------------------------------------------
![APP UI](https://github.com/cudi33/Cudi-Final/blob/821fd9c36980327e9ad5b2cdc55dd736a5637b33/photo1.PNG)  

### Ana Sayfa  
Bu sayfa, kullanıcıya hangi kriptografi aracını kullanmak istediğini seçme imkanı sunar.


Araç Seçenekleri  

🔒 AES Şifreleme:  
Gelişmiş Şifreleme Standardı (AES) ile 256-bit güvenlik sunar. Verileri şifreleyip çözme imkanı tanır.

🧬 SHA256 Hash:  
Verilerin bütünlüğünü doğrulamak ve dijital imzalar için tek yönlü SHA256 hash değerleri üretir.

![APP UI](https://github.com/cudi33/Cudi-Final/blob/df7eb828cb7ff1819d08a379fb1f7bc85a5836b3/aes%20metin%20%C5%9Fifreleme.PNG)   

🔐 ### AES Şifreleme Sayfası  
Bu sayfa, kullanıcıya AES (Advanced Encryption Standard) algoritması ile veri şifreleme ve çözme (decryption) işlemleri yapma imkanı sunar.  


Anahtar Boyutu (Key Size):
Şifreleme işlemlerinde kullanılan anahtarın uzunluğunu belirler. Genellikle 128, 192 veya 256 bit seçenekleri vardır.  
 Daha uzun anahtar = Daha güçlü şifreleme (256 bit önerilir)  

Şifreleme Modu (Encryption Mode):  
AES algoritmasının nasıl çalışacağını belirleyen mod seçimidir.  
En yaygın modlar:  
CBC (Cipher Block Chaining): Her blok bir öncekine bağlıdır. Rastgele IV gerektirir.   
GCM (Galois/Counter Mode): Hem şifreleme hem de bütünlük doğrulaması sağlar. Modern ve önerilen moddur.  
Dolgu Şeması (Padding Scheme): (yalnızca CBC gibi blok modlarında geçerlidir)
Verinin blok boyutuna uygun hale getirilmesi için eklenen dolgu yöntemidir.  
En yaygını:  
PKCS#7: Verinin sonuna eksik bayt sayısı kadar karakter ekle  

Key (Anahtar):  
AES algoritmasının şifreleme ve çözme işlemlerinde kullanılan gizli anahtardır.  
“Anahtar Üret” butonuyla rastgele güvenli bir key oluşturulabilir.  
 
IV (Initialization Vector – Başlatma Vektörü):  
CBC veya GCM gibi modlarda kullanılan başlangıç verisidir.  
Her şifreleme işlemi için farklı IV kullanılması güvenliği artırır.  
“IV Üret” ile otomatik oluşturulabilir.   


![APP UI](https://github.com/cudi33/Cudi-Final/blob/8db2b39335cf77371fbdbbd2ba86cd281cde7e43/aes%20%C5%9Fifrelenmi%C5%9F%20metin%20%C3%A7%C3%B6zme.PNG)   

AES Çözme (Decryption)   
Bu arayüz, daha önce AES algoritması kullanılarak şifrelenmiş verinin çözülmesi (decryption) için tasarlanmıştır. Kullanıcı, gerekli parametreleri girerek orijinal düz metne ulaşabilir.  
Çözme Anahtarı (Decryption Key):  
Şifrelemede kullanılan gizli anahtar buraya yazılır. AES, simetrik algoritma olduğu için aynı anahtar çözmede de kullanılır.   
Başlatma Vektörü (IV - Initialization Vector):  
Şifrelemede kullanılan IV burada tekrar girilmelidir.    
Şifrelenmiş Veri (Encrypted Data):  
AES algoritmasıyla oluşturulmuş şifreli metin bu alana yapıştırılır.  
Download Decrypted File:  
Çözülen veriyi dosya olarak bilgisayara indirir.    


![APP UI](https://github.com/cudi33/Cudi-Final/blob/8085bfaeb370dfc9ffc065ccb01e67c5b4b1a5e9/aes-resim-%C5%9Fifreleme.PNG)  

🔒 Dosya Şifreleme  
jpeg uzantılı bir görsel seçilerek yüklenip şifrelendi.  
Dosya Download Encrypted File butonuyla indirilebilir.  

![APP UI](https://github.com/cudi33/Cudi-Final/blob/cbaff06f85c13730e040a5ce575760a294477445/aes-%C5%9Fifrelenmi%C5%9F-resim-%C3%A7%C3%B6zme.PNG)  

🔓 Dosya Çözme  
Aynı anahtar ve IV kullanılarak şifreli dosya çözüldü.  
Orijinal .jpeg dosyası başarılı şekilde geri elde edildi.  
Download Decrypted File ile geri indirilebilir.  

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

![APP UI](https://github.com/cudi33/Cudi-Final/blob/2bc3b8ef672a3dafb73dd614b4797d80e268c991/hash%20metin%20%C5%9Fifreleme.PNG)  

🔐 SHA256 Hash Araçları
SHA256, bir metnin veya dosyanın sabit uzunlukta, tek yönlü bir özetini (hash) oluşturur.  
Bu sayede veri bütünlüğü doğrulanabilir, ancak geri döndürülemez (tek yönlüdür).  
Metin Girişi:  
Hash değeri üretilecek düz metin girilir.  
Veya Dosya Yükle:  
Hash değeri alınacak dosya yüklenebilir.  

![APP UI](https://github.com/cudi33/Cudi-Final/blob/e70178e8da4c195842447f06c59d899194d5b789/hash%20k%C4%B1r%C4%B1c%C4%B1.PNG)  
🛠️ Hash Kırıcı  
daha önce oluşturulmuş bir SHA256 hash’in hangi metne ait olduğunu bulmak için kullanılır. (Yalnızca sözlükte kayıtlı hash'ler için çalışır).  
Hedef SHA256 Hash:  
Tersine çözülmek istenen hash değeri girilir.  


![APP UI](https://github.com/cudi33/Cudi-Final/blob/9c8e536d92fc7af135c478725a496283ffc12b9d/hash%20ile%20dosya%20%C5%9Fifreleme.PNG)   

📄 SHA256 ile Dosya Hash (Özet) Hesaplama  
Bu sayfada, SHA256 algoritması kullanılarak nasıl hash değerinin üretildiği gösterilmektedir.    


Neden Dosya Hash Kullanılır?  
Dosyanın değişip değişmediğini kontrol etmek (bütünlük doğrulaması)  
Güvenli karşılaştırmalar yapmak (örneğin: dosya aynı mı?)  
Dijital imza öncesi içerik sabitleme  




