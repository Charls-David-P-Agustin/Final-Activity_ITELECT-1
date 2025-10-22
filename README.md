# Final-Activity_ITELECT-1


// This is the main background of the GUI design//

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:background="#C8A789"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="18dp"
    android:gravity="center"
    tools:context=".MainActivity">

// This is the First Text of greetings
    <TextView
        android:id="@+id/textViewWelcome"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Welcome to Android UI"
        android:textSize="18sp"
        android:fontFamily="sans-serif-medium"
        android:textColor="#000000"
        android:padding="8dp"
        android:layout_marginTop="32dp"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />

    // this is the second text which is the question for visiting 
    <TextView
        android:id="@+id/textViewInstructions"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:text="What are you looking for?"
        android:textStyle="bold"
        android:fontFamily="sans-serif-medium"
        android:textSize="16sp"
        android:padding="8dp"
        android:layout_marginTop="12dp"
        app:layout_constraintTop_toBottomOf="@id/textViewWelcome"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />

    //and this is the last text for all
    <TextView
        android:id="@+id/textViewLabel2"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:text="Choices:"
        android:fontFamily="sans-serif-medium"
        android:textSize="18sp"
        android:padding="4dp"
        android:textStyle="bold"
        android:layout_marginTop="12dp"
        app:layout_constraintTop_toBottomOf="@id/textViewInstructions"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />

    // This body part are typing their to what they looking for
    <EditText
        android:id="@+id/editTextInput"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:hint="Enter the country"
        android:fontFamily="sans-serif-medium"
        android:textColor="#000000"
        android:textStyle="bold"
        android:padding="12dp"
        android:textSize="24sp"
        android:layout_marginTop="16dp"
        app:layout_constraintTop_toBottomOf="@id/textViewLabel2"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />

    // This part we have a 5 option to what we choosing for the items
    <AutoCompleteTextView
        android:id="@+id/autoCompleteCountry"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:hint="Select a item"
        android:fontFamily="sans-serif-medium"
        android:textColor="#000000"
        android:padding="12dp"
        android:textSize="24sp"
        android:layout_marginTop="16dp"
        app:layout_constraintTop_toBottomOf="@id/editTextInput"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />

    // it showing all the 5 options about on our input
    <Spinner
        android:id="@+id/spinnerOptions"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        app:layout_constraintTop_toBottomOf="@id/autoCompleteCountry"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />


    // 
    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="36dp"
        android:layout_marginTop="132dp"
        android:text="Button"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@id/imageButton" />

    // This is the power button to open it or close of GUI
    <ToggleButton
        android:id="@+id/toggleButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="184dp"
        android:layout_marginTop="236dp"
        android:text="ON/OFF"
        app:layout_constraintStart_toEndOf="@id/button"
        app:layout_constraintTop_toBottomOf="@id/spinnerOptions" />

    // This are the 1st image of the items
    <ImageButton
        android:id="@+id/imageButton"
        android:layout_width="161dp"
        android:layout_height="99dp"
        android:layout_marginTop="8dp"
        android:scaleType="fitCenter"
        android:src="@drawable/football"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@id/spinnerOptions" />


    // This are 2nd image for switching
    <ImageSwitcher
        android:id="@+id/imageSwitcher"
        android:layout_width="222dp"
        android:layout_height="129dp"
        android:inAnimation="@android:anim/fade_in"
        android:outAnimation="@android:anim/fade_out"
        app:layout_constraintDimensionRatio="16:9"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHeight_default="percent"
        app:layout_constraintHeight_percent="0.25"
        app:layout_constraintHorizontal_bias="1.0"
        app:layout_constraintStart_toStartOf="parent"
        tools:layout_editor_absoluteY="346dp">

        //
        <ImageView
            android:id="@+id/imageView"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:src="@drawable/basketball_8147489_1280" />
    </ImageSwitcher>

    // This is the Switch button for two images are switch to each other
    <Button
        android:id="@+id/buttonSwitchImage"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="64dp"
        android:text="Switch Image"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@id/imageSwitcher" />

    //
    <ImageView
        android:id="@+id/imageView3"
        android:layout_width="159dp"
        android:layout_height="162dp"
        android:src="@drawable/football_8266065_1280"
        app:layout_constraintStart_toStartOf="parent"
        tools:layout_editor_absoluteY="338dp" />

</androidx.constraintlayout.widget.ConstraintLayout>
