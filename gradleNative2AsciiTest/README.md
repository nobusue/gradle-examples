gradleNative2AsciiTest
======================

Test for processing platform non-native resources.

Please try

`gradle clean processResources asciiToNative`

If you are using Windows and not setting -Dfile.encoding=UTF-8, you will see *build/resources/main/reverse/test.utf8.properties* corrupted.

`gradle clean nativeToAscii asciiToNative`

will generate non-corruted *build/resources/main/reverse/test.utf8.properties* .

If you are not Windows user, please modify `nativeToAscii` task in build.gradle.
