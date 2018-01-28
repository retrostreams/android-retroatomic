# android-retroatomic

![](art/streamsupport-sf.png)

android-retroatomic is a backport of the java.util.concurrent.atomic classes added in Java 8 (DoubleAccumulator, LongAccumulator, DoubleAdder and LongAdder) for Android developers wanting to use the Android Studio 3.0 desugar toolchain.

There is nothing specific to Android or the desugar toolchain in this code (it could even be compiled to Java 6 bytecode) but it has a dependency on [android-retrostreams](https://github.com/retrostreams/android-retrostreams) which is why this exists as a separate component (the corresponding [streamsupport-atomic](https://sourceforge.net/p/streamsupport/code/ci/default/tree/src/atomic/) component can't be used with android-retrostreams
and [android-retrostreams](https://github.com/retrostreams/android-retrostreams) itself can *only* be used with desugar or Java 8 / 9).

Other than having a different package name this code has no further changes compared with [streamsupport-atomic](https://sourceforge.net/p/streamsupport/code/ci/default/tree/src/atomic/)

Online Javadoc is available at [docs](https://retrostreams.github.io/android-retroatomic/apidocs/index.html)

Please give feedback [here](https://github.com/retrostreams/android-retroatomic/issues) if you experience any problems.


### build.gradle:

```gradle
dependencies {
    compile 'net.sourceforge.streamsupport:android-retroatomic:1.6.1'
}
```

## LICENSE

GNU General Public License, version 2, with the Classpath Exception
