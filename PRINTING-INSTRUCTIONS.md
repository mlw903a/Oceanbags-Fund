# 5x9 Flyer Printing Instructions

## Files Created
- `5x9-flyer-front.html` - Front side design
- `5x9-flyer-back.html` - Back side design

## Print Specifications

### Dimensions
- **Finished Size:** 5" × 9"
- **With Bleed:** 5.25" × 9.25" (0.125" bleed on all sides)
- **Safe Area:** Keep all critical text/images 0.125" from trim edge

### Print Settings
- **Resolution:** 300 DPI minimum
- **Color Mode:** CMYK (for professional printing)
- **Paper Stock:** Recommend 100lb cover stock (glossy or matte)
- **Finish:** Consider UV coating or matte laminate for durability

## How to Prepare for Printing

### Option 1: Convert HTML to PDF (Recommended)
1. Open each HTML file in Google Chrome or Firefox
2. Print to PDF with these settings:
   - Paper size: Custom (5.25" × 9.25")
   - Margins: None
   - Scale: 100%
   - Background graphics: ON
   - Headers/footers: OFF

### Option 2: Professional Printer
Send both HTML files to your printer along with these specs:
- Two-sided printing (front and back)
- Finish size: 5" × 9"
- Include 0.125" bleed
- Cut marks requested

## QR Code Setup

### Generate QR Code for PayPal Link
**PayPal URL:** `https://www.paypal.com/ncp/payment/CLFFCAHE2G288`

**Option A - Online Generator:**
1. Visit: https://www.qr-code-generator.com/
2. Enter the PayPal URL above
3. Download as PNG (minimum 300×300 pixels)
4. Save as `paypal-qr-code.png`

**Option B - Use Python (if available):**
```bash
pip install qrcode[pil]
python3 -c "
import qrcode
qr = qrcode.QRCode(version=1, error_correction=qrcode.constants.ERROR_CORRECT_H, box_size=10, border=4)
qr.add_data('https://www.paypal.com/ncp/payment/CLFFCAHE2G288')
qr.make(fit=True)
img = qr.make_image(fill_color='black', back_color='white')
img.save('paypal-qr-code.png')
"
```

### Insert QR Code into Back Design
1. Generate the QR code using one of the methods above
2. Open `5x9-flyer-back.html` in a text editor
3. Find the QR code placeholder section (around line 240)
4. Replace the SVG placeholder with: `<img src="paypal-qr-code.png" alt="Donate via PayPal" />`

## Spacing & Layout Notes

### Front Side
- **Hero section** (top): 0.6" padding ensures headline is prominent
- **Content area**: 0.4" padding for readability
- **Stats box**: Left border accent draws eye to key facts
- **Footer**: Full-width for strong brand presence

### Back Side
- **Donation tiers**: Equal width boxes make amounts scannable
- **QR code**: 1.5" × 1.5" — large enough to scan easily
- **Action section**: Highlighted background encourages engagement

## Pre-Print Checklist

- [ ] Generate QR code and test scan with phone camera
- [ ] Insert QR code image into back design
- [ ] Convert both HTML files to PDF
- [ ] Check PDFs at 100% zoom for text clarity
- [ ] Verify colors look correct (blues, golds, grays)
- [ ] Confirm bleed extends to 5.25" × 9.25"
- [ ] Print one test copy before full run
- [ ] Check alignment front-to-back when folded

## Recommended Print Vendors

### Local/Austin Area
- FedEx Office (quick turnaround)
- AlphaGraphics Austin
- Minuteman Press

### Online
- **PrintPlace.com** - Great for bulk quantities
- **GotPrint.com** - Fast turnaround
- **Vistaprint** - Good for smaller runs

### Order Specifications to Provide
```
Product: Flyers/Postcards
Size: 5" × 9" (custom)
Quantity: [your amount]
Paper: 100lb Cover Gloss or Matte
Sides: Two-sided full color
Coating: UV Gloss (optional)
Turnaround: Standard or Rush
```

## Budget Estimates

### Print Costs (approximate)
- 250 copies: $80-120
- 500 copies: $120-180
- 1000 copies: $180-250

*Prices vary by vendor, paper stock, and turnaround time*

## Design Customization

If you need to modify the designs:
1. HTML files can be edited in any text editor
2. Colors are defined in the `<style>` section
3. Text content is in the `<body>` section
4. Current color scheme:
   - Navy: `#1e3a5f`
   - Blue: `#2d5a8c`
   - Gold/Yellow: `#ffd700`
   - Dark gray: `#2c3e50`

## Questions?

Contact your designer or refer to the campaign strategy document for messaging guidance.

---
**Created:** November 2025
**Campaign:** Oceanbags Foundation - 500 Backpacks for Kids on the Move
