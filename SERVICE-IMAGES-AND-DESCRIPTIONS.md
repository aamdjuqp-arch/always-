# 🖼️ Service Images and Payment Link Descriptions

## Overview
Each shipping service has unique social sharing images and payment link descriptions to provide brand-specific identity when links are shared on social media platforms.

---

## 📦 Supported Shipping Services

### 1. أرامكس (Aramex)
- **Image:** `/og-aramex.jpg` (81KB)
- **Title:** أرامكس - Aramex | صفحة دفع آمنة
- **Description:** أرامكس - شركة أرامكس الرائدة في خدمات الشحن السريع والحلول اللوجستية في المنطقة - صفحة دفع آمنة ومحمية
- **Payment Link:** `/pay/aramex.html?service=aramex&payId={uuid}`
- **About:** Leading express delivery and logistics solutions company in the Middle East region

---

### 2. فيديكس (FedEx)
- **Image:** `/og-fedex.jpg` (52KB)
- **Title:** فيديكس - FedEx | صفحة دفع آمنة
- **Description:** فيديكس - خدمات شحن دولية موثوقة مع تتبع فوري للشحنات - صفحة دفع آمنة ومحمية
- **Payment Link:** `/pay/fedex.html?service=fedex&payId={uuid}`
- **About:** International express shipping services with real-time package tracking

---

### 3. DHL
- **Image:** `/og-dhl.jpg` (50KB)
- **Title:** DHL | صفحة دفع آمنة
- **Description:** DHL - شركة DHL الرائدة عالمياً في خدمات الشحن السريع واللوجستية - صفحة دفع آمنة ومحمية
- **Payment Link:** `/pay/dhl.html?service=dhl&payId={uuid}`
- **About:** World's leading express and logistics company

---

### 4. UPS
- **Image:** `/og-ups.jpg` (29KB)
- **Title:** UPS | صفحة دفع آمنة
- **Description:** UPS - شركة United Parcel Service الأمريكية الرائدة في خدمات الشحن والتوصيل - صفحة دفع آمنة ومحمية
- **Payment Link:** `/pay/ups.html?service=ups&payId={uuid}`
- **About:** American multinational package delivery and supply chain management company

---

### 5. سمسا (SMSA)
- **Image:** `/og-smsa.jpg` (58KB)
- **Title:** SMSA | صفحة دفع آمنة
- **Description:** SMSA - شركة سمسا للسحن والتوصيل - صفحة دفع آمنة ومحمية
- **Payment Link:** `/pay/smsa.html?service=smsa&payId={uuid}`
- **About:** Saudi shipping and delivery company

---

### 6. زاجل (Zajil)
- **Image:** `/og-zajil.jpg` (47KB)
- **Title:** زاجل - Zajil | صفحة دفع آمنة
- **Description:** زاجل - شركة زاجل لخدمات الشحن والتوصيل في المملكة العربية السعودية - صفحة دفع آمنة ومحمية
- **Payment Link:** `/pay/zajil.html?service=zajil&payId={uuid}`
- **About:** Saudi-based shipping and delivery services company

---

### 7. نايل (Naqel)
- **Image:** `/og-naqel.jpg` (46KB)
- **Title:** نايل - Naqel | صفحة دفع آمنة
- **Description:** نايل - شركة نايل اكسبرس لخدمات الشحن والتوصيل - صفحة دفع آمنة ومحمية
- **Payment Link:** `/pay/naqel.html?service=naqel&payId={uuid}`
- **About:** Naqel Express shipping and delivery services

---

### 8. الإمارات (Emirates Post)
- **Image:** `/og-empost.jpg` (77KB)
- **Title:** البريد الإماراتي - Emirates Post | صفحة دفع آمنة
- **Description:** البريد الإماراتي - المشغل الوطني للبريد في دولة الإمارات العربية المتحدة - صفحة دفع آمنة ومحمية
- **Payment Link:** `/pay/empost.html?service=empost&payId={uuid}`
- **About:** National postal operator of the United Arab Emirates

---

## 🔗 Payment Link Structure

### URL Format
```
https://your-domain.netlify.app/pay/{service}.html?service={service}&payId={uuid}
```

### Example Links
```
# Aramex Payment Link
https://your-domain.netlify.app/pay/aramex.html?service=aramex&payId=4d6ed486-b214-41e8-a550-6b3b20ffe36e

# FedEx Payment Link
https://your-domain.netlify.app/pay/fedex.html?service=fedex&payId=4d6ed486-b214-41e8-a550-6b3b20ffe36e

# Emirates Post Payment Link
https://your-domain.netlify.app/pay/empost.html?service=empost&payId=4d6ed486-b214-41e8-a550-6b3b20ffe36e
```

---

## 🖼️ Social Sharing Images

### Image Specifications
- **Format:** JPG
- **Location:** `/public/og-*.jpg`
- **Used for:** Social media preview (Facebook, Twitter, LinkedIn, WhatsApp)

### Image List
1. ✅ `/og-aramex.jpg` - Aramex logo/branding
2. ✅ `/og-fedex.jpg` - FedEx logo/branding
3. ✅ `/og-dhl.jpg` - DHL logo/branding
4. ✅ `/og-ups.jpg` - UPS logo/branding
5. ✅ `/og-smsa.jpg` - SMSA logo/branding
6. ✅ `/og-zajil.jpg` - Zajil logo/branding
7. ✅ `/og-naqel.jpg` - Naqel logo/branding
8. ✅ `/og-empost.jpg` - Emirates Post logo/branding

### Additional Post Office Images
- `/og-saudipost.jpg` - Saudi Post
- `/og-kwpost.jpg` - Kuwait Post
- `/og-omanpost.jpg` - Oman Post
- `/og-bahpost.jpg` - Bahrain Post
- `/og-qpost.jpg` - Qatar Post

---

## 📱 Social Media Behavior

### When Links Are Shared:
1. **Facebook** - Shows service-specific title, description, and image
2. **Twitter** - Shows service-specific card with image
3. **LinkedIn** - Shows service-specific preview
4. **WhatsApp** - Shows service-specific image and description
5. **Telegram** - Shows service-specific preview

### User Flow:
1. User shares payment link
2. Social media crawler fetches the static HTML file
3. Displays service-specific preview (title, description, image)
4. Recipient clicks the link
5. JavaScript redirects to React app with correct service context
6. Payment process continues with service-specific branding

---

## 🎨 Meta Tags Implementation

### Each Service HTML File Contains:
```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>{SERVICE_NAME} | صفحة دفع آمنة</title>
    <meta name="description" content="{SERVICE_DESCRIPTION_ARABIC}" />
    
    <!-- Open Graph / Facebook -->
    <meta property="og:title" content="{SERVICE_NAME} | صفحة دفع آمنة" />
    <meta property="og:description" content="{SERVICE_DESCRIPTION_ARABIC}" />
    <meta property="og:image" content="/og-{SERVICE}.jpg" />
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:image" content="/og-{SERVICE}.jpg" />
</head>
<body>
    <!-- Service-specific content -->
    <script>
        // Redirect to React app with service and payId
    </script>
</body>
</html>
```

---

## ✅ Benefits

1. **Brand Recognition** - Each service shows its own brand identity
2. **Trust** - Users recognize the shipping company immediately
3. **Professional Appearance** - Service-specific descriptions add credibility
4. **Social Media Optimization** - Better engagement when links are shared
5. **Cross-Platform** - Works on all major social media platforms
6. **User Experience** - Clear service context before visiting the link

---

## 🚀 Deployment

All service images and descriptions are:
- ✅ Included in the repository
- ✅ Built into the `/dist/` directory
- ✅ Pushed to GitHub
- ✅ Ready for deployment

No additional configuration needed!

---

**Repository:** https://github.com/aamdjuqp-arch/always-.git
