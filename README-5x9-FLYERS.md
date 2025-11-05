# 5×9 Flyer Files - Quick Reference

## What You Have

### Design Files
1. **5x9-flyer-front.html** → Front side of flyer
2. **5x9-flyer-back.html** → Back side of flyer

### Supporting Files
- **PRINTING-INSTRUCTIONS.md** → Complete printing guide
- **paypal-qr-code.png** → QR code for donations (you need to generate this)

## Quick Start - Get to Print in 5 Steps

### Step 1: Generate QR Code
Visit: **https://www.qr-code-generator.com/**
- Enter URL: `https://www.paypal.com/ncp/payment/CLFFCAHE2G288`
- Download as PNG
- Save as `paypal-qr-code.png` in this folder

### Step 2: Add QR Code to Back Design
- Open `5x9-flyer-back.html` in text editor
- Find line ~240 (QR code placeholder)
- Replace the `<svg>` block with: `<img src="paypal-qr-code.png" alt="PayPal Donation" style="width:100%;height:100%;" />`

### Step 3: Convert to PDF
- Open `5x9-flyer-front.html` in Chrome/Firefox
- File → Print → Save as PDF
- Settings: Custom size 5.25" × 9.25", No margins, Background graphics ON
- Repeat for `5x9-flyer-back.html`

### Step 4: Review PDFs
- Check text is clear at 100% zoom
- Verify QR code scans with your phone
- Ensure colors look vibrant (especially blues and gold)

### Step 5: Send to Printer
- Upload both PDFs
- Specify: 5" × 9" finished size, double-sided, 100lb cover stock
- Request sample proof before full run

## Design Elements

### Front Side
- **Tagline:** "Strong enough for the road no child should have to take."
- **Goal:** 500 backpacks for children displaced by war
- **Key Stats:** $25 per backpack, Partners.ngo partnership, Ocean Bound Plastics

### Back Side
- **Donation Tiers:** $25 (one), $100 (four), $250 (ten backpacks)
- **QR Code:** Direct PayPal donation
- **Features:** Why durable matters, eco-credentials, partner info

## Color Scheme
- **Navy Blue:** #1e3a5f (primary)
- **Bright Blue:** #2d5a8c (accents)
- **Gold:** #ffd700 (highlights)
- **White:** Background

## File Sizes (After PDF Conversion)
- Front: ~200-400 KB
- Back: ~200-400 KB (without QR code image)

## Recommended Print Quantity
- **Book fair booth:** 100-250 copies minimum
- **Distribution campaign:** 500-1000 copies
- **Test run:** Order 25-50 first to verify quality

## Need Help?
- **Spacing issues?** Open HTML in browser, use browser dev tools to adjust padding values
- **Color looks off?** Most professional printers offer color matching services
- **Different size needed?** Edit the `width` and `height` values in HTML `<style>` section

---

**Next Steps:** See `PRINTING-INSTRUCTIONS.md` for detailed specifications and vendor recommendations.
