# Natural Writing v2: Evaluation suite

## Purpose and method

This is a diagnostic suite for the skill's decisions, not an AI-authorship benchmark. All baselines are original test fixtures created for this project. Each revision is constrained to the facts in its baseline; no external detail is added.

The main suite contains five English and five Turkish cases across personal/application writing, academic or scientific explanation, professional email, informal explanation, and article/report prose. Four negative tests check whether the skill can leave already effective prose alone.

For each case, the review asks:

1. Did the revision preserve facts, claim strength, purpose, and necessary terminology?
2. Did it preserve or appropriately infer the writer's voice and relationship to the reader?
3. Did it reduce unsupported importance, promotional language, vague attribution, filler, or repetitive structures?
4. Did syntax and paragraph shape follow the content rather than a variation target?
5. Did the result become too casual, artificially irregular, or over-edited?
6. Which tempting rule, if applied mechanically, would have caused damage?

## Coverage

| ID | Language | Genre | Primary stress test | Result |
|---|---|---|---|---|
| EN-1 | English | College application | Concrete reflection without invented drama | Pass |
| EN-2 | English | Scientific explanation | Precision without removing useful passive/nominal forms | Pass |
| EN-3 | English | Professional email | Concision without losing courtesy | Pass |
| EN-4 | English | Informal explanation | Natural register without forced slang | Pass |
| EN-5 | English | Report prose | Source scope and neutral interpretation | Pass |
| TR-1 | Turkish | Application/personal | Turkish voice and concrete reflection | Pass |
| TR-2 | Turkish | Scientific explanation | Formal register and technical terminology | Pass after suffix-density check |
| TR-3 | Turkish | Professional email | Direct request with appropriate politeness | Pass |
| TR-4 | Turkish | Informal explanation | Natural Turkish syntax, no translationese | Pass |
| TR-5 | Turkish | Report/article | Neutral claims and readable data reporting | Pass |
| EN-N1 | English | Personal negative test | Preserve an em dash, fragment, and meaningful triad | No edit |
| EN-N2 | English | Methods negative test | Preserve conventional passive voice | No edit |
| TR-N1 | Turkish | Conversational negative test | Preserve colloquial rhythm and omitted subjects | No edit |
| TR-N2 | Turkish | Methods negative test | Preserve formal passive morphology | No edit |

---

## English cases

### EN-1 — College application paragraph

**Baseline**

> Volunteering for three months at the Riverside Repair Café was a transformative experience that taught me the importance of patience, collaboration, and problem-solving. One particularly meaningful moment occurred when I spent forty minutes replacing the battery in Mrs. Flores's laptop, but the fan still did not start. After she asked me to explain each step, I checked the machine again and found that I had left a connector loose. This experience not only enhanced my technical abilities but also fostered a deeper appreciation for communication. It underscored the fact that engineering is not just about fixing devices, but about helping people. I will carry this valuable lesson with me as I pursue my academic journey.

**Revision**

> During my three months at the Riverside Repair Café, I spent forty minutes replacing the battery in Mrs. Flores's laptop. The fan still would not start. When she asked me to explain each step, I opened the machine again and found the loose connector I had missed. That mistake made me slow down and say what I was doing instead of treating the person across the table as another device to fix. I left the café more careful with both machines and explanations.

**Assessment**

- **What changed and why:** The revision leads with the supplied scene, removes generic evaluative phrases and the automatic three-part lesson, and lets the reflection arise from the mistake. The final sentence develops the machine/person connection without claiming a life-changing transformation.
- **Meaning and voice:** The duration, person, device, error, and lesson are preserved. The voice is more personal but not made confessional or theatrical.
- **Casualness or artificial irregularity:** The short second sentence emphasizes the failed repair; it is content-led rather than randomly inserted. Diction remains suitable for an application.
- **Overcorrection check:** The specificity rule could have invited invented sensory details or a fabricated outcome for Mrs. Flores. None were added. The anti-triad rule did not merely replace three virtues with two synonyms; it removed the unsupported list and retained the demonstrated lesson.

### EN-2 — Scientific explanation

**Baseline**

> Photosynthesis is a crucial and remarkable biological process that plays a pivotal role in sustaining life on Earth. During the light-dependent reactions, light energy is harnessed by chlorophyll and water is split, leading to the production of ATP and NADPH and the release of oxygen. Subsequently, the Calvin cycle utilizes these important molecules to facilitate the conversion of carbon dioxide into carbohydrate precursors. This sophisticated two-stage mechanism not only provides plants with energy-rich compounds but also underscores the interconnected nature of life and the atmosphere.

**Revision**

> Photosynthesis converts light energy into chemical energy. In the light-dependent reactions, chlorophyll absorbs photons, electron transport generates ATP and NADPH, and the splitting of water releases oxygen. The Calvin cycle then uses ATP and NADPH to reduce carbon dioxide and build carbohydrate precursors. The two stages are linked by the energy carriers produced in the first and consumed in the second.

**Assessment**

- **What changed and why:** Promotional adjectives and unsupported planetary significance were replaced by mechanism. “Subsequently” became a simpler temporal link; the last sentence now explains the relation between the stages instead of adding a moral.
- **Meaning and voice:** The scientific content is preserved and made more precise. “Carbohydrate precursors” avoids implying that the cycle directly produces finished glucose in one step.
- **Casualness or artificial irregularity:** The register remains academic and compact. Sentence lengths vary only because one sentence defines the process and two describe its stages.
- **Overcorrection check:** A mechanical direct-verb or anti-nominalization rule might remove the conventional passive “linked” or the technical noun “splitting.” V2 retains both because they are clear and scientifically useful.

### EN-3 — Professional email

**Baseline**

> Subject: Request Regarding the Upcoming Analysis Deadline
>
> Dear Dr. Chen,
>
> I hope this message finds you well. I am writing to reach out regarding the analysis that is currently due this Friday. Unfortunately, the freezer failure on Tuesday resulted in the loss of two sample batches, creating an unexpected challenge for the project. In light of this situation, I wanted to respectfully ask whether it might be possible to extend the deadline until next Wednesday. This additional time would allow me to repeat the runs and provide a more robust and comprehensive analysis. Thank you very much for your time, consideration, and understanding.
>
> Best regards,  
> Maya

**Revision**

> Subject: Request to extend analysis deadline to Wednesday
>
> Dear Dr. Chen,
>
> Tuesday's freezer failure destroyed two sample batches, so I need to repeat those runs before I can complete the analysis. Could I move Friday's deadline to next Wednesday? The extra time would let me include the replacement results rather than submit an incomplete analysis.
>
> Thank you for considering the request.
>
> Best,  
> Maya

**Assessment**

- **What changed and why:** The email states the cause, request, and consequence directly. Generic opening language, duplicated request framing, and inflated adjectives were removed.
- **Meaning and voice:** Every operational fact is preserved: Tuesday, two batches, Friday, next Wednesday, and repeat runs. The request remains respectful.
- **Casualness or artificial irregularity:** “Could I” and “Thank you” keep appropriate professional warmth. The revision is direct, not brusque.
- **Overcorrection check:** Treating every non-informational sentence as filler could remove courtesy entirely. V2 retains a brief thanks because relationship management is a real function in email.

### EN-4 — Informal explanatory prose

**Baseline**

> Sunsets are a fascinating natural phenomenon that showcase the remarkable way light interacts with our atmosphere. As the sun approaches the horizon, its light travels through a greater amount of atmosphere. This causes shorter blue wavelengths to be scattered away, while the longer red and orange wavelengths remain visible. Dust, smoke, and clouds can also influence the colors that appear. Essentially, this process highlights the beauty and complexity of nature, turning the sky into a vibrant tapestry of colors. It is not just a pretty sight, but also a powerful reminder of the science all around us.

**Revision**

> At sunset, sunlight reaches us through more of the atmosphere than it does at noon. Air molecules scatter the shorter blue wavelengths more strongly, so much of that blue light is redirected before it reaches your eyes. The red and orange wavelengths make it through in greater proportion. Dust, smoke, and clouds can change the colors, which is why two sunsets from the same place may look different.

**Assessment**

- **What changed and why:** The revision removes scenic praise and a canned “not just” ending, then uses the available space for one useful qualification about day-to-day variation.
- **Meaning and voice:** The core explanation and the supplied qualification about dust, smoke, and clouds are preserved. The revision adds no facts beyond the baseline.
- **Casualness or artificial irregularity:** Second person appears once to fit an informal explanation, without slang or choppy fragments.
- **Overcorrection check:** “Fascinating” and “vibrant” are not forbidden. They were removed because they displaced explanation in this passage, not because the words themselves are suspect.

### EN-5 — Article/report prose

**Baseline**

> The West Ward library's innovative delivery pilot achieved remarkable results and demonstrated the transformative potential of community-centered services. Of the 120 households invited to participate, 72 returned the follow-up survey. An impressive 49 respondents used the delivery service at least once, while 31 used it twice or more. Average reported wait time fell from 18 minutes in the first month to only 7 minutes in the third month. These findings clearly underscore the program's success and highlight a promising path forward for modern libraries everywhere.

**Revision**

> The West Ward library invited 120 households to join its delivery pilot; 72 completed the follow-up survey. Of those respondents, 49 reported using the service at least once and 31 reported using it twice or more. Average reported wait time fell from 18 minutes in the first month to 7 minutes in the third. Because the figures come from respondents rather than all invited households, they describe use among the survey group and do not establish uptake across the full pilot population.

**Assessment**

- **What changed and why:** Promotional evaluation and a universal recommendation were removed. The revision identifies the denominator and the self-report limitation, which matter more than an abstract success claim.
- **Meaning and voice:** All numbers and time points are preserved. “Reported” is repeated deliberately to keep source scope clear.
- **Casualness or artificial irregularity:** The register remains neutral report prose. Repetition is retained where terminological consistency prevents overclaiming.
- **Overcorrection check:** A blanket anti-repetition rule might vary “reported” into less precise synonyms. V2 prioritizes source clarity over lexical variety.

---

## Turkish cases

### TR-1 — Başvuru yazısı / kişisel anlatı

**Temel metin**

> Belediye kütüphanesinde sekiz hafta gönüllü olarak çalışmak benim için son derece dönüştürücü ve ufuk açıcı bir deneyim oldu. Bu süreçte iletişim, empati ve problem çözme becerilerimi geliştirme fırsatı buldum. Özellikle 12 yaşındaki Ece'nin katalog tabletindeki menüyü üç kez sorması dikkat çekici bir andı. İlk başta aynı açıklamayı tekrarladım; daha sonra sorunun Ece'de değil, benim açıklamamda olduğunu fark ettim ve tek sayfalık görsel bir yönerge hazırladım. Bu deneyim, yalnızca topluma katkı sağlamanın önemini değil, aynı zamanda etkili iletişimin dönüştürücü gücünü de gözler önüne serdi.

**Revizyon**

> Belediye kütüphanesindeki sekiz haftalık gönüllülüğüm sırasında, 12 yaşındaki Ece katalog tabletinin menüsünü üç kez sordu. İlk iki seferde aynı cevabı biraz daha yavaş tekrarladım. Üçüncüsünde sorunun Ece'de değil, açıklamamda olduğunu anladım. Menüyü adım adım gösteren tek sayfalık bir yönerge hazırladım. O gün, anlaşılmayan bir şeyi yeniden söylemekle yeniden anlatmanın aynı olmadığını öğrendim.

**Değerlendirme**

- **Ne değişti, neden:** Soyut beceri listesi ve büyük önem iddiası çıkarıldı; verilen olay ve ondan doğan sınırlı çıkarım öne alındı.
- **Anlam ve ses:** Süre, kişi, üç soru ve görsel yönerge korunuyor. Ses kişisel fakat yapay biçimde dramatik değil.
- **Aşırı gündeliklik / yapay düzensizlik:** Kısa üçüncü cümle fark ediş anını taşıyor; sırf ritim çeşitlensin diye eklenmedi.
- **Aşırı düzeltme kontrolü:** Somutluk kuralı, kütüphanenin görünümü ya da Ece'nin tepkisi gibi olmayan ayrıntıları uydurmaya yol açabilirdi. Eklenmedi.

### TR-2 — Akademik/bilimsel açıklama

**Temel metin**

> Polimeraz zincir reaksiyonu, moleküler biyoloji alanında kritik bir rol oynamakta ve belirli DNA bölgelerinin çoğaltılmasını sağlamaktadır. İlk aşamada çift sarmal yüksek sıcaklıkta ayrılmaktadır. Ardından primerler hedef dizilere bağlanmakta ve DNA polimeraz yeni zincirleri sentezlemektedir. Bu aşamaların tekrarlanması sonucunda DNA miktarı ideal koşullarda yaklaşık üstel olarak artmaktadır. PCR; tanı, dizileme hazırlığı ve araştırma amacıyla kullanılmakta, ürünün özgüllüğü ise primer tasarımı ile reaksiyon koşullarına bağlı bulunmaktadır. Bu güçlü yöntem, bilimsel araştırmaların ilerlemesine önemli katkılar sağlamakta ve modern biyoteknolojinin dönüştürücü potansiyelini gözler önüne sermektedir.

**Revizyon**

> Polimeraz zincir reaksiyonu (PCR), belirli bir DNA bölgesini çoğaltır. Her döngüde çift sarmal yüksek sıcaklıkta ayrılır, primerler hedef dizilere bağlanır ve DNA polimeraz yeni zincirleri sentezler. Ürünler sonraki döngülerde kalıp görevi gördüğü için hedef DNA miktarı ideal koşullarda yaklaşık üstel biçimde artar. PCR; tanı, dizileme hazırlığı ve araştırma gibi farklı amaçlarla kullanılır, ancak elde edilen ürünün özgüllüğü primer tasarımına ve reaksiyon koşullarına bağlıdır.

**Değerlendirme**

- **Ne değişti, neden:** Tekrarlanan `-maktadır` yapıları azaltıldı, genel övgü yerine mekanizma ve bir sınırlama getirildi. Kısaltma ilk kullanımda tanımlandı.
- **Anlam ve ses:** Temel aşamalar ve üstel artış korunuyor. “İdeal koşullarda yaklaşık” ifadesi, gerçek reaksiyon veriminin kusursuz olmadığını belirterek iddia gücünü ayarlıyor.
- **Aşırı gündeliklik / yapay düzensizlik:** Dil bilimsel kalıyor; teknik terimler sadeleştirme uğruna kaldırılmadı. Son cümledeki edilgen `kullanılır` türün doğal bir parçası olarak korundu.
- **Aşırı düzeltme kontrolü:** `-mektedir` karşıtı katı bir kural metni gündelikleştirebilir, bütün edilgenleri kaldırmak da yöntem dilini bozabilirdi. Değişiklik yalnızca tekrar ve sertlik yaratan yoğunluğa uygulandı.

### TR-3 — Profesyonel e-posta

**Temel metin**

> Konu: Proje Raporunun Teslim Tarihi Hakkında
>
> Sayın Demir,
>
> Umarım iyisinizdir. Proje raporunun teslim süreciyle ilgili olarak sizinle iletişime geçmek istiyorum. Veri tablosundaki iki toplamın kaynak kayıtlarla uyuşmadığını bugün fark ettim. Bu beklenmedik durum, kapsamlı ve hatasız bir çalışma sunabilmem için ek süreye ihtiyaç duymama neden olmaktadır. Bu bağlamda, cuma günü olan teslim tarihinin pazartesi saat 12.00'ye kadar uzatılmasının mümkün olup olmadığını saygılarımla sormak isterim. Anlayışınız ve değerlendirmeniz için şimdiden teşekkür ederim.
>
> Saygılarımla,  
> Deniz

**Revizyon**

> Konu: Rapor için pazartesiye kadar ek süre talebi
>
> Sayın Demir,
>
> Veri tablosundaki iki toplamın kaynak kayıtlarla uyuşmadığını bugün fark ettim. Rakamları doğrulayıp raporu düzeltmek için cuma günkü teslimi pazartesi saat 12.00'ye erteleyebilir miyiz?
>
> Değerlendirmeniz için teşekkür ederim.
>
> Saygılarımla,  
> Deniz

**Değerlendirme**

- **Ne değişti, neden:** İletişim kurduğunu söyleyen giriş, aynı talebi birkaç kez çerçeveleyen isim tamlamaları ve kanıtsız “kapsamlı” iddiası çıkarıldı.
- **Anlam ve ses:** İki uyumsuz toplam, cuma, pazartesi 12.00 ve doğrulama amacı korunuyor. Hitap ve kapanış profesyonel ilişkiyi sürdürüyor.
- **Aşırı gündeliklik / yapay düzensizlik:** Soru biçimi doğrudan ama buyurgan değil. E-posta gereksiz biçimde sohbet diline çekilmedi.
- **Aşırı düzeltme kontrolü:** “Dolgu cümlelerini sil” yaklaşımı teşekkür ve hitabı da silebilirdi. V2, nezaketi türün işlevsel bir parçası sayıyor.

### TR-4 — Gündelik açıklayıcı metin

**Temel metin**

> 20.000 mAh kapasiteli bir powerbankin 5.000 mAh kapasiteli bir telefonu tam olarak dört kez şarj edememesi ilk bakışta oldukça şaşırtıcı bir durumdur. Bunun temel nedeni, enerji dönüşümü sürecinde çeşitli kayıpların meydana gelmesidir. Ayrıca powerbank kapasitesi hücre gerilimi üzerinden ifade edilirken telefon farklı bir gerilimde şarj edilmektedir. Dönüşüm sırasında ve powerbankin kendi devresinde enerji tüketilmektedir. Bu durum, kullanılabilir enerjinin azalmasına yol açmaktadır. Sonuç olarak bu örnek, teknoloji dünyasında görünen değerlerin her zaman gerçek performansı yansıtmadığını gözler önüne sermektedir.

**Revizyon**

> Kâğıt üzerinde 20.000 mAh'lik bir powerbank, 5.000 mAh'lik telefonu dört kez dolduracakmış gibi görünür. Ama iki kapasite aynı çalışma geriliminde ölçülmez. Powerbank gerilimi yükseltirken, telefon da gelen elektriği batarya için dönüştürürken enerji kaybeder; cihazın kendi devresi de bir miktar enerji kullanır. Bu yüzden pratikte dört tam şarjdan daha azı normaldir.

**Değerlendirme**

- **Ne değişti, neden:** Tekrarlanan “bu durum” zinciri ve soyut teknoloji dersi çıkarıldı. Gerilim farkı ile iki dönüşüm kaybı doğrudan açıklandı.
- **Anlam ve ses:** Sayılar ve ana neden korunuyor. Sonuç, günlük kullanıcının sorusuna cevap veriyor.
- **Aşırı gündeliklik / yapay düzensizlik:** “Kâğıt üzerinde” ve “Ama” gündelik açıklamaya uygun; argo ya da yapay kısa cümle eklenmedi.
- **Aşırı düzeltme kontrolü:** Her paragraf başı geçiş sözcüğünü silmek yerine burada “Ama” gerçek bir beklenti–sonuç karşıtlığı kurduğu için tutuldu.

### TR-5 — Haber/rapor metni

**Temel metin**

> Kent Konseyi tarafından hayata geçirilen yenilikçi mahalle bisikleti pilotu, sürdürülebilir ulaşım alanında önemli bir kilometre taşı olmuştur. Üç ay boyunca sekiz istasyonda toplam 1.640 sürüş gerçekleştirilmiştir. Sürüşlerin yüzde 62'si hafta içi 07.00–10.00 ve 17.00–20.00 saatleri arasında yapılmıştır. Ankete katılan 23 kullanıcı, bazı istasyonlarda aydınlatma eksikliği bulunduğunu belirtmiştir. Tüm bu veriler, projenin toplum tarafından büyük bir ilgiyle karşılandığını ve gelecekte kent genelinde yaygınlaştırılması gerektiğini açıkça ortaya koymaktadır.

**Revizyon**

> Kent Konseyi'nin mahalle bisikleti pilotunda, üç ay boyunca sekiz istasyondan 1.640 sürüş yapıldı. Sürüşlerin yüzde 62'si hafta içi 07.00–10.00 ve 17.00–20.00 saatlerinde gerçekleşti. Ankete katılan 23 kullanıcı bazı istasyonlarda aydınlatmanın yetersiz olduğunu bildirdi. Veriler kullanımın işe gidiş ve dönüş saatlerinde yoğunlaştığını gösteriyor; ancak kullanıcı sayısı, anketin yanıt oranı ve istasyonların ayrı ayrı kullanım düzeyleri verilmediği için kent geneline yaygınlaştırma konusunda tek başına yeterli değil.

**Değerlendirme**

- **Ne değişti, neden:** “Yenilikçi,” “kilometre taşı” ve zorunlu yaygınlaştırma sonucu çıkarıldı. Saat dağılımından yapılabilecek dar yorum korundu; eksik paydalar açıklandı.
- **Anlam ve ses:** Süre, istasyon, sürüş, yüzde, saatler ve 23 katılımcı aynen korunuyor. “İşe gidiş ve dönüş” saatlerden yapılan makul bir yorumdur; kesin kullanıcı amacı olarak sunulmamıştır.
- **Aşırı gündeliklik / yapay düzensizlik:** Haber/rapor dili korunuyor. Geçmiş zaman kipleri tutarlı, son cümle veri sınırını açıklayacak kadar uzun.
- **Aşırı düzeltme kontrolü:** Basit fiil tercihi uğruna bütün edilgen yapılar otomatik değiştirilmedi; değişiklikler aktörü bilinen ilk cümlede doğrudanlık, diğerlerinde akış için yapıldı. Raporun sayısal tekrarı “çeşitlilik” adına bozulmadı.

---

## Negative tests: text that should remain substantially unchanged

### EN-N1 — Natural personal prose

**Input**

> I kept the blue mug after my grandfather died—not because it was valuable, but because the handle fit his thumb. It is chipped, too heavy, and terrible at keeping coffee warm. I use it anyway. Not graceful, but mine.

**Output**

> I kept the blue mug after my grandfather died—not because it was valuable, but because the handle fit his thumb. It is chipped, too heavy, and terrible at keeping coffee warm. I use it anyway. Not graceful, but mine.

**Why no edit:** The em dash carries a clean correction, the three properties are concrete rather than ornamental, and the fragment is part of the voice. The paragraph has no unsupported significance claim; it trusts the object to carry the emotion. Rules against dashes, triads, contrast, or fragments would all overcorrect it.

### EN-N2 — Scientific methods prose

**Input**

> Samples were centrifuged at 10,000 × g for 10 minutes at 4 °C. The supernatant was transferred to sterile tubes, and protein concentration was measured by the Bradford assay. Each sample was analyzed in triplicate.

**Output**

> Samples were centrifuged at 10,000 × g for 10 minutes at 4 °C. The supernatant was transferred to sterile tubes, and protein concentration was measured by the Bradford assay. Each sample was analyzed in triplicate.

**Why no edit:** Agentless passive voice is conventional because the procedure, not the operator, is the focus. Repetition provides methodological consistency. Converting every clause to “we” or varying the verbs would change the genre without improving clarity.

### TR-N1 — Doğal gündelik anlatı

**Girdi**

> Otobüsü kaçırınca eve yürüdüm. Yağmur önce çiseledi, sonra birden bastırdı; ben de koşmak yerine ağır ağır devam ettim. Zaten sırılsıklam olmuştum. Köşedeki fırından ekmek kokusu geliyordu, o kadar.

**Çıktı**

> Otobüsü kaçırınca eve yürüdüm. Yağmur önce çiseledi, sonra birden bastırdı; ben de koşmak yerine ağır ağır devam ettim. Zaten sırılsıklam olmuştum. Köşedeki fırından ekmek kokusu geliyordu, o kadar.

**Neden değiştirilmedi:** Özneler bağlamdan açık olduğu için tekrarlanmıyor; noktalı virgül iki bağlı hareketi taşıyor; son ifade anlatıcının ölçülü sesini koruyor. Metne soyut bir “hayat dersi” eklemek de, cümle boylarını yapay biçimde çeşitlendirmek de zarar verirdi.

### TR-N2 — Bilimsel yöntem metni

**Girdi**

> Katılımcılardan yazılı onam alınmıştır. Görüşmeler sessiz bir odada gerçekleştirilmiş, ses kayıtları iki araştırmacı tarafından birbirinden bağımsız olarak kodlanmıştır. Görüş ayrılıkları ortak değerlendirmeyle giderilmiştir.

**Çıktı**

> Katılımcılardan yazılı onam alınmıştır. Görüşmeler sessiz bir odada gerçekleştirilmiş, ses kayıtları iki araştırmacı tarafından birbirinden bağımsız olarak kodlanmıştır. Görüş ayrılıkları ortak değerlendirmeyle giderilmiştir.

**Neden değiştirilmedi:** `-mıştır` ve edilgen yapı yöntem türüne uygun; işlemleri ve sorumluluk düzeyini açıkça bildiriyor. Sırf daha gündelik görünsün diye geniş zamana ya da etkin özneye çevirmek, tür uyumunu ve mevcut sesi bozardı.

---

## Overcorrection log and resulting rule changes

| Tempting mechanical rule | Failure it would cause | v2 safeguard confirmed by tests |
|---|---|---|
| Replace every generic sentence with a concrete one | Invented scenes, motives, outcomes, or evidence | Add specificity only from supplied or verified information; otherwise ask, qualify, retain, or remove. |
| Remove every nominalization and passive | Damaged scientific, legal, and methods prose; misplaced focus | Change only when the form hides a relevant actor, inflates wording, or impairs comprehension. |
| Delete all courtesy or orientation phrases as filler | Abrupt, socially miscalibrated emails | Count politeness and reader orientation as legitimate genre functions. |
| Ban marked words, transitions, triads, contrasts, or em dashes | False positives and loss of useful rhetoric | Evaluate repetition, density, logic, and genre; no single occurrence triggers a change. |
| Maximize sentence-length variation | Choppy explanations and inconsistent procedures | Let idea size, emphasis, and convention determine sentence shape. |
| Replace every `-mektedir/-maktadır` or formal passive in Turkish | Unnaturally casual academic prose and altered aspect/register | Inspect density; preserve legitimate formal morphology. |
| Prefer explicit English-like subjects in Turkish | Pronoun-heavy translationese | Omit recoverable subjects unless contrast, emphasis, or ambiguity requires them. |
| Avoid repeating the same term | Weakened source scope and terminological precision | Preserve controlled repetition in reports, methods, law, and technical prose. |

## Suite-level findings

- All ten positive cases improved in specificity, source discipline, or economy without losing supplied facts.
- The two scientific cases and two methods negative tests show that v2 must not equate natural prose with active voice, short words, or informality.
- The application cases confirm that concrete reflection works only when the source text contains concrete material; the skill needs an explicit no-invention branch.
- The email cases show that “necessity” includes social function, not just new information.
- The report cases confirm that repeated terms and longer qualifying sentences may be necessary to represent denominators and uncertainty accurately.
- The negative tests are a required stop condition: an editor that changes them substantially fails even if the new version is grammatical.

## Limits and next test round

This suite was authored and evaluated within the same design process. It tests rule coherence, not reader preference at scale. A v3 evaluation should add:

- blinded ratings from several native or highly proficient English and Turkish editors;
- user-authored passages with explicit voice samples and permission to compare edit distance;
- legal clauses, grant prose, recommendation letters, product copy, documentation, and literary dialogue;
- longer texts where paragraph ordering and repeated endings become visible;
- controlled pairs that vary only one feature, such as Turkish explicit-subject density or English participial-clause density;
- measures for factual preservation, edit distance, genre fit, and inter-rater agreement rather than detector scores.
