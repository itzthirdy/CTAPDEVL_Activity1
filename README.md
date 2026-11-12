# CTAPDEVL - Activity 1: About Me Screen

An introductory Android application project built using Android Studio to demonstrate fundamental layout design, XML attribute configuration, and ConstraintLayout positioning.

---

## 📋 Student & Course Information

* **Student Name:** Cesar S. Jondiz III
* **Course:** CTAPDEVL (App Development and Emerging Technologies)
* **Section:** INF25A
* **Submission Date:** November 12, 2026
* **Activity:** Hands-On Activity – Build Your "About Me" Screen

---

## 🛠️ Tech Stack & Environment

* **IDE:** Android Studio
* **Language:** Java
* **UI Framework:** Android Views / XML Layouts
* **Layout Manager:** `androidx.constraintlayout.widget.ConstraintLayout`
* **Target Emulator/Device:** Medium Phone API 37.0

---

## 📱 Implementation Details

The activity required modifying `res/layout/activity_main.xml` to display a customized name banner with custom typography and background styling:

* **Screen Background:** Configured container background hex color to `#F7F5EF`.
* **Primary TextView:** Configured with custom text (`Cesar S. Jondiz III!`), styled in bold red (`#FF0000`), with an expanded text size of `38sp`.
* **Constraints:** Anchored to all parent edges (`top`, `bottom`, `start`, `end`) to ensure consistent centered alignment across screen densities.

### XML Layout (`activity_main.xml`)

```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="[http://schemas.android.com/apk/res/android](http://schemas.android.com/apk/res/android)"
    xmlns:app="[http://schemas.android.com/apk/res-auto](http://schemas.android.com/apk/res-auto)"
    xmlns:tools="[http://schemas.android.com/tools](http://schemas.android.com/tools)"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#F7F5EF"
    tools:context=".MainActivity">

    <TextView android:layout_height="wrap_content" android:layout_width="wrap_content" android:text="Cesar S. Jondiz III!" android:textColor="#FF0000" android:textSize="38sp" android:textStyle="bold" app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent"/>

</androidx.constraintlayout.widget.ConstraintLayout>
