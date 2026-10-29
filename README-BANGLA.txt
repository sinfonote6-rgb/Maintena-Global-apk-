MAINTENA Android APK project

গুরুত্বপূর্ণ: এই পরিবেশে Android SDK/Gradle build tool নেই, তাই এখানে সরাসরি APK compile করা যায়নি। এই project-এ আপনার Maintena HTML app Android WebView-এর মধ্যে রাখা হয়েছে এবং GitHub Actions দিয়ে APK বানানোর workflow আছে।

সহজ উপায়:
1. ZIP ফাইলটি extract করুন।
2. GitHub-এ নতুন repository তৈরি করুন (যেমন maintena-android)।
3. ZIP extract করা ফোল্ডারের ভেতরের সব ফাইল repository-তে upload করুন; .github ফোল্ডারটিও থাকতে হবে।
4. GitHub repository-তে Actions tab খুলুন।
5. “Build Maintena APK” workflow নির্বাচন করে “Run workflow” চাপুন।
6. Build শেষ হলে workflow run খুলুন, নিচের Artifacts অংশ থেকে “Maintena-debug-APK” download করুন।
7. ZIP artifact extract করে app-debug.apk Android ফোনে পাঠিয়ে install করুন। Android-এ অজানা উৎস থেকে install করার অনুমতি দিতে হতে পারে।

ডেমো লগইন:
Admin: admin@maintena.demo / admin123
Technician: ID 1 / 1111

সীমাবদ্ধতা:
- এটি আপনার বর্তমান demo app-কে APK wrapper-এর মধ্যে চালায়; cloud database বা secure authentication যোগ করে না।
- ডেটা ডিভাইসের local storage-এ থাকে। অ্যাপ uninstall করলে ডেটা হারাতে পারে।
- এটি debug APK; Google Play-তে প্রকাশের জন্য signed release build, app icon, privacy policy, এবং প্রয়োজনীয় পরীক্ষা দরকার।
- Demo credentials বাস্তব নিরাপদ লগইন নয়। বাস্তব factory/customer data ব্যবহার করবেন না।
