# ColorPicker

This is a custom component for Android that allows you to select a custom color.

## Requeriments

- API 24 or more.

## Setup dependencies

### Gradle

```gradle
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
dependencies {
    implementation 'com.github.dgqdev:ColorPicker:1.0.1'
}
```

### Maven

```xml
<!-- <repositories> section of pom.xml -->
<repository>
    <id>jitpack.io</id>
   <url>https://jitpack.io</url>
</repository>
```

```xml
<!-- <dependencies> section of pom.xml -->
<dependency>
    <groupId>com.github.dgqdev</groupId>
    <artifactId>ColorPicker</artifactId>
    <version>1.0.1</version>
</dependency>
```

## Usage

```xml

<com.dgqdev.colorpicker.ColorPicker 
    android:id="@+id/colorPicker"
    android:layout_height="wrap_content" 
    android:layout_width="match_parent" />
```

```kt
// Get color programatically
val selectedColor = colorPicker.getSelectedColorHex()
```

## ColorPicker attributes

| Attribute              | Format          | Default value |
|------------------------|-----------------|---------------|
| initialColor           | reference/color | null          |
| showColorPickedPointer | boolean         | true          |
