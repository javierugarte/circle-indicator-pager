Circle Indicator pager
=======
[ ![Download](https://api.bintray.com/packages/javiergm/maven/CircleIndicatorPager/images/download.svg) ](https://bintray.com/javiergm/maven/CircleIndicatorPager/_latestVersion)

## Download
- Using Gradle

```groovy
    compile 'com.bikomobile:circleindicatorpager:1.0.0'
```

- Using Maven

```xml
    <dependency>
        <groupId>com.bikomobile</groupId>
        <artifactId>circleindicatorpager</artifactId>
        <version>1.0.0</version>
        <type>pom</type>
    </dependency>
```


## How to use this library

Add View to your layout

```xml
	 <com.bikomobile.circleindicatorpager.CircleIndicatorPager
            android:id="@+id/circle_indicator_pager"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_alignParentBottom="true"
            android:layout_marginBottom="28dp"
            app:ci_drawable="@drawable/blue_radius"
            app:ci_drawable_unselected="@drawable/gray_radius"
            app:ci_height="7dp"
            app:ci_width="7dp" />
```

In your class, you setter the viewpager to CircleIndicatorPager

```java
	CircleIndicatorPager indicator = (CircleIndicatorPager) findViewById(R.id.circle_indicator_pager);
	indicator.setViewPager(viewPager);
```

You can configure the indicator programatically

```java
indicator.configureIndicator(int indicatorWidth, int indicatorHeight, int indicatorMargin,
                                   @DrawableRes int indicatorBackgroundId,
                                   @DrawableRes int indicatorUnselectedBackgroundId)
```
## Custom attributes


| Attr name | Attr format | Example |
|---|---|---|
| ci_width | dimension | 5dp |
| ci_height | dimension | 5dp |
| ci_margin | dimension | 10dp |
| ci_drawable | reference | @drawable / @color |
| ci_drawable\_unselected | reference | @drawable / @color |
| ci_orientation | enum | horizontal \| vertical |
| ci_gravity | enum | top \| bottom \| left \| right \| center\_vertical \| fill\_vertical \| center\_horizontal \| fill\_horizontal \| center \| fill \| clip\_vertical \| clip\_horizontal \| start \| end |

## Contribute


## About me


## License

```
Copyright 2016 Javier González

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

