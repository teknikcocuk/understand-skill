---
name: understand
description: Kullanıcının verdiği istemi UYGULAMADAN yalnızca ANLAR — asıl niyeti, önemsediklerini ve örtük kabulleri kendi cümleleriyle geri anlatır, "Bunu mu demek istedin?" diye sorup durur. Çıktısı onaylanmış bir anlayıştır; istem, plan veya uygulama değildir. Yalnız kullanıcı /understand ile çağırır; kendiliğinden tetiklenmez.
disable-model-invocation: true
argument-hint: <anlaşılacak istem>
---

# understand — uygulamadan anla

Kullanıcının istemi:

$ARGUMENTS

Görevin bu istemi **yerine getirmek değil, anlamak**. Anlamak burada uygulamaya giden bir ön adım değil, kendi başına biten bir iştir: kullanıcı, işe başlamadan önce ikinizin aynı şeyi kastettiğinden emin olmak istiyor. Bu skill'in çıktısı bir istem ya da plan değil, **onaylanmış bir anlayıştır** — uygulama, kullanıcının sonraki ayrı istemiyle gelir.

## Nasıl çalışırsın

1. **Kendini kullanıcının yerine koy.** İstemi yüzeydeki kelimelerle değil şu sorularla oku: bu kişi bunu neden istiyor, arkasındaki amaç ne, neyi önemsiyor, neyi önemsemiyor? Cevabı mevcut konuşma bağlamında ara — önceki mesajlar, üzerinde çalışılan iş, alınan kararlar. İstem çoğu zaman o bağlamın devamıdır; öyle oku. Bağlamdan kopma, kendi kafana göre yön veya kapsam ekleme.

2. **Anladığını kısa ve düz anlat:** asıl niyet, kullanıcının önemsedikleri, istemin dayandığı örtük kabuller, ve varsa yorumunun ikircikli kaldığı yer — ikirciği gizleme, açıkça "şurada iki türlü okunabiliyor" de. Uzunluk ölçüsü: anlamayı gösteren kadar, fazlası değil. Uzun anlatım anlamayı kanıtlamaz, sulandırır.

3. **Sonunda mutlaka sor: "Bunu mu demek istedin?" — ve DUR.** Uygulama yok, uygulamaya hazırlık yok, "istersen başlayayım" teklifi yok, tool çağrısı yok. Kapıyı kullanıcı açar; senin görevin kapının önünde net bir anlayışla beklemek.

4. **"Evet" gelirse** bu anlayışı **o istem için** kabul et: o istem bundan böyle bu anlayışla okunur. Bunu genelleştirme — oturumun geri kalanına, başka istemlere veya genel karar verme tarzına yayma; onay tek bir istemin yorumunu sabitler, başka hiçbir şeyi değil. Tek satırla teyit et ve yine dur. Uygulama, kullanıcının sonraki ayrı istemiyle gelir.

5. **"Hayır" ya da düzeltme gelirse** yeniden anla, yeniden anlat, yeniden sor. Döngü kullanıcı onaylayana kadar sürer; sabırsızlanıp uygulamaya sıçrama.

## Ton ve biçim

Doğal, konuşur gibi yaz — madde işareti ve başlık kullanma; anlayış bir metin parçası olarak akmalı, rapor gibi değil. Türkçe istem Türkçe, İngilizce istem İngilizce anlaşılır ve anlatılır.
