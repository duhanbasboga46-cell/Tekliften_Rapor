import pandas as pd
import matplotlib.pyplot as plt

# Veriler örnek olarak dosyalardan çıkarıldı
data = [
    {
        "Musteri": "Ornek Musteri",
        "Tarih": "2026-05-12",
        "Adet": 5,
        "BirimFiyat": 906.16,
        "ToplamTutar": 4650.78
    },
    {
        "Musteri": "Ornek Musteri 2",
        "Tarih": "2026-06-12",
        "Adet": 4,
        "BirimFiyat": 1383.21,
        "ToplamTutar": 5652.82
    }
]

df = pd.DataFrame(data)

print("\n=== GENEL ÖZET ===")
print(f"Toplam Müşteri Sayısı: {len(df)}")
print(f"Toplam Satış: €{df['ToplamTutar'].sum():,.2f}")
print(f"Toplam Adet: {df['Adet'].sum()}")
print(f"Ortalama Sipariş Tutarı: €{df['ToplamTutar'].mean():,.2f}")

# Grafik 1
plt.figure(figsize=(8,5))
plt.bar(df["Musteri"], df["ToplamTutar"])
plt.title("Müşteri Bazlı Toplam Teklif Tutarı")
plt.ylabel("Euro")
plt.tight_layout()
plt.savefig("musteri_satislari.png")
plt.close()

# Grafik 2
plt.figure(figsize=(8,5))
plt.bar(df["Musteri"], df["Adet"])
plt.title("Müşteri Bazlı Adet Analizi")
plt.ylabel("Adet")
plt.tight_layout()
plt.savefig("adet_analizi.png")
plt.close()

# Grafik 3
plt.figure(figsize=(8,5))
plt.bar(df["Musteri"], df["BirimFiyat"])
plt.title("Müşteri Bazlı Birim Fiyat Karşılaştırması")
plt.ylabel("Euro")
plt.tight_layout()
plt.savefig("birim_fiyat.png")
plt.close()

print("\nGrafikler oluşturuldu:")
print("- musteri_satislari.png")
print("- adet_analizi.png")
print("- birim_fiyat.png")

plt.savefig("Grafikler/toplam_satis.png")
plt.savefig("Grafikler/adet_analizi.png")
