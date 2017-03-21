# Steps
1. Follow the instructions https://github.com/Yelp/ffmpeg-android
2. Clone a project for assembling aar file https://github.com/WritingMinds/ffmpeg-android-java
3. ./gradlew assembleRelease

## Errors
### Step 2
Error:(2, 0) No service of type Factory<LoggingManagerInternal> available in ProjectScopeServices.
    <a href="openFile:/Users/sashatinkoff/Downloads/ffmpeg-android-java-master/FFmpegAndroid/build.gradle">Open File</a>
    
    Update build.gralde for module FFmpegAndroid. Change classpath 'com.github.dcendents:android-maven-gradle-plugin:1.3' to the last one. You can get a recent version of the plugin here https://github.com/dcendents/android-maven-gradle-plugin
