# Flutter Dev Notes

- [Flutter Documentation](https://flutter.dev/docs) for documentation, cookbooks and samples.
- [pub.dev](https://pub.dev/) for packages
- [DartPad](https://dartpad.dev/) for testing Dart code
- [Android Mobile App Developer Tools](https://developer.android.com) for Android development guides
- [Android Studio](https://developer.android.com/studio/intro) for Android Studio help and guides
- [Flutter | Google Codelabs](https://codelabs.developers.google.com/?product=flutter) for Flutter codelabs
- [Flutter | Udemy: Complete Flutter Course](https://www.udemy.com/course/flutter-bootcamp-with-dart/learn/lecture/17117348#overview) for Udemy Flutter course
- [Flutter Tips and Tricks](https://github.com/bizz84/flutter-tips-and-tricks/tree/main/tips) for tips and tricks

Mason package: https://pub.dev/packages/mason_cli
Templating app to generate common used files
https://www.youtube.com/watch?v=SnrHoN632NU

## Colors
Follow the [Material 3](https://m3.material.io/styles) guide lines for colors and styling 

## SQFLite errors

### dart Failed to load dynamic library 'libsqlite3.so': libsqlite3.so: cannot open shared object file: No such file or directory
If this is happening on Linux, need to install sqlite3
```bash
sudo apt install sqlite3 libsqlite3-dev
```

- [Failed to load dynamic library lib/libsqlite3.so" not found](https://github.com/simolus3/drift/issues/1073)
