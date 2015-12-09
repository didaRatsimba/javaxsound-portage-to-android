# javaxsound-portage-to-android
It sucks when you need to use javax.sound in an android project (dalvik limitation), here is the solution : 
To build the project, just launch mvn clean package and add the created jar to the lib directory of the android project.
Be careful, you have to use the classes from this jar (mg.dida.*) and never use javax.sound.* or com.sun.media.sound.* directly in your class. It compiles but throw exceptions at runtime.
