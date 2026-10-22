Step 1: The Buggy HTML Code (Before)
Save this intentionally broken code as buggy.html to see the errors in action:

HTML
<html>
<head>
    <title>My Buggy Page
</head>
<body>
    <p><h1>Welcome to my site</h1></p>
    <img src="image.jpg">
    <div>
        <p>This is a paragraph that was never closed properly.
    </div>
</body>
</html>
Step 2: Identifying the Errors
When you open buggy.html in a browser or validator, you will spot several errors:

Missing <!DOCTYPE html>: The document type declaration is missing, causing browsers to enter quirks mode.

Missing closing </title> tag: The title tag is left unclosed.

Incorrect Nesting: A block-level heading (<h1>) is incorrectly placed inside an inline paragraph (<p>).

Missing attribute: The <img> tag is missing the required alt attribute.

Missing closing paragraph tag: The <p> tag inside the <div> is missing </p>.

Step 3: The Fixed HTML Code (After)
Save your corrected version as index.html (or fixed.html) with proper indentation and all errors resolved:

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Fixed Page</title>
</head>
<body>

    <!-- Correct nesting: Heading is separate from the paragraph -->
    <h1>Welcome to my site</h1>

    <!-- Added missing alt attribute for accessibility -->
    <img src="image.jpg" alt="A placeholder description of the image">

    <div>
        <!-- Added missing closing paragraph tag -->
        <p>This is a paragraph that is now closed properly.</p>
    </div>

</body>
</html>
Step 4: Inspecting with Browser DevTools & Validators
To fulfill the debugging steps required by your assignment:

DevTools: Right-click your fixed webpage in Chrome, Edge, or Firefox, and select Inspect (or press F12). Look at the Elements panel to verify that the DOM tree is clean, properly nested, and error-free.

W3C Validator: Go to the W3C Markup Validation Service, upload your fixed HTML file (or paste the code), and check that it passes with 0 errors or warnings.

Submission Requirements Checklist
Before Code: Include your snippet of the buggy code.

After Code: Include your snippet of the clean, fixed code.

Screenshot: Take a screenshot of the fixed webpage running in your browser and submit it along with your code files.