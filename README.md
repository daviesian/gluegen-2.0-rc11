  gluegen
==============

#### A modified version of gluegen which loads native libs from current JAR.

Specifically for use with JOGL v2.0 RC11, included in first commit.

Produces a jar file with a complete JOGL distribution inside, suitable for use on all platforms.

### How main jar was created

- Extract gluegen-java-src.zip from jogamp-all-platforms.7z
- Modify four classes to load native libs from current JAR.
- Merge all of gluegen-rt.jar into jogl.all.jar (which can also be extracted from jogamp-all-platforms.7z)
- Replace those four classes in jogl.all.jar
- Extract all gluegen-rt-natives-*.jar into the root of jogl.all.jar.
- Extract all jogl-natives-*.jar into separate folders in jogl.all.jar/native
- Rename jogl.all.jar to jogl.all.cl-2.0.1.jar

### Author

* Ian Davies 
