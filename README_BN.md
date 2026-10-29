# Camera XX — Android Studio Project

এই প্রজেক্টে Kotlin, Jetpack Compose এবং CameraX দিয়ে বাস্তব ক্যামেরা প্রিভিউ, সামনে/পেছনের ক্যামেরা বদল, জুম, ফ্ল্যাশ এবং MediaStore-এ ছবি সেভ করার প্রাথমিক ভিত্তি আছে।

## APK বানানোর নিয়ম
1. ZIP ফাইলটি Extract করুন।
2. Android Studio-তে `CameraXX-Android-Project` ফোল্ডার খুলুন।
3. Gradle Sync সম্পন্ন হতে দিন এবং প্রয়োজন হলে Android SDK 35 ইনস্টল করুন।
4. Build > Build Bundle(s) / APK(s) > Build APK(s) নির্বাচন করুন।
5. সাধারণত APK পাওয়া যায় `app/build/outputs/apk/debug/app-debug.apk`-এ।

টার্মিনাল থেকে:
- Windows: `gradlew.bat assembleDebug`
- macOS/Linux: `./gradlew assembleDebug`

## গুরুত্বপূর্ণ সীমাবদ্ধতা
- এই প্রাথমিক সংস্করণে ক্যামেরা প্রিভিউ, ক্যাপচার, ক্যামেরা বদল, জুম, ফ্ল্যাশ এবং MediaStore সেভ যুক্ত আছে।
- Brightness/contrast slider বর্তমানে UI demonstration; সেগুলো ক্যাপচার করা ছবির pixels পরিবর্তন করে না।
- 500 filters, undo/redo editor, subject segmentation/portrait blur, sky replacement এবং in-app gallery viewer এখনও implement করা হয়নি।
- ডিভাইস/SDK/Gradle পরিবেশ অনুযায়ী build পরীক্ষা প্রয়োজন। এই ZIP তৈরি করার সময় Android Gradle build চালিয়ে যাচাই করা হয়নি।
