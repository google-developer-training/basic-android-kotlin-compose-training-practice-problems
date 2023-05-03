# Compose Quadrant - Solution Code
 
This project contains solution code for the Compose Quadrant practice problem. In this exercise,build an app that displays the information about the Composable functions you learned.
 
## New Modifiers/Properties
 
Following is an overview of the Modifiers/Properties which were not covered in the Codelabs but are used to solve the problem.
 
**fontWeight**
 
This parameter in `Text` composable allows you specify how bold or light the text content should appear. `FontWeight.Bold` is used to set the font style to bold
 
**textAlign**
 
This parameter in `Text` composable defines how to align the text horizontally.  The `TextAlign.Justify` property stretches the lines of text that end with soft line break to fill the width of the container.
 
**Modifier.weight**

This modifier is scoped to Row composable. The modifier allows the size of the element's width proportional to its `weight` and relative to other weighted sibling elements. The parent will divide the horizontal space remaining after measuring unweighted child elements and distribute it according to this weight.
 
## Solution
 
Following is the overview of steps used in the solution
1. For a single quadrant, create a `ComposableInforCard`
 
   ```
   // Setup background, padding and size modifiers. Also, set the alignment to center - vertically as well
   // as horizontally
   Column(...) {
       // Title text
       Text(...)
       // Description text
       Text(...)
   }
   ```
2. Create a `Row` composable, to align two cards horizontally. Set the weight to `1f` so that the space is distributed equally.
 
   ```
   Row(Modifier.weight(1f)){
       // Quadrant to be displayed on first half of the screen
       ComposableInforCard(...)
       // Quadrant to be displayed on second half of the screen
       ComposableInforCard(...)
   }
   ```
3. Create another `Row` composable, with same structure as above, to display the remaining two quadrants
4. Wrap both the `Row` composables in a `Column` composable to align them vertically.
 
   ```
   Column(...){
       // First row, which displays info on Text and Image composable functions
       Row(Modifier.weight(1f)) {
           ...
       }
       // Second row, which displays info on Row and Column composable functions
       Row(Modifier.weight(1f)) {
           ...
       }
   }
   ```
 
## Note:
 
The solution code uses the basic composables covered in Unit 1, Pathway 3 for Android Basics in Compose:
- [Build a simple app with text composables](https://developer.android.com/codelabs/basic-android-kotlin-compose-text-composables#0)
- [Add images to your Android app](https://developer.android.com/codelabs/basic-android-kotlin-compose-add-images#0)
 
There's a lot of room for improvement, so feel free to experiment and try different things.
 

