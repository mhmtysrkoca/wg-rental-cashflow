# wg-rental-cashflow
Almanya WG kira+konut yatırımı nakit akışı: oda kira/doluluk, tüm giderler, kredi, AfA, vergi etkisi. DSCR, cap rate, cash-on-cash ve CSV.
## Kısaltmalar / Terimler Sözlüğü

- **WG (Wohngemeinschaft):** Paylaşımlı ev/oda kiralama modeli. Birden fazla kiracı, oda bazında kira öder.
- **AfA (Absetzung für Abnutzung):** Amortisman/yıpranma payı (Almanya). **Sadece bina payı** üzerinden yıllık % ile gider yazılır.  
  *AfA tabanı* = Satın alma bedeli × (1 − arsa payı %)
- **NOI (Net Operating Income):** Net işletme geliri (faiz/borç hariç).  
  `NOI (yıllık) = (Etkin kira (ay) − Aylık işletme giderleri) × 12`
- **OPEX (Operating Expenses):** İşletme giderleri. Bu uygulamada: Aidat/Hausgeld, sigorta, emlak vergisi (yıllık/12), yönetim %, bakım %, CapEx rezervi, utilities, diğer.
- **CapEx (Capital Expenditures):** Büyük onarım/yenileme gibi sermaye harcamaları. Bu uygulamada **“CapEx rezervi”** aylık ayrılan tutar.
- **ADS (Annual Debt Service):** Yıllık borç servisi (kredi taksitleri + varsa aylık ekstra anapara).  
  `ADS = (Aylık taksit + aylık ekstra) × 12`
- **Cap Rate (Capitalization Rate):** Yatırımın fiyatına göre net getiri oranı.  
  `Cap rate = NOI / Satın alma bedeli`
- **DSCR (Debt Service Coverage Ratio):** Borç karşılama oranı — borç servisini karşılama gücü.  
  `DSCR = NOI / ADS`  (Genelde **>1** güvenlidir)
- **Cash-on-Cash (CoC) Return:** Nakit koyulan paraya göre yıllık nakit getiri oranı.  
  `CoC = Vergi sonrası yıllık nakit akışı / (Peşinat + Alım masrafları + Tadilat)`
- **Etkin Kira (Effective Rent):** Doluluk/boş kalma etkisi dahil kira.  
  `Etkin kira (ay) = (Oda kiraları × oda bazında doluluk) × (1 − global boş kalma %) + diğer gelir`
- **Grunderwerbsteuer (Taşınmaz edinim vergisi):** Satın alma sırasında ödenen vergi (eyalete göre değişir).  
- **Hausgeld / HOA (Aidat):** Kat mülkiyetli dairelerde ortak giderler + yedek akçe kalemlerini içeren aylık ödeme.
- **AfA oranı (%):** Binanın yıllık amortisman yüzdesi (ör. %2).

## Formül Özeti

- **Aylık taksit (PMT):**  
  `M = P * r * (1+r)^n / ((1+r)^n − 1)`  
  (P: kredi tutarı, r: aylık faiz, n: toplam ay; r=0 ise `M = P/n`)
- **NOI (yıllık):**  
  `NOI = (Etkin kira (ay) − OPEX (ay)) × 12`
- **ADS (yıllık):**  
  `ADS = (Aylık taksit + aylık ekstra anapara) × 12`
- **Vergilendirilebilir gelir (yaklaşık):**  
  `NOI − İlk yıl faiz − AfA`
- **Gelir vergisi (yaklaşık):**  
  `Vergilendirilebilir gelir × marjinal vergi oranı`  
  (Negatifse ve *zarar diğer geliri azaltır* seçeneği açıksa, bu tutar **vergi avantajı** olarak nakde eklenir.)
- **Vergi öncesi nakit akışı:**  
  `NOI − ADS`
- **Vergi sonrası nakit akışı:**  
  `Vergi öncesi nakit akışı − Gelir vergisi`
- **Cap rate:** `NOI / Satın alma bedeli`
- **DSCR:** `NOI / ADS`
- **Cash-on-Cash:** `Vergi sonrası yıllık nakit akışı / (Peşinat + Alım masrafları + Tadilat)`

> **Notlar:**  
> • AfA yalnızca **bina payına** uygulanır; `AfA tabanı = Fiyat × (1 − arsa payı %)`  
> • Yönetim % ve Bakım % bu uygulamada **etkin kiraya** göre hesaplanır.  
> • Bu araç eğitim amaçlıdır; vergi kuralları kişisel duruma göre değişebilir.
