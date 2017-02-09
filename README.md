# ffmpeg-for-Android-compiled
It's a complete file that can be used in your Android project

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
    
    
Please keep in mind that compiled aar files should be located in app/libs.

Now you can assemble a project for certain architecture using gradle flavors.
