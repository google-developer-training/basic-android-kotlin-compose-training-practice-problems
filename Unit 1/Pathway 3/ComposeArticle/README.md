# Compose Article - Solution Code

This project contains solution code for Compose Article practice problem. In the exercise, you need to build a screen which displays article about Jetpack Compose Tutorial.

## Solution

1. Download the image from the URL given in practice problem
2. Import the image in the ComposeArticle project
3. Use `Column` composable function to arrange the components vertically:
 
    ```
    Column(){
        // Load image using painterResource()
        Image(...)
        // Load text using stringResource()
        Text(...)
        // Load text using stringResource()
        Text(...)
    }
    ```

## Note:

The solution code uses the basic composables covered in Unit 1, Pathway 3 for Android Basics in Compose:
- [Build a simple app with text composables](https://developer.android.com/codelabs/basic-android-kotlin-compose-text-composables#0)
- [Add images to your Android app](https://developer.android.com/codelabs/basic-android-kotlin-compose-add-images#0)

There's a lot of room for improvement, so feel free to experiment and try different things. 
