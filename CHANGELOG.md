# Change Log

### *(2016-04-02)*
 * change minSdkVersion to 16
 * change targetSdkVersion to 23
 * Fix [Issue #4] Add OSS license type in README.
 * Fix [Issue #5] NullPointer Exception.
 * Fix [Issue #6] android:allowBackup conflict.

--------------

### *(2015-03-14)*
 * change minSdkVersion to 10, but it won't have the parallax effect on such version
 * Reorganize the android project
 * Moved images from drawables to mipmaps.

--------------

### *(2015-02-25)*
 * Fix [Issue #3] moved to jcenter repository.
 * fixed a bug on the sample version due to a change on android 5
 * update the sample version to use jcenter repository

--------------

### *(2014-07-27)*
 * Fix [Issue #2] Update <a href="https://github.com/xgc1986/ParallaxPagerTransformer/blob/master/README.md" target="_blank">README.md</a> to avoid problem in gradle 0.8.+ ("Error:Module version com.xgc1986.ParallaxPagerTransformer:library:0.2-SNAPSHOT depends on libraries but is not a library itself")

--------------

### (0.2-SNAPSHOT) *(2014-06-23)*
 * Replace package parallaxpagerlibrary to parallaxpagertransformer
 * Added method setSpeed(float) (default = 0.2f). This change the speed of the effect during the transition between two pages
 * Deleted hardcoded values on sample
 * Updated sample

--------------

### (0.1-SNAPSHOT) *(2014-06-23)*
 * [Issue #1] Change project title to ParallaxPagerTransformer (as suggested by <a href="https://github.com/tasomaniac" target="_blank">tasomaniac</a>)
 * Exported to sonatype.org
 * Delete some resources from SampleParallaxProjectSample
 * SampleParallaxProjectSample is importing the library from sonatype
 * Fix some layout issue from SampleParallaxProjectSample

--------------

### *(2014-06-28)*
 * Add `void setBorder(int px)`. Sets a current border while de transition between twopages, the border's with is `px`.

```java
	/** ... **/

	ViewPager Pager = (ViewPager) findViewById(R.id.pager);
	ParallaxTransformer parallaxTransformer = new ParallaxTransformer(R.id.parallaxContent);
	parallaxTransformer.setBorder(3);
	mPager.setPageTransformer(false, parallaxTransformer);
	/** ... **/
```
