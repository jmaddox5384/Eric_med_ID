# Medical ID - Eric Blanchard

A secure, mobile-friendly medical ID page that displays critical health information when scanned via QR code. Designed for emergency situations where first responders or medical professionals need quick access to patient information.

## Features

- 🔐 **PIN Protection** - 4-digit PIN required to view sensitive medical info
- 📱 **Mobile Optimized** - Clean, responsive design for any device
- 📞 **One-Tap Contact** - Call or text emergency contacts instantly
- 🚨 **Emergency Bypass** - Direct call button available without PIN
- 📋 **QR Code** - Auto-generated for wallet cards or medical bracelets

## Quick Setup (GitHub Pages)

1. Fork or clone this repository
2. Go to **Settings** → **Pages**
3. Under "Source", select **Deploy from a branch**
4. Choose `main` branch and `/ (root)` folder
5. Click **Save**

Your page will be live at: `https://YOUR-USERNAME.github.io/REPO-NAME/`

## Customization

Open `index.html` and search for `UPDATE:` comments to find all the places you need to customize:

### Security
```javascript
// Line ~580 - Change the PIN
const CORRECT_PIN = "1234";  // Change to your secure PIN
```

### Patient Information
- **Name**: Search for "ERIC BLANCHARD" (appears twice - PIN screen and header)
- **DOB & Blood Type**: In the emergency header section
- **Allergies**: Add/remove `<span class="tag">` elements
- **Medical Conditions**: Add/remove `<span class="tag condition">` elements
- **Medications**: Add/remove medication rows in the info-list
- **Notes**: Update the important notes paragraph

### Contact Information
- **Primary Contact**: Update phone numbers in `tel:` and `sms:` links
- **Emergency Contacts**: Update names, relationships, and phone numbers
- **Healthcare Providers**: Update doctor names, pharmacy, insurance info

### Phone Number Format
Use international format: `+15551234567` (no dashes or spaces)

## Files

```
medical-id/
├── index.html    # Main page (everything in one file)
└── README.md     # This file
```

## Security Considerations

⚠️ **Important**: This page is publicly accessible. The PIN provides basic deterrence but is not true security. Anyone with technical knowledge could bypass it.

**Recommendations:**
- Use an obscure/random repository name
- Don't share the URL publicly
- Consider the PIN as a privacy measure, not security
- Keep sensitive info (like full SSN or account numbers) off the page

## Printing QR Code

1. Open the page and enter the PIN
2. Scroll to the QR code section
3. Screenshot or print the page
4. Cut out QR code for wallet card or medical bracelet

## License

MIT - Feel free to use and modify for personal use.

---

*Last Updated: February 2026*
