# 🚀 AFAIK Knowledge Hub - SharePoint Dashboard

**A modern, modular, SharePoint-compatible HTML dashboard built with Vanilla JavaScript**

---

## 📁 File Structure

```
SharePoint-Dashboard/
├── index.html          - Main HTML file with scoped CSS
├── data.js             - All application data (projects, organization, resources)
├── icons.js            - Inline SVG icons (no external dependencies)
├── components.js       - Page rendering functions
└── app.js              - Routing logic and state management
```

---

## ✨ Features

✅ **SharePoint-Safe Architecture**
- No React, Webpack, or build tools required
- All CSS scoped to `#filinvest-dashboard-v2` (no conflicts)
- Inline SVG icons (no external CDN dependencies)
- Vanilla JavaScript (ES6+)

✅ **Complete Page Views**
- **Homepage** - Hero section with company branding
- **Dashboard** - Progress tracking and missions
- **Projects** - 10 projects with filtering and detail views
- **Organization** - Team hierarchy chart (8 members)
- **Resources** - Accordion-style permits and forms guide
- **Links** - Quick links to 6 internal systems
- **Map Explorer** - Embedded virtual tour iframe

✅ **Glassmorphism Design**
- Modern blur effects and gradients
- Filinvest corporate colors (#003d71, #0052a3)
- Fully responsive (desktop, tablet, mobile)

✅ **Interactive Features**
- Client-side routing (no page refresh)
- Search functionality
- Floating chatbot
- Mission completion tracking
- Project filtering by category

---

## 🔧 How to Deploy to SharePoint

### Option 1: Upload to Document Library (Recommended)

1. **Create a folder** in your SharePoint site:
   - Navigate to: `Site Contents > Documents > New Folder`
   - Name it: `AFAIK-Dashboard`

2. **Upload all 5 files** to this folder:
   ```
   index.html
   data.js
   icons.js
   components.js
   app.js
   ```

3. **Get the direct link**:
   - Right-click `index.html` > Copy Link
   - Example: `https://yoursite.sharepoint.com/sites/YourSite/Documents/AFAIK-Dashboard/index.html`

4. **Embed in a page** (Optional):
   - Edit a SharePoint page
   - Add a "File Viewer" web part or "Embed" web part
   - Paste the link to `index.html`

---

### Option 2: Embed via Script Editor Web Part

1. **Upload the files** to a Document Library

2. **Get the URLs** for each file:
   ```
   /sites/YourSite/Documents/AFAIK-Dashboard/data.js
   /sites/YourSite/Documents/AFAIK-Dashboard/icons.js
   /sites/YourSite/Documents/AFAIK-Dashboard/components.js
   /sites/YourSite/Documents/AFAIK-Dashboard/app.js
   ```

3. **Add Script Editor Web Part** to your page

4. **Paste this code**:
   ```html
   <div id="filinvest-dashboard-v2">
     <!-- Navigation and content structure from index.html -->
   </div>
   
   <script src="/sites/YourSite/Documents/AFAIK-Dashboard/data.js"></script>
   <script src="/sites/YourSite/Documents/AFAIK-Dashboard/icons.js"></script>
   <script src="/sites/YourSite/Documents/AFAIK-Dashboard/components.js"></script>
   <script src="/sites/YourSite/Documents/AFAIK-Dashboard/app.js"></script>
   ```

---

### Option 3: Single-File Deployment (Easiest)

If you need everything in ONE file for easy upload:

1. Open `index.html`
2. Replace these lines:
   ```html
   <script src="data.js"></script>
   <script src="icons.js"></script>
   <script src="components.js"></script>
   <script src="app.js"></script>
   ```

3. With the **actual content** of each .js file:
   ```html
   <script>
   // Paste contents of data.js here
   </script>
   <script>
   // Paste contents of icons.js here
   </script>
   <script>
   // Paste contents of components.js here
   </script>
   <script>
   // Paste contents of app.js here
   </script>
   ```

4. Upload the single HTML file to SharePoint

---

## 🎨 Customization Guide

### Update Projects Data
Edit `data.js` → `AppData.projects` array

```javascript
{
  id: 11,
  name: "Your New Project",
  category: "FILIGREE",
  location: "Location Here",
  type: "FILIGREE",
  status: "Pre-selling",
  description: "Short description",
  features: ["Feature 1", "Feature 2"],
  color: "#2563eb",
  units: "500",
  completion: "2027"
}
```

### Update Organization Chart
Edit `data.js` → `AppData.organization` array

### Change Colors
Edit `index.html` → Search for:
- `#003d71` (Filinvest Dark Blue)
- `#0052a3` (Filinvest Blue)
- Replace with your brand colors

---

## 🧪 Local Testing

1. Open `index.html` in a modern browser (Chrome, Edge, Firefox)
2. All features should work immediately
3. No web server required (it's pure HTML/JS)

---

## 📊 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome  | 90+     | ✅ Full Support |
| Edge    | 90+     | ✅ Full Support |
| Firefox | 88+     | ✅ Full Support |
| Safari  | 14+     | ✅ Full Support |
| IE 11   | N/A     | ❌ Not Supported |

---

## 🔒 Security Notes

- All code runs **client-side** (no server required)
- No external API calls or data transmission
- All data is embedded in `data.js`
- Safe for internal SharePoint deployment
- No authentication bypass attempts

---

## 📞 Support

For issues or questions:
1. Check browser console for JavaScript errors
2. Verify all 5 files are in the same folder
3. Ensure file URLs are accessible
4. Test in incognito mode to rule out caching

---

## 📝 Version History

**v2.0.0** (February 2026)
- Complete rewrite from React to Vanilla JS
- Modular architecture (5 separate files)
- SharePoint-safe scoped CSS
- All data migrated from React components
- 100% compatible with SharePoint Modern & Classic

---

## ⚡ Performance

- **Initial Load**: < 1 second
- **Page Navigation**: Instant (no refresh)
- **File Size**: ~150KB total (all 5 files)
- **No Dependencies**: Zero external libraries

---

## 🎯 Next Steps

1. ✅ Upload files to SharePoint
2. ✅ Test basic functionality
3. ✅ Customize data (optional)
4. ✅ Share with team
5. ✅ Collect feedback

---

**Built with ❤️ for Filinvest Alabang Incorporated**
