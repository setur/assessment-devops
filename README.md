# DevOps Assessment

## Merhaba

Bu değerlendirme işe başvuru sürecindeki adaylar için hazırlanmış olup, katılacak kimselerin yaklaşım ve yetkinliklerini değerlendirmede bizlere yardımcı olmak için tasarlanmıştır.

Değerlendirme dahilinde; belirtilen süre içerisinde aşağıda kapsamı ve detayları belirlenmiş projeyi tamamlamanızı beklemekteyiz. Dikkat edebileceğiniz bir diğer husus ise, bizlerin doğru bir değerlendirme yapmamıza yardımcı olacak şekilde iletebileceğiniz en iyi çalışmayı bizlere teslim ediyor olmanız.


### Senaryo

Mevcut bir kubernetes cluster kurulumu üzerine belirlenen araç ve servislerin kurulumu yapılacaktır. Bu kurulumun diğer clusterlara, ortamlara tekrar kurulabilmesini sağlamak için Infrastructure as Code yaklaşımı ile kurulum tamamiyle scriptler ve/veya araçlar aracılığıyla sağlanmalıdır. Çalışmanın çıktısı da kod olarak iletilmelidir.

İletilecek microservice'ler en az iki adet olmak üzere REST endpoint'leri bulunan, healthcheck yapabilen ve birbirlerini çağıracak containerlar olmalıdırlar.

Ayrıca bu microservicelerin aşağıdaki kriterleri karşılamaları gerekmektedir:
- Kendi aralarındaki trafiğin Jaeger, Kiali v.b. araçlarla izlenilebilir olması,
- Metriclerinin prometheus benzeri bir metrics server'a aktarılması,
- Ingress olarak konumlanacak bir API Gateway ile HTTP trafiği alabilmesi,
- Readiness ve Health checklerinin periyodik yapılabilmesi,
- Belirleyeceğiniz metriklere göre ölçeklenebilmesi,
- Environment variable'ları kullanabilmesi,
- Docker image'lar için bir container registry'den çağrılıyor olması,


### Teknik Beklentiler

- Kullanılacak Teknolojiler:
  - Docker
  - Kubernetes
  - Git
  - Istio, Consul v.b.

- Kısıtlamalar ve Gereksinimler:
  - Projenin sık commitlerle Git üzerinde geliştirilmesi
  - Git üzerinde master, development branchleri ve sürüm taglemelerinin kullanımı
  - Projenin nasıl çalıştırılacağına dair README.md dokümantasyonu


## Sorularınız

Değerlendirmelerle ilgili sorularınızı [github@setur.com.tr](mailto:github@setur.com.tr) adresine iletebilirsiniz.


### Lisans

[Apache 2.0](LICENSE) ile lisanslanmıştır.
