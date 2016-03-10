# RadioButtons_Example


![Exaxmple](art/capture.png)

```xml
<resources>

  <style name="AppTheme"
         parent="Theme.AppCompat.Light.DarkActionBar">

    <item name="colorPrimary">@color/colorPrimary</item>
    <item name="colorPrimaryDark">@color/colorPrimaryDark</item>
    <item name="colorAccent">@color/colorAccent</item>
    <item name="radioButtonStyle">@style/elmeutema_style</item>
    <item name="elradiobuttonraret">@style/red_radio_style</item>
  </style>

  <style name="elmeutema_style"
         parent="@style/Widget.AppCompat.CompoundButton.RadioButton">
    <item name="colorAccent">#0000FF</item>
    <item name="android:textColorSecondary">#ff0000</item>
  </style>


  <style name="red_radio_style"
         parent="@style/Widget.AppCompat.CompoundButton.RadioButton">
    <item name="colorAccent">#ff0000</item>
    <item name="android:textColorSecondary">#760e0e</item>
  </style>


  <style name="elmeutema">
    <item name="colorAccent">#0000FF</item>
    <item name="android:textColorSecondary">#ff0000</item>
  </style>


  <style name="red_radio">
    <item name="colorAccent">#ff0000</item>
    <item name="android:textColorSecondary">#760e0e</item>
  </style>


</resources>


```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingLeft="@dimen/activity_horizontal_margin"
    android:paddingRight="@dimen/activity_horizontal_margin"
    android:paddingTop="@dimen/activity_vertical_margin"
    android:paddingBottom="@dimen/activity_vertical_margin"
    android:orientation="vertical"
    tools:context="com.alorma.radiobuttons.MainActivity"
    >

  <RadioButton
      android:layout_width="match_parent"
      android:layout_height="wrap_content"
      android:text="Hello default"
      android:checked="true"
      />

  <RadioButton
      android:layout_width="match_parent"
      android:layout_height="wrap_content"
      android:text="Hello blue with parent"
      android:theme="@style/elmeutema_style"
      android:checked="true"
      />

  <RadioButton
      android:layout_width="match_parent"
      android:layout_height="wrap_content"
      android:text="Hello red with parent"
      android:theme="@style/red_radio_style"
      android:checked="true"
      />

  <RadioButton
      android:layout_width="match_parent"
      android:layout_height="wrap_content"
      android:text="Hello blue"
      android:theme="@style/elmeutema"
      android:checked="true"
      />

  <RadioButton
      android:layout_width="match_parent"
      android:layout_height="wrap_content"
      android:text="Hello red"
      android:theme="@style/red_radio"
      android:checked="true"
      />

</LinearLayout>

```
