# My First App — Android APK project
## বাংলায় APK build করার নিয়ম
1. এই ZIP extract করো।
2. GitHub-এ একটি নতুন repository তৈরি করো।
3. Extract করা সব ফাইল repository-র root-এ upload/commit করো (শুধু ZIP ফাইলটি নয়)।
4. repository-র Actions tab খোলো। প্রথমবার GitHub Actions enable করতে হতে পারে।
5. **Build Android APK** workflow নির্বাচন করে **Run workflow** চাপো। main branch-এ push করলেও build শুরু হবে।
6. Build শেষ হলে workflow run-এর নিচের **Artifacts** থেকে `android-debug-apk` download করো।
7. Artifact ZIP extract করলে `app-debug.apk` পাবে।

## গুরুত্বপূর্ণ
- এটি একটি **debug APK**, পরীক্ষা ও sideload করার জন্য। Play Store release-এর জন্য আলাদা signed release build ও keystore দরকার।
- ZIP project-এ `www/index.html` থাকতে হবে। আপলোড করা ZIP-এর ভেতরের HTML/CSS/JS ফাইলগুলো `www/`-এ রাখা হয়।
- Android APK তৈরি করতে GitHub Actions-এ internet access ও Android SDK build environment লাগে।
- GitHub account-এ repository এবং Actions ব্যবহারের অনুমতি থাকতে হবে।
