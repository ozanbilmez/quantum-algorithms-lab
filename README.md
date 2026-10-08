# quantum-algorithms-lab

Kuantum hesaplamanın temellerini Qiskit ile deneyerek öğrendiğim notebook koleksiyonu. Her hafta bir klasör.

## İçindekiler

| Hafta | Konu | İçerik |
| --- | --- | --- |
| 1 | Lineer cebir ve tek kübit | Bloch küresi ve faz, operatör formalizmi, hafta özeti |
| 2 | Çok kübitli sistemler ve dolanıklık | Ayrılabilirlik, CHSH oyunu, süperyoğun kodlama ve teleportasyon, hafta özeti |

## Çalıştırma

```
uv venv
uv pip install qiskit qiskit-aer matplotlib numpy pylatexenc ipykernel
```

Sonra VS Code'da notebook'u aç ve kernel olarak `.venv`'i seç (Python 3.10+).

## Notlar

- CHSH: klasik strateji en çok 3/4 kazanır, kuantum strateji `cos²(π/8) ≈ 0.854`. Ölçüm tabanı `RY(-2·açı)` ile ayarlandı.
- Teleportasyon: Bell çifti ve 2 klasik bit ile bilinmeyen durum aktarılır. Z düzeltmesi çıkarılınca fidelity `½(1 + cos²θ)` değerine düşer (θ = 1.1 için ≈ 0.603).