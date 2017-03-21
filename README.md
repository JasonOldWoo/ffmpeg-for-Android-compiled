# ffmpeg-for-Android-compiled
## About

These are generated files of https://github.com/WritingMinds/ffmpeg-android-java but they are separated on different AAR files for different architecture (to decrease a size of your application). You can find samples which can be helpful for you here http://writingminds.github.io/ffmpeg-android-java/.
Please keep in mind that you should change build.gradle to use compiled AAR files instead of compiling library

## How to include files in your project

To make it work use flavors as follows in your app/build.gradle

flavorDimensions "architecture"

    productFlavors {
        arm {
            dimension "architecture"
        }
        x86 {
            dimension "architecture"
        }
    }
    
    ....
    armCompile(name: 'ffmpeg_arm.0.3.2', ext: 'aar')
    x86Compile(name: 'ffmpeg_x86.0.3.2', ext: 'aar')
    
    
Please keep in mind that compiled aar files should be located in app/libs.

Now you can assemble a project for certain architecture using gradle flavors.
