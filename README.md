# 🖼️ Broken Image in Gallery – File Not Loading

This QA project documents and resolves a bug where one image fails to load in a web-based photo gallery. The bug was discovered during functional testing and has been successfully reproduced, fixed, and verified.

---

## 🐞 Bug Summary

- **Issue:** One image in the gallery does not display (shows a broken image icon).
- **Cause:** The image source path was either incorrect or the image file was missing.
- **Fix:** The image reference was corrected and tested in the browser.

---

## 🎯 Project Goal

- Reproduce the broken image issue.
- Identify the root cause of the broken link.
- Implement a fix by correcting the image path or replacing the file.
- Verify that the gallery loads all images correctly.

---

## 🧪 Test Cases

| Test Case ID | Test Scenario                      | Steps to Reproduce                                           | Expected Result                         | Status |
|--------------|-------------------------------------|--------------------------------------------------------------|------------------------------------------|--------|
| TC-BIIG-001  | Navigate to gallery page            | Open gallery page in browser                                 | Page loads without errors                | ✅ Pass |
| TC-BIIG-002  | Scroll through image set            | Scroll through all displayed images                          | All images render properly               | ✅ Pass |
| TC-BIIG-003  | Identify broken image               | Stop at specific image that fails to render                  | All images should display correctly      | ❌ Fail |
| TC-BIIG-004  | Verify image source path            | Inspect element in browser dev tools                         | Source should point to valid image file  | ❌ Fail |
| TC-BIIG-005  | Fix broken image                    | Replace or correct broken image file                         | Image loads in browser                   | ✅ Pass |
| TC-BIIG-006  | Re-verify full image gallery        | Reload and test all images again after fix                   | No broken images appear                  | ✅ Pass |

---

## 📸 Screenshots

Located in the `/screenshots` folder:
- `broken_gallery_view.png`
- `fixed_gallery_view.png`

These demonstrate before/after results of the bug fix.

---

## 🔧 Tools Used

- **Browser** (Chrome) – for manual testing and inspection
- **VS Code** – for editing HTML files
- **Jira** – to track tasks and sprint flow
- **GitHub** – for version control and documentation

---

## 📁 Project Structure

```
BrokenImageGallery/
├── broken_version/
│   └── index.html       # Version with broken image
├── fixed_version/
│   └── index.html       # Version with bug fix applied
├── screenshots/
│   ├── broken_gallery_view.png
│   └── fixed_gallery_view.png
├── TestCases.md
└── README.md
```

---

## ✅ Status

All images are now loading correctly. The fix was implemented and all test cases have passed.
