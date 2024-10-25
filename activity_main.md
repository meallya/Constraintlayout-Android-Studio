<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#F0F0F0"
    tools:ignore="ExtraText">

    <!-- Judul -->
    <TextView
        android:id="@+id/title"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:text="Blissful Botanicals"
        android:textSize="24sp"
        android:textStyle="italic"
        android:textColor="#4A4A4A"
        android:gravity="center"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        android:padding="16dp"
        app:layout_constraintHorizontal_bias="0.5"/>

    <!-- Deskripsi Singkat -->

    <!-- Gambar Skincare -->
    <TextView
        android:id="@+id/description"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:padding="16dp"
        android:text="Skintific Niacinamide Moisturizer hydrates and minimizes pores with 5% Niacinamide for fresh, radiant skin.

"
        android:textColor="#7D7D7D"
        android:textSize="16sp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/title" />

    <!-- Horizontal Scroll View untuk tombol -->

    <ImageView
        android:id="@+id/skincareImage"
        android:layout_width="0dp"
        android:layout_height="200dp"
        android:layout_margin="16dp"
        android:layout_marginTop="16dp"
        android:contentDescription="Gambar Skincare"
        android:scaleType="centerCrop"
        android:src="@drawable/skincare"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/description" />

    <HorizontalScrollView
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        app:layout_constraintTop_toBottomOf="@+id/skincareImage"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        android:padding="16dp">

        <LinearLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:orientation="horizontal">

            <!-- Tombol 1 -->
            <Button
                android:id="@+id/button1"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginEnd="8dp"
                android:backgroundTint="#FFB3BA"
                android:text="Contact"
                android:textColor="#FFFFFF"/>

            <!-- Tombol 2 -->
            <Button
                android:id="@+id/button2"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginEnd="8dp"
                android:backgroundTint="#FFB3BA"
                android:text="Cart "
                android:textColor="#FFFFFF"/>

            <!-- Tombol 3 -->
            <Button
                android:id="@+id/button3"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:backgroundTint="#FFB3BA"
                android:text="Order"
                android:textColor="#FFFFFF"/>
        </LinearLayout>
    </HorizontalScrollView>

</androidx.constraintlayout.widget.ConstraintLayout>
