# Hafta 2 Özeti: Çok kübitli sistemler ve dolanıklık

## Tensör çarpımı ve ayrılabilirlik
İki kübitli durum `a|00> + b|01> + c|10> + d|11>` olarak yazılır. Durum iki ayrı kübitin çarpımı ise ayrılabilirdir ve bu ancak `ad = bc` olduğunda mümkündür. Dolanıklık ölçüsü olarak `C = 2|ad - bc|` kullanıyoruz: C = 0 ayrılabilir, C = 1 maksimum dolanık demek.

## Bell durumları
Dört durum: `Φ± = (|00> ± |11>)/√2` ve `Ψ± = (|01> ± |10>)/√2`. Üretmek için H ve CNOT kullanılır. Ayırt etmek için CNOT, ardından ilk kübite H uygulanıp iki kübit ölçülür: Φ+ → 00, Φ− → 10, Ψ+ → 01, Ψ− → 11.

## CHSH
Klasik stratejiyle kazanma olasılığı en çok 3/4. Kuantum stratejiyle `cos²(π/8) ≈ 0.854` elde edilir. Qiskit'te ölçüm tabanını açıyla değiştirmek için `RY(-2·açı)` kullandık ve dört girdi çiftinde de 0.8536 gördük.

## Teleportasyon
Gerekenler: Alice ile Bob arasında paylaşılan bir Bell çifti ve Alice'ten Bob'a 2 klasik bit. Alice'in Bell ölçümünün dört sonucu eşit olasılıklıdır (1/4). Bob'un düzeltmesi: önce X, sonra Z. Z olmadan fidelity `½(1 + cos²θ)` olur (θ = 1.1 için 0.6029). Işıktan hızlı iletişim yok: Bob klasik bitler gelmeden yalnızca rastgele görünen bir durum görür. Alice'in orijinal kübiti ölçümle yok olur, yani klonlama olmaz.

## Süperyoğun kodlama
Teleportasyonun tersi: paylaşılan Bell çifti ile 1 kübit göndererek 2 klasik bit aktarılır. Alice bitlere göre I, X, Z veya ZX uygular. Bob Bell ölçümüyle iki biti okur. Qiskit'te dört girişin hepsi olasılık 1.0 ile doğru çıktı.

## Takıldığım yer
(buraya kendi cümlelerinle yaz)