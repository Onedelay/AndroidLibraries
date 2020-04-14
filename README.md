# Android library version's

gradle 에 추가할 때 귀찮아서 정리하는 안드로이드 라이브러리 버전 리스트

최종 업데이트 : 2020.04.14

<br>

## AndroidX

- [ConstraintLayout](https://developer.android.com/jetpack/androidx/releases/constraintlayout)
  - MotionLayout 은 2.0.0 이상

```groovy
implementation 'androidx.constraintlayout:constraintlayout:1.1.3'
```

- [RecyclerView](https://developer.android.com/jetpack/androidx/releases/recyclerview)

```groovy
implementation "androidx.recyclerview:recyclerview:1.1.0"
```

- [Lifecycle](https://developer.android.com/jetpack/androidx/releases/lifecycle)
  - ViewModelProvider 쓰려면 필요함

```groovy
implementation "androidx.lifecycle:lifecycle-extensions:2.2.0"
```

- [Room](https://developer.android.com/jetpack/androidx/releases/room)

```groovy
implementation "androidx.room:room-runtime:${room_version}"
implementation "androidx.room:room-rxjava2:${room_version}"
implementation "androidx.room:room-coroutines:${room_version}"
kapt "androidx.room:room-compiler:${room_compiler_version}"
```

- [Databinding](https://developer.android.com/jetpack/androidx/releases/databinding)

```groovy
android {
    ...
    dataBinding {
        enabled = true
    }
}
```

- [Compose](https://developer.android.com/jetpack/androidx/releases/compose)

```groovy
dependencies {
    def compose_version = "0.1.0-dev08"

    kotlinPlugin "androidx.compose:compose-compiler:$compose_version"
    implementation "androidx.compose:compose-runtime:$compose_version"
}

composeOptions {
    kotlinCompilerVersion "1.3.61-dev-withExperimentalGoogleExtensions-20200129"
    kotlinCompilerExtensionVersion "0.1.0-dev08"
}
```



<br>

## Design

- Android material

```groovy
implementation 'com.google.android.material:material:1.1.0'
```

- [Lottie](https://github.com/airbnb/lottie-android/releases)

```groovy
implementation "com.airbnb.android:lottie:${lottie_version}"
```



<br>

## Network

- [Retrofit](https://github.com/square/retrofit/blob/master/CHANGELOG.md#change-log)

```groovy
implementation "com.squareup.retrofit2:retrofit:${retrofit_version}"
implementation "com.squareup.retrofit2:converter-gson:${retrofit_version}"
implementation "com.squareup.retrofit2:adapter-rxjava2:${retrofit2_version}"
```

- [Gson](https://github.com/google/gson/blob/master/CHANGELOG.md)

```groovy
implementation "com.google.code.gson:gson:${gson_version}"
```



<br>

## ImageLoader

- [Glide](https://github.com/bumptech/glide/releases)

```groovy
implementation "com.github.bumptech.glide:glide:${glide_version}"
kapt "com.github.bumptech.glide:compiler:${glide_version}"
```



<br>

## Reactive

- [RxJava](https://github.com/ReactiveX/RxJava/releases)

```groovy
implementation "io.reactivex.rxjava2:rxjava:${rxjava_version}"
```

- [RxAndroid](https://github.com/ReactiveX/RxAndroid/releases)

```groovy
implementation "io.reactivex.rxjava2:rxandroid:${rxandroid_version}"
```

- [RxKotlin](https://github.com/ReactiveX/RxKotlin/releases)

```groovy
implementation "io.reactivex.rxjava2:rxkotlin:${rxkotlin_version}"
```

- [RxRelay](https://github.com/JakeWharton/RxRelay/releases)

```groovy
testImplementation "com.jakewharton.rxrelay2:rxrelay:${rxrelay_version}"
```



<br>

## Coroutine

```groovy
implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.3.0'
```



<br>

## Media

- [ExoPlayer](https://github.com/google/ExoPlayer/blob/release-v2/RELEASENOTES.md)

```groovy
implementation "com.google.android.exoplayer:exoplayer:${exo_player_version}"
```



<br>

## DI

- [Dagger2](https://github.com/google/dagger/releases)

```groovy
implementation "com.google.dagger:dagger-android:${dagger_version}"
kapt "com.google.dagger:dagger-compiler:${dagger_version}"
kapt "com.google.dagger:dagger-android-processor:${dagger_version}"
```



<br>

## Debugging

- [Stetho]()

```groovy
implementation "com.facebook.stetho:stetho:${stetho_version}"
implementation "com.facebook.stetho:stetho-okhttp3:${stetho_version}"
```





<br>

## Test

- 
