<img width="1495" height="493" alt="basliq" src="https://github.com/user-attachments/assets/e4226fdd-3afa-42ae-a4eb-db62ebde02f3" />
# 📊 Customer Churn Analysis with Power BI

Bu layihədə **Power BI** və **Power Query** istifadə edilərək **Customer Churn analizi** aparılmışdır.  
Layihənin əsas məqsədi müştərilərin tərk etmə davranışını anlamaq, churn səbəblərini müəyyənləşdirmək və bu məlumatlar əsasında biznes üçün qərarverməni dəstəkləməkdir.

---

## 🎯 Project Objective

Churn analizinin aparılma məqsədi:
- Şirkəti tərk edən müştəriləri tanımaq
- CRM və satış dataları əsasında churn səbəblərini müəyyənləşdirmək
- Mövcud müştərilərin əldə saxlanılmasını artırmaq
- Biznesin mənfəətini artırmaqdır

> Qeyd: Yeni müştəri qazanmaq mövcud müştərini əldə saxlamaqdan daha çox xərc tələb edir.

---

## 🗂 Dataset & Assumptions

- Dataset tarixi köhnə olduğu üçün bəzi dəyərlərə sonradan **Power BI funksiyaları** vasitəsilə əlavələr edilmişdir  
- Hesablamalar əsasən datanın öz tarixinə uyğun aparılmışdır  
- Real biznes datası ilə işlədikdə analiz daha da təkmilləşdirilə bilər

---

## 🧠 Methodology

Churn məntiqi biznes ehtiyaclarına uyğun şəkildə qurulmuşdur.  
Müştərilər 3 əsas kateqoriyaya bölünmüşdür:

- **Yeni müştərilər**
- **Daimi müştərilər**
- **Tərk etmiş müştərilər (Churn)**

Churn hesablanması fərqli tarix intervalları üzərindən aparıla bilər, lakin ümumi məntiq dəyişmir.

---

## 🧮 DAX Measures Used

Layihədə istifadə olunan əsas DAX funksiyaları:

1. **FIRSTDATE**  
   - Müştərinin ilk alış tarixini hesablamaq üçün istifadə olunub  
   - Satış cədvəlindəki tarix datasına əsaslanır  

2. **LASTDATE**  
   - Müştərinin son alış tarixini hesablamaq üçün istifadə olunub  

3. **TotalSatış (Measure)**  
   - Hər dəfə `SUM` yazmamaq üçün ayrıca measure kimi yaradılıb  

4. **Churn Logic (Custom Measure)**  
   - Biznes qaydalarına uyğun churn məntiqi qurulub  
   - Müştərilər yeni, daimi və churn kateqoriyalarına ayrılıb  

5. **DISTINCTCOUNT**  
   - Hər bir kateqoriya üzrə unikal müştəri sayı hesablanıb  

---

## 📈 Visualization

Power BI faylını yükləmədən vizuallaşdırmaya baxmaq üçün GitHub-da **PNG formatında** paylaşılmışdır.
![Uploading Churn analizi yekun vizual.png…]()
Vizual hissədə:
- **Region → Bölgə Müdiri → Satış Təmsilçisi** iyerarxiyası qurulub
- **Drill Up / Drill Down** funksionallığı istifadə edilib

Bu funksionallıq sayəsində:
- Menecer istənilən bölgə müdirinin üzərinə klik edərək onun satış təmsilçilərinin performansını izləyə bilər
- Churn olan müştərilərin:
  - hansı satış kanalından
  - hansı təmsilçidən
  - hansı müdirdən
  - hansı regiondan gəldiyi analiz oluna bilər

> Bu yanaşma real biznes mühitində qərarverməni ciddi şəkildə dəstəkləyir.

---

## 💼 Business Insights & Use Cases

Real datalarla işlədikdə churn analizi daha geniş istifadə sahəsinə malikdir:

- Churn rate-in aylar və illər üzrə izlənməsi
- CRM və Marketinq komandaları üçün müştəri profillərinin çıxarılması
- Riskli müştərilərə churn baş verməzdən əvvəl müdaxilə
- Retention və win-back kampaniyalarının qurulması
- SMS, reklam və fərdi təkliflər vasitəsilə itirilmiş müştərilərin geri qaytarılması

---

## 🛠 Tools & Technologies

- Power BI  
- Power Query  
- DAX  
- CRM & Sales Data Analysis  

---

## 👤 Author

**İsmayılov Rüfət**  
*Data Analysis | Power BI | CRM Analytics*


