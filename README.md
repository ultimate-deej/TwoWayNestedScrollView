[![](https://jitpack.io/v/ultimate-deej/TwoWayNestedScrollView.svg)](https://jitpack.io/#ultimate-deej/TwoWayNestedScrollView)

# Overview
A `NestedScrollView` modified to scroll along both axes.

- [x] Scrolling in both dimensions at the same time
- [x] `liftOnScroll`*
- [x] `fillViewport` works in both dimensions too
- [x] X-Axis keyboard navigation

<sub>*The entirety of the nested scroll thing has not been tested much, but lift on scroll feature of AppBarLayout works just fine.</sub>

# Installation
```gradle
repositories {
    // your repos
    maven { url "https://jitpack.io" }
}
```
```gradle
dependencies {
    implementation 'com.github.ultimate-deej:twowaynestedscrollview:0.1'
}
```
### or
Just copy [this file](/lib/src/main/java/org/deejdev/twowaynestedscrollview/TwoWayNestedScrollView.java) to your project.

# Contributing

The purpose of this library is to provide a fork of `NestedScrollView` that can scroll in both dimensions, while making the least possible changes to the logic. As a result:

### What *may* be accepted
- Fixes for bugs introduced in this fork

### What will **NOT** be accepted
- Fixes for bugs existing in the Google's original implementation will **NOT** be accepted
- New features will **NOT** be accepted
- Everything else

# What has been changed?
Except for making X-axis logic align with its Y-axis counterpart, no other changes have been made to how the widget works. The essential [commit](//github.com/ultimate-deej/TwoWayNestedScrollView/commit/80472c3c24f3ff469b3a8669e1518977fb1477ec) you are looking for.

# Known issues
There has been no changes made to accessibility and focus handling, and just partially to keyboard navigation.
