# Power Automate ile Power BI Tablo Verilerini CSV Dosyası Olarak E-Postaya Gönderme

Günümüzde, iş dünyası veriye dayalı kararlar almanın önemini daha da iyi anlamış durumda. Power BI gibi güçlü bir veri analizi aracı, işletmelerin karmaşık verileri anlamalarına ve görselleştirmelerine yardımcı oluyor. Ancak verileri etkili bir şekilde paylaşma ve işbirliği yapma gerekliliği, bu süreci tamamlamak için başka bir boyut ekliyor. İşte tam bu noktada, "Power Automate" devreye giriyor. Bu makalede, Power Automate ile Power BI tablo verilerini CSV dosyası olarak e-postaya göndermenin nasıl yapıldığını öğreneceğiz. Ayrıca, bu yöntemin avantajlarına ve farklı sektörlerdeki kullanım alanlarına da bir göz atacağız.

For english please click here: https://medium.com/nerd-for-tech/sending-power-bi-table-data-as-a-csv-file-via-email-with-power-automate-d194c77f9b3e

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/c322107c-9681-405d-a36f-5f7d8918654f)


## Power Automate ile Veri İş Akışı Yönetimi

Power Automate, iş süreçlerinizi otomasyonlaştırmak ve veri iş akışlarınızı yönetmek için geliştirilen bir Microsoft hizmetidir. Bu güçlü araç, farklı uygulamalar arasında veri taşıma ve iş akışlarını oluşturma konusunda büyük bir esneklik sunar. Power BI ve Power Automate'ı bir araya getirerek, veri analizini bir adım öteye taşıyabilirsiniz.

### Avantajları:

- **Otomasyon:** Veri gönderim işlemi otomatikleştirilir, böylece manuel müdahale ihtiyacını azaltır ve zaman kazandırır.
- **Hızlı Veri Paylaşımı:** Anlık veri güncellemeleriyle, ekipler arasında hızlı ve güncel veri paylaşımını sağlar.
- **Özelleştirme Yeteneği:** Veri gönderim işlemini özelleştirebilirsiniz. İstediğiniz verileri, sıkıştırma düzeyini ve iletişim sıklığını ayarlayabilirsiniz.
- **Uygulama Entegrasyonu:** Power Automate, çeşitli uygulamalarla entegre edilebilir, bu da veri akışlarını daha geniş bir iş ekosistemine entegre etme olanağı sunar.

## Sektördeki Kullanımı

Power Automate ile Power BI tablo verilerini CSV dosyası olarak e-postaya gönderme yeteneği, birçok sektörde kullanılır:

- **Üretim:** Üretim sektörü, üretim verilerini, envanter raporlarını ve kalite kontrol sonuçlarını anında paylaşmak için bu yöntemi kullanabilir.
- **Perakende:** Perakende şirketleri, satış verilerini, envanter güncellemelerini ve müşteri analizlerini kolayca paylaşabilir.
- **Sağlık Hizmetleri:** Sağlık kuruluşları, hasta verilerini ve tıbbi raporları güvenli bir şekilde paylaşabilir.
- **Eğitim:** Eğitim kurumları, öğrenci performans verilerini ve sınav sonuçlarını hızla iletebilir.

Power Automate ile Power BI'nın entegrasyonu, veri analizini daha erişilebilir hale getirirken, iş süreçlerinizi otomatikleştirme ve veri paylaşımını hızlandırma konusunda güçlü bir araç sunar. Bu makalede, bu iki güçlü aracın nasıl birleştirileceğini ve işletmelerin veri yönetimi ve paylaşımını nasıl geliştirebileceğinizi inceleyeceğiz.

## Adım Adım Talimatlar

1. E-Posta göndermek istediğiniz Power BI raporunu açın ve tetiklemek istediğiniz sayfaya gidin.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/28cf56cc-5beb-4b61-89e6-38224da8ed81)

2. Tablo formatında iletmek istediğiniz tabloyu kopyalayıp yapıştırın. Dilerseniz tabloya ek alanlar da ekleyebilirsiniz.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/9910801d-9983-44d0-983e-ec9993edf017)

3. Tabloyu Power Automate ile tetiklenecek bir buton haline getireceğimiz için boyutunu küçültüp, raporda dilediğiniz alana yerleştirin.

  ![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/45dff9db-b376-4bbf-82f4-0eee087b773d)
  
4. Ardından tablonuz seçiliyken sağ tarafta yer alan Power Automate görseline tıklayıp dönüştürün.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/070888c7-b574-43c9-8e7a-029ee43f7bec)

   
5. Power Automate butonuna dönüştüreceğiniz görselin 3 nokta simgesine tıklayın ve ardından edit butonundan ilerleyin.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/0c6afdc2-0ae9-4e5d-9a42-81156fa92497)

6. Açılan pencerede yeni otomatik bir akış oluşturabilirsiniz ya da pencerenin aşağısında bulunan otomatik iş akışlarını kullanabilirsiniz.
   Biz yeni bir iş akışı oluşturmak için ekranın sol üst bölümünde bulunan "new" butonuna tıklayacağız.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/f275ee22-6cf3-4c21-b149-6147ced1ff53)

7. Başlangıç olarak tablo dizinimizi tanıtmak için "Initialize variable" görevini seçmeniz gerekiyor.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/75c7d34b-e3f3-4b1c-9695-3001bfacd1de)

8. Variable ismini tanımladıktan sonra csv formatında bir tablo ileteceğiniz için tipini "Array" olarak seçmeniz gerekiyor.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/fda2b0f5-6937-4079-a66a-5d087f19274a)

9. Yeni adımda e-mail göndermek istediğiniz tablo değişkenlerini tanımlamak için "Append to array variable" görevini seçmeniz gerekiyor.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/4bd44ae0-ac87-4c97-9490-467e14644615)

10. Name alanına yukarıda tanımladığımız Array ismini girdikten sonra value bölümüne Dynamic content alanından tablo alanlarınızı tanımlayın.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/dcf326be-fef8-4a45-a497-96f3dd919ffb)

11. Bir sonraki adımda tablonuzu csv formatına çevirmek için "Create CSV table" görevini kullanın.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/43a70fab-ed51-4f0f-8f39-5416787ac39a)

12. Dynamic content alanında tablo değişken adını seçin.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/2d4f0a6e-3bf3-4c1a-80b1-7a3682256bd4)

13. Bir sonraki adımda e-mailinizin içeriğini doldurarak işlemleri tamamlayın. Ardından ekranın sağ üst bölümünde bulunan "Save and apply" butonuna tıklayarak akışınızı kaydedin.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/32ba920b-6e67-450e-aa0a-2678025bce8d)

14. İş akışı başarıyla kayıt edildikten sonra rapora geri dönmek için ekranın sol bölümünde bulunan "back to report" butonuna tıklayabilirsiniz.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/d8c6c579-edd6-4a98-8df4-add255cdcb44)

15. Power Automate'i tetiklemek için rapora düzenlediğimiz iş akışı butonu geldi. Butonu tetiklemek için tıklayın.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/0f71f94c-03d1-405f-989f-8c8dbf30da3b)

16. İş akışı tetiklendi.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/39b6d250-b257-4837-8f20-2ff17edc5b1f)

17. Mail ve tablo formatındaki içeriğimiz başarılı olarak iletildi.

![image](https://github.com/aysegulyigitbi/Power-Automate/assets/127193220/105dd78c-ff20-48d0-9810-7ba35ebf3978)

Bu adımları takip ederek, Power Automate kullanarak Power BI tablo verilerini CSV dosyası olarak e-posta ile gönderebilirsiniz.
