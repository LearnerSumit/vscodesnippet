# How to Use Custom Snippets in VS Code

Follow these steps to create and use a custom snippet in Visual Studio Code:

## Steps

1. **Open VS Code Settings**
   - Open Visual Studio Code.

2. **Open Command Palette**
   - Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac).

3. **Search for Snippets**
   - Type **`Snippets: Configure Snippets`** in the Command Palette and press `Enter`.

4. **Choose `javascriptreact` or `javascript`**
   - Select `javascriptreact.json` if you're working with `.jsx` files.
   - Or select `javascript.json` if you're working with `.js` files.

5. **Paste the Following Code**
   - Add the snippet JSON code to the file:
     ```json
     {
       "React Functional Component": {
         "prefix": "sumit",
         "body": [
           "const ${1:${TM_FILENAME_BASE}} = () => {",
           "  return (",
           "    <div>",
           "      ${2:content}",
           "    </div>",
           "  );",
           "};",
           "",
           "export default ${1:${TM_FILENAME_BASE}};"
         ],
         "description": "Creates a React functional component with the file name as the component name"
       }
     }
     ```

6. **Save the File**
   - Save the file and close it.

7. **Use the Snippet**
   - Open a `.jsx` file (e.g., `MyComponent.jsx`).
   - Type `sumit` and press `Tab` or `Enter`. The snippet will expand automatically, using the file name as the component name.

---

Now you're ready to quickly generate React Functional Components with just a few keystrokes! 🎉
