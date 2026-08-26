# Practical-2: Activity Life Cycle and Basic UI

## AIM

Create an Android application to demonstrate the functions of the
**Activity Life Cycle** and **Basic UI**.

The application displays **"Hello World!"** in a `TextView` at the
center of the Activity screen with:

-   Yellow layout background (`#FFFF00`)
-   Holo Blue Bright text color
-   27sp text size
-   Bold and Italic text style

The application also demonstrates:

-   Activity Life Cycle methods
-   Log messages in Logcat
-   Toast messages
-   Snackbar messages
-   Basic `ConstraintLayout` properties
-   TextView properties and ID generation
-   Android built-in color resources

------------------------------------------------------------------------

## Study / Concepts

### 1. TextView

A `TextView` is used to display text on the Android screen.

Important properties used in this practical:

``` xml
android:text="Hello World!"
android:textColor="@android:color/holo_blue_bright"
android:textSize="27sp"
android:textStyle="bold|italic"
```

### 2. Layout Background

The Activity layout uses a yellow background:

``` xml
android:background="#FFFF00"
```

### 3. Toast Message

A Toast displays a short message to the user.

Example:

``` kotlin
Toast.makeText(
    this,
    "onResume function called.",
    Toast.LENGTH_SHORT
).show()
```

### 4. Snackbar Message

A Snackbar displays a short message at the bottom of the screen.

Example:

``` kotlin
Snackbar.make(
    findViewById(R.id.myCoordinatorLayout),
    "onResume function called.",
    Snackbar.LENGTH_SHORT
).show()
```

### 5. Log Message

Log messages are used to display Activity Life Cycle information in
**Logcat**.

Example:

``` kotlin
Log.i("MainActivity", "onResume function called.")
```

------------------------------------------------------------------------

## Activity Life Cycle

The practical demonstrates the Activity Life Cycle methods by printing
messages in Logcat.

The main methods are:

``` text
onCreate()
onStart()
onResume()
onPause()
onStop()
onRestart()
onDestroy()
```

These methods are called at different stages of an Activity's life.

For example:

``` kotlin
override fun onStart() {
    super.onStart()
    Log.i("MainActivity", "onStart function called.")
}

override fun onResume() {
    super.onResume()
    Log.i("MainActivity", "onResume function called.")
}
```

The messages can be viewed in **Android Studio → Logcat**.

------------------------------------------------------------------------

## Basic UI

The main screen contains a `TextView` displaying:

``` text
Hello World!
```

The TextView is placed in the center of the Activity.

Its appearance is:

-   **Text:** Hello World!
-   **Text Color:** Holo Blue Bright
-   **Text Size:** 27sp
-   **Text Style:** Bold + Italic
-   **Background:** Yellow

------------------------------------------------------------------------

## Output

### Log Message in Logcat

The Activity Life Cycle methods are displayed in Logcat using Log
messages.

![Log Message in Logcat](screenshots/logcat.png)

### Snackbar Message

A Snackbar message is displayed at the bottom of the screen.

![Snackbar Message](screenshots/snackbar.png)

### Toast Message

A Toast message is displayed at the bottom of the screen.

![Toast Message](screenshots/toast.png)

------------------------------------------------------------------------

## Practical Requirements

This practical demonstrates the following:

-   TextView and its properties
-   Toast Message
-   Snackbar Message
-   Android built-in resources such as colors
-   Activity Life Cycle
-   Log Message in Logcat
-   Properties of `ConstraintLayout`
-   Generating an ID for a TextView

------------------------------------------------------------------------

## Result

The Android application successfully demonstrates **Basic UI** and the
**Activity Life Cycle** using Logcat, Toast, and Snackbar messages.
<table>
  <tr>
    <td><img width="1917" height="1077" alt="Screenshot 2026-07-04 224905" src="https://github.com/user-attachments/assets/21773f86-33be-4ab8-8082-4022ba3ad63b" /></td>
    <td><img width="1917" height="1078" alt="Screenshot 2026-07-04 011955" src="https://github.com/user-attachments/assets/a97c794d-4bd9-4bf0-bace-cd30713e31ef" /></td>
    <td><img width="1917" height="1075" alt="Screenshot 2026-07-04 012009" src="https://github.com/user-attachments/assets/cf5073aa-730b-4fd5-8167-9abf6df59120" /></td>
  </tr>
  <tr>
    <td><img width="1917" height="1078" alt="Screenshot 2026-07-04 012028" src="https://github.com/user-attachments/assets/012ed086-5e7b-4c79-8c3d-e10cbf72b12f" /></td>
    <td><img width="1912" height="1078" alt="Screenshot 2026-07-04 012454" src="https://github.com/user-attachments/assets/3db7a652-71a9-45e1-bdfd-e02dd342016e" /></td>
    <td><img width="1917" height="1077" alt="Screenshot 2026-07-09 224455" src="https://github.com/user-attachments/assets/92b6a67d-f1dc-4d8f-aee8-95b0f048e580" /></td>
  </tr>
  <tr>
    <td><img width="1917" height="1077" alt="Screenshot 2026-07-09 225146" src="https://github.com/user-attachments/assets/89c859a7-5f47-4c65-8c16-70dd00cfa48b" /></td>
  </tr>
</table>
