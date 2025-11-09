# 📊 Service Summary Table - Images and Descriptions

## Quick Reference for All Shipping Services

| # | Service (Arabic) | Service (English) | Image File | Image Size | Payment Link |
|---|------------------|-------------------|------------|------------|--------------|
| 1 | أرامكس | Aramex | og-aramex.jpg | 81KB | /pay/aramex.html |
| 2 | فيديكس | FedEx | og-fedex.jpg | 52KB | /pay/fedex.html |
| 3 | دي إتش إل | DHL | og-dhl.jpg | 50KB | /pay/dhl.html |
| 4 | يو بي إس | UPS | og-ups.jpg | 29KB | /pay/ups.html |
| 5 | سمسا | SMSA | og-smsa.jpg | 58KB | /pay/smsa.html |
| 6 | زاجل | Zajil | og-zajil.jpg | 47KB | /pay/zajil.html |
| 7 | نايل | Naqel | og-naqel.jpg | 46KB | /pay/naqel.html |
| 8 | الإمارات | Emirates Post | og-empost.jpg | 77KB | /pay/empost.html |

---

## 📋 Service Descriptions (Arabic)

### 1. أرامكس (Aramex)
**الوصف:** شركة أرامكس الرائدة في خدمات الشحن السريع والحلول اللوجستية في المنطقة

### 2. فيديكس (FedEx)
**الوصف:** فيديكس - خدمات شحن دولية موثوقة مع تتبع فوري للشحنات

### 3. دي إتش إل (DHL)
**الوصف:** شركة DHL الرائدة عالمياً في خدمات الشحن السريع واللوجستية

### 4. يو بي إس (UPS)
**الوصف:** شركة United Parcel Service الأمريكية الرائدة في خدمات الشحن والتوصيل

### 5. سمسا (SMSA)
**الوصف:** شركة سمسا للسحن والتوصيل

### 6. زاجل (Zajil)
**الوصف:** شركة زاجل لخدمات الشحن والتوصيل في المملكة العربية السعودية

### 7. نايل (Naqel)
**الوصف:** شركة نايل اكسبرس لخدمات الشحن والتوصيل

### 8. الإمارات (Emirates Post)
**الوصف:** المشغل الوطني للبريد في دولة الإمارات العربية المتحدة

---

## 🔗 Payment Link URL Format

### Template:
```
https://your-domain.netlify.app/pay/{service}.html?service={service}&payId={unique-id}
```

### Example:
```
https://your-domain.netlify.app/pay/empost.html?service=empost&payId=4d6ed486-b214-41e8-a550-6b3b20ffe36e
```

---

## 🖼️ Image Locations

All images are stored in:
```
/public/og-{service}.jpg
```

Example:
- `/public/og-aramex.jpg`
- `/public/og-fedex.jpg`
- `/public/og-dhl.jpg`
- etc.

---

## 📱 Social Media Preview

Each service displays uniquely when payment links are shared:

### Facebook Preview Shows:
- **Title:** {Service Name} | صفحة دفع آمنة
- **Description:** Service-specific Arabic description
- **Image:** Service-specific og-{service}.jpg

### Twitter Preview Shows:
- **Card Type:** summary_large_image
- **Title:** {Service Name} | صفحة دفع آمنة
- **Description:** Service-specific Arabic description
- **Image:** Service-specific og-{service}.jpg

---

## ✅ Implementation Status

- ✅ All 8 services have unique images
- ✅ All services have Arabic descriptions
- ✅ All meta tags are configured
- ✅ Payment link structure is in place
- ✅ Images are optimized and ready
- ✅ Repository contains all files

**Total Services:** 8
**Total Images:** 13 (8 shipping + 5 postal)
**Total Files:** 208+
**Repository:** https://github.com/aamdjuqp-arch/always-.git
