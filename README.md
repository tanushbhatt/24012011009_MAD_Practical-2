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
     <td><img width="1722" height="280" alt="image" src="https://github.com/user-attachments/assets/b34b71a3-8c78-4d4a-bf27-6a64aa5b0fc6" /></td>
      <td><img width="1917" height="502" alt="image" src="https://github.com/user-attachments/assets/8a8039c2-90df-4c1e-a7d7-a7409d9c1e5c" /></td>
  </tr>
    <tr>
        <td><img width="1917" height="501" alt="image" src="https://github.com/user-attachments/assets/bae372a9-4f7a-4bea-bdd6-661f43bba34b" /></td>
        <td><img width="1917" height="498" alt="image" src="https://github.com/user-attachments/assets/901ae0dc-3632-4812-8fd5-31314c75bc72" /></td>
    </tr>
  <tr>
      <td><img width="1917" height="495" alt="image" src="https://github.com/user-attachments/assets/cc0a81d2-4304-4b7d-94a1-d72dbfe95a71" /></td>
      <td><img width="386" height="862" alt="image" src="https://github.com/user-attachments/assets/d564400a-0776-4103-9ff5-fe80122ddf8f" /></td>
  </tr>
</table>
