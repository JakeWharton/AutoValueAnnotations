AutoValue Annotations
=====================

A standalone packaging of the annotations from [Google's AutoValue library][1].

When using AutoValue with Gradle it is _highly_ inconvenient to specify the dependency both as
`apt` and `provided`. Doing so leaks all of AutoValue's annotation processor code and its
shaded dependencies into your classpath. This project allows you to only depend on the annotations
as `provided` and specify the processor only as an `apt` dependency.

With any luck, [AutoValue issue #268][4] will be implemented sometime in the future obviating the
need for this repacking.


Download
--------

```groovy
apt 'com.google.auto.value:auto-value:1.2'
provided 'com.jakewharton.auto.value:auto-value-annotations:1.2-update1'
```


Change Log
----------

This project contains no code. See [AutoValue's change log][2] instead.


License
-------

This project contains no code. See [AutoValue's license][3] instead.







 [1]: https://github.com/google/auto/
 [2]: https://github.com/google/auto/blob/master/value/CHANGES.md
 [3]: https://github.com/google/auto/blob/master/LICENSE.txt
 [4]: https://github.com/google/auto/issues/268
