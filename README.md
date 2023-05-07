# TUGAS-PEMROGRAMAN-MOBILE
TUGAS PEMROGRAMAN MOBILE
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout 
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Ask Me Anything!"
        android:textSize="24sp"
        app:layout_constraintBottom_toTopOf="@+id/button"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Click Me"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView" />

</androidx.constraintlayout.widget.ConstraintLayout>
import android.content.Intent
import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
import android.view.View

class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
    }

    fun startExerciseActivity(view: View) {
        val intent = Intent(this, ExerciseActivity::class.java)
        startActivity(intent)
    }

    fun startDietActivity(view: View) {
        val intent = Intent(this, DietActivity::class.java)
        startActivity(intent)
    }

    fun startSleepActivity(view: View) {
        val intent = Intent(this, SleepActivity::class.java)
        startActivity(intent)
    }
}
// ExerciseActivity.kt
import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity

class ExerciseActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_exercise)
        // Tambahkan logika atau tampilan sesuai dengan fitur latihan
    }
}

// DietActivity.kt
import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity

class DietActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_diet)
        // Tambahkan logika atau tampilan sesuai dengan fitur diet
    }
}

// Sleep
