# Libaums Wrapper for EtchDroid

This library is a shim to adapt [libaums](https://github.com/magnusja/libaums) to EtchDroid's needs.

Previously EtchDroid used a fork in order to add the required features. However, right now enough
patches have been merged to libaums so that a hard fork is not needed any more and a simple
wrapper library suffices.

## How to use

Root `build.gradle`:

```gradle
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
}
```

Module `build.gradle`:

```gradle
dependencies {
	        api 'com.github.EtchDroid:libaums_wrapper:v0.1.1'
}
```

Do not also include Libaums as it's pulled in as a dependency.

## License

Licensed under the Apache 2.0 license.
