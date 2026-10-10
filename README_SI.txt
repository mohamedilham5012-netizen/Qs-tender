QS Rate Finder Pro - Android Studio project + phone-only cloud build workflow
=============================================================================

ZIP-இல் Android project source உள்ளது; இது நேரடியாக install செய்யக்கூடிய APK அல்ல.
Android SDK/Gradle build tools இந்த chat environment-ல் இல்லை; ஆகவே APK compile செய்து verify செய்ய இயலவில்லை.

PHONE மட்டும் இருந்தால்:
- PHONE_BUILD_SI.txt-ஐப் பாருங்கள்.
- .github/workflows/build-apk.yml GitHub Actions மூலம் cloud-ல் debug APK உருவாக்கும்.
- GitHub repository-க்கு extracted project files upload செய்ய வேண்டும்; ZIP மட்டும் upload செய்தால் workflow இயங்காது.

Project features bundled from the HTML prototype:
- Rate search and best-match display
- BOQ image OCR using an online-loaded Tesseract library
- PDF / Excel import functions using online-loaded browser libraries
- CSV export
- Built-in sample rates from the provided Kurunegala 2026 2nd Half PDF

Note: Camera, OCR, PDF/Excel import and matching need device/browser testing. Check source schedule before using any rate in an estimate.
