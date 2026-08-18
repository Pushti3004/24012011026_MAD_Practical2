# Practical-2: Android Activity Life Cycle and Basic UI

## Aim
To create an Android application that demonstrates the **Activity Life Cycle** and basic Android UI components using `TextView`, `Toast`, `Log`, and `ConstraintLayout`.

## Tools Required
- Android Studio
- Android SDK
- Kotlin
- Android Emulator or Android device

## Practical Objectives

### 2.1 Create Basic Android UI
Create an Activity containing a `TextView` that displays **"Hello World"** at the center of the Activity screen.

The Activity layout should have:
- **Background color:** Yellow (`#FFFF00`)
- **Text:** Hello World
- **Text color:** Holo Blue Bright (`@android:color/holo_blue_bright`)
- **Text size:** `27sp`
- **Text style:** Bold and Italic
- **TextView position:** Center of the Activity screen

### 2.2 Study TextView and Its Properties
Understand the commonly used `TextView` properties, including:
- `android:id`
- `android:text`
- `android:textColor`
- `android:textSize`
- `android:textStyle`
- `android:layout_width`
- `android:layout_height`

### 2.3 Study ConstraintLayout
Understand the properties and constraints of `ConstraintLayout`, including:
- Start and end constraints
- Top and bottom constraints
- Width and height
- Margins
- Centering a view using constraints
- Generating an ID for a `TextView`

### 2.4 Demonstrate Activity Life Cycle
Implement all major Activity life-cycle callback methods:

1. `onCreate()`
2. `onStart()`
3. `onResume()`
4. `onPause()`
5. `onStop()`
6. `onRestart()`
7. `onDestroy()`

Display a **Log message** whenever each method is called.

### 2.5 Log Message in Logcat
Use Android's `Log` class to display Activity life-cycle messages in **Logcat**.

Example:

```kotlin
Log.d("ActivityLifeCycle", "onCreate() called")
```

The Logcat should show the sequence of life-cycle methods as the Activity moves between different states.

### 2.6 Toast Message
Use `Toast` to display short messages when Activity life-cycle methods are executed.

Example:

```kotlin
Toast.makeText(this, "onCreate Called", Toast.LENGTH_SHORT).show()
```

Toast messages provide quick visual feedback to the user.

## Activity Life Cycle

The Activity life cycle represents the different states through which an Android Activity passes during its lifetime.

### Normal Execution Flow

```text
onCreate()
    ↓
onStart()
    ↓
onResume()
    ↓
Activity Running
    ↓
onPause()
    ↓
onStop()
```

If the stopped Activity is opened again:

```text
onRestart()
    ↓
onStart()
    ↓
onResume()
```

When the Activity is permanently removed:

```text
onDestroy()
```

## Expected Learning Outcomes

After completing this practical, the student will be able to:

1. Create a basic Android Activity.
2. Design a simple UI using `TextView`.
3. Apply TextView properties such as text color, size, and style.
4. Use `ConstraintLayout` to position UI components.
5. Generate and use IDs for Android views.
6. Understand the Android Activity life cycle.
7. Implement Activity life-cycle callback methods.
8. Display debugging information using `Log`.
9. View Activity life-cycle messages in Logcat.
10. Display temporary messages using `Toast`.
11. Use Android built-in resources such as colors.

## Conclusion
This practical provides hands-on experience with basic Android UI development and the Activity Life Cycle. It demonstrates how to create and configure a `TextView`, use `ConstraintLayout`, display `Toast` messages, and monitor Activity life-cycle methods through Logcat.
