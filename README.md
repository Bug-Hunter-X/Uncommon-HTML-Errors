# Uncommon HTML Bugs
This repository demonstrates some uncommon errors that can occur in HTML.

The `bug.html` file contains the buggy code.  The `bugSolution.html` file provides the corrected version.

**Bugs demonstrated:**

1. **Accessing a non-existent element:** Attempting to access and modify the `innerHTML` of an element that does not exist on the page. This will result in a runtime error in some cases, or unexpected behavior if it happens inside a conditional that doesn't catch the error. 
2. **Modifying read-only attributes:** Attempting to modify a read-only attribute (like the `readonly` attribute on the body element) using `setAttribute` will likely have no effect and may not trigger an error, but can lead to unexpected behaviors.
3. **Using reserved keywords as IDs:** Using a reserved keyword (such as `class`) as an element's ID can cause parsing errors or unexpected behavior because it conflicts with the keywords the browser uses for styling or internal behavior.  This can cause the script attempting to access that element by its ID to fail silently.