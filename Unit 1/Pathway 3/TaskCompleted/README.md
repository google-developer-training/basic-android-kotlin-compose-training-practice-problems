# Task Manager - Solution Code

This project contains solution code for Task Manager practice problem. In the exercise, you need to build a screen which displays **All tasks completed** screen. Users see this screen when they complete all the tasks on a given day.

## Solution

1. Download the image from the URL given in practice problem
2. Import the image in the ComposeArticle project
3. Use `Column` composable function to arrange the components vertically:
 
    ```
    Column(
        // Use modifier to set the width and height to max,
        // Set horizontal & vertical alignment parameters to center
    ) {
        // Load image using painterResource()
        Image(...)
        // Load text using stringResource(). Use modifier to set the padding. Set fontWeight to Bold
        Text(...)
        // Load text using stringResource(). Set fontSize to 16.sp
        Text(...)
    }
    ```

## Note:

The solution code uses the basic composables covered in Unit 1, Pathway 3 for Android Basics in Compose:
- [Build a simple app with text composables](https://developer.android.com/codelabs/basic-android-kotlin-compose-text-composables?#0)
- [Add images to your Android app](https://developer.android.com/codelabs/basic-android-kotlin-compose-add-images?#0)

There's a lot of room for improvement, so feel free to experiment and try different things. 
