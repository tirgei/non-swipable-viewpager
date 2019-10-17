# Preferences Helper

[![](https://jitpack.io/v/tirgei/non-swipable-viewpager.svg)](https://jitpack.io/#tirgei/non-swipable-viewpager)
[![BCH compliance](https://bettercodehub.com/edge/badge/tirgei/non-swipable-viewpager?branch=master)](https://bettercodehub.com/)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/e2d93e7d107d48a69cc04aa3c9cff8b4)](https://www.codacy.com/manual/tirgei/non-swipable-viewpager?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=tirgei/non-swipable-viewpager&amp;utm_campaign=Badge_Grade)

An android library to implement a non-swipable ViewPager

### Download
You can add the library to your project via gradle

Step 1: Add in your root build.gradle of your project
```
    allprojects {
        repositories {
            ...
            maven { url 'https://jitpack.io' }
        }
    }
```

Step 2: Add the dependency to your app gradle
```

    dependencies {
    	...
	implementation 'com.github.tirgei:non-swipable-viewpager:{latest-version}'
	...
    }

```


### Usage
To use the library, add it to your xml layout. The library uses the default viewpager functions

```
<com.gelostech.nonswipableviewpager.NonSwipeableViewPager
        android:id="@+id/viewpager"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_below="@id/appbar"/>
```

From your Activity/ Fragment, set your ViewPagerAdapter to the NonSwipableViewPager
```
    // Kotlin
    val adapter = PagerAdapter(supportFragmentManager, this)
    viewpager.adapter = adapter

    // Java
    PagerAdapter adapter = new PagerAdapter(getSupportFragmentManager(), this);
    viewpager.setAdapter(adapter);
```

### License
```
MIT License

Copyright (c) 2019 Vincent Tirgei

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```