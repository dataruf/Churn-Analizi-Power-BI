<img width="1495" height="493" alt="basliq" src="https://github.com/user-attachments/assets/e4226fdd-3afa-42ae-a4eb-db62ebde02f3" />
Bu proyektdə Power BI və daxilindəki Power Query istifadəsi ilə Churn analizini aparmışam.
Churn analizinin aparılma məqsədi bizi tərk edən müştəriləri tanımaq həmçinin CRM və uyğun satış datalarının köməyi ilə onların tərk etmə səbəblərini müəyyənləşdirmək, biznesin mənfəətini atrtırmaqdır.
Necə deyərlər yeni müştəri qazanmaq daha çox xərc tələb edir nəinki mövcud müştərini əldə tutmaq.
Dataset tarixi köhnə olduğu üçün bəzi dəyərlərə sonralar funksiya ilə əlavələr olunub. Lakin ümumi olaraq təqdim olunan datanın öz tarixinə əsasən hesablamalar aparılmışdır.
İsitfadə olunan DAX funksiyaları:
  1) Fisrtdate bu funksiya ilə ilk alış tarixi hesablanır. (satış cədvəlindəki dataya uyğun)
  2) Lastdate bu funksiya ilə son alış tarixi hesablanır. (satış cədvəlindəki dataya uyğun)
  3) Totalsatış bu funksiyada hər dəfə sum ilə hesablamamaq üçün birdəfə üçün measuere şəklində hesablanmışdır.
  4) Churn funksiyasını özümüz biznesimizə uyğun seçirik. Burada fərqli tarixlər üzərindən hesablamalar aparıla bilər lakin ümumi mahiyyət dəyişmir. Yəni 3 kateqoriyada müştərimiz olur. Yeni, daimi və tərk etmiş (churn)
  5) Distinctcount bu funksiya ilə uyğun kateqoriyadakı müştərilərin sayları hesablanıb.
Vizuallaşdırma hissəsinə PowerBI yükləmədən baxmaq üçün Githubda vizuallaşdırma bölməsindən png formatlı şəklə baxmaq olar. Burada Bölgə müdirləri-Təmsilçilər arasında kateqoriyalara baxılmış drill up funksionallığı
istifadə edilmişdir. Bu funksionallığın köməyi ilə menecer hər hansı bölgə müdirinin adına tıklayaraq onun satış təmsilçilərinin performansını izləyə bilər. Həmçinin itirlən müştərilərin əsasən hansı satış kanalından
hansı təmsilçidən, müdirdən və regiondan gəldiyini izləyə bilər. Əslində real datalarla işlədikdə daha təkmilləşmiş formada  Churn analizinin aparılması mümkündür. 
Məsələn Churn rate aylar illər üzrə izlənilə bilər, marketinq və CRM komandaları bütün bu məlumatlarla biznesə uyğun itirilmiş müştəri profillərini çıxara,
və uyğun profilli müştərilərə Churn olmadan müdaxilə etmək üçün fərqli kompaniyalar yarada bilərlər. Bundan əlavə itirilmiş müştəriləri yenidən şirkətə qazandırmaq üçün fərqli sms,reklam və s. üsullarla satış
kompaniyaları yaradılması da mümkündür.
Hazırladı İsmayılov Rüfət.
