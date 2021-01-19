# DarkModeDisableForce
 
- Change value in `themes.xml`
```xml
<resources xmlns:tools="http://schemas.android.com/tools">
    <!-- Base application theme. -->
    <style name="Theme.DarkModeDisableForce" parent="Theme.MaterialComponents.Light.DarkActionBar">
        <!-- Primary brand color. -->
        <item name="colorPrimary">@color/purple_500</item>
        <item name="colorPrimaryVariant">@color/purple_700</item>
        <item name="colorOnPrimary">@color/white</item>

        <!-- Secondary brand color. -->
        <item name="colorSecondary">@color/purple_500</item>
        <item name="colorSecondaryVariant">@color/purple_700</item>
        <item name="colorOnSecondary">@color/white</item>
        <!-- Status bar color. -->
        <item name="android:statusBarColor" tools:targetApi="l">?attr/colorPrimaryVariant</item>
        <!-- Customize your theme here. -->

        <!-- Disbale Dark Mode. -->
        <item name="android:forceDarkAllowed" tools:targetApi="q">false</item>
    </style>
</resources>
```
note :
1. Use `Theme.MaterialComponents.Light.DarkActionBar` as parent
2. Change value item `colorSecondary`, `colorSecondaryVariant`, `colorOnSecondary`. (Optional)
3. Add `<item name="android:forceDarkAllowed" tools:targetApi="q">false</item>` in parent style item

---

```
Copyright 2021 M. Fadli Zein
```