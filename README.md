# wolf
This code is a Python script that utilizes the `turtle` module to draw shapes based on coordinates and colors extracted from a Microsoft Word document.

## Requirements
- Python 3.x
- turtle module
- re module
- docx module

## Installation
1. Make sure you have Python 3.x installed on your system.
2. Install the required modules by running the following command:
   ```
   pip install turtle docx
   ```

## Usage
1. Replace the value of the `source` variable with the name of the Word document (without the file extension) that you want to extract coordinates and colors from. Place the Word document in the same directory as the script.
2. Run the script using the following command:
   ```
   python script.py
   ```
3. The script will read the Word document and extract coordinate and color data from it.
4. A turtle graphics window will open, and the script will draw shapes based on the extracted data.

## How it works
1. The script imports the necessary modules: `turtle`, `re` (regular expressions), and `docx` (for working with Word documents).
2. It initializes some variables including the `source` which specifies the name of the Word document.
3. The script opens the Word document using the `docx` module and reads its paragraphs.
4. For each paragraph, it uses regular expressions to extract coordinate tuples and color tuples from the text.
5. The extracted data is stored in the `coordinates` and `colour` lists.
6. The script creates a turtle object and a turtle screen.
7. Various settings are configured for the turtle graphics, such as speed, hiding the turtle, and setting the screen to fullscreen mode.
8. The script iterates over the extracted coordinates and colors, and for each set, it sets the pen color and begins filling.
9. It then iterates over the coordinate pairs and draws lines between them to form shapes.
10. Finally, it ends the fill, hides the turtle, and starts the turtle screen main loop to display the drawn shapes.

Note: The script ignores any paragraphs in the Word document that do not match the expected coordinate and color patterns.

Feel free to customize the code according to your needs or incorporate it into a larger project. Happy drawing!
