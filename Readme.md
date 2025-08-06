# PyCalc Web

**PyCalc Web** is a simple Python-powered calculator that runs **directly in the browser** using [Pyodide](https://pyodide.org/).  
You can enter any Python expression, and it will evaluate it live — no backend or server needed, just Python and WebAssembly.

## Features
- Evaluate full Python expressions right in the browser.
- No installation required; runs offline after the first load.
- Supports Python operators (`+`, `-`, `*`, `/`, `**`, `//`, `%`).
- Friendly error handling.
- Lightweight and easy to use.
- Imports the `math` module so users can use functions like `math.sin()`, `math.pow()`, `math.sqrt()`, etc.
- Replaces `<input>` with `<textarea>` so users can write full Python code (e.g., defining variables).
- Better error formatting.

## How to run locally
1. Clone or download this repository.  
2. Open `calculator.html` in a modern browser (Chrome, Firefox, Edge).  
3. Wait a moment for Pyodide to load (a message will appear).  
4. Enter your Python expression and click **Evaluate**.  
5. See the result instantly!

## How it works
- The page loads the Pyodide WebAssembly runtime via CDN.  
- User input is taken from a text area.  
- The input string is executed as a Python expression using `pyodide.runPythonAsync()`.  
- Results or errors are displayed dynamically on the page.

## Ideas for Future Enhancements
- Support multi-line Python code with better indentation support.  
- Add imports for useful modules like `math` for advanced math functions.  
- Implement a history feature for previous calculations.  
- Integrate plotting libraries (e.g., `matplotlib`) to visualize math functions.  
- Add dark mode and improve UI styling.

## Resources
- [Pyodide Documentation](https://pyodide.org/en/stable/)  
- [Python Official Docs](https://docs.python.org/3/)  
- [WebAssembly Overview](https://webassembly.org/)

## Contributing
Feel free to fork, submit issues, or send pull requests! Let's make Python in the browser more powerful together.

## License
This project is open source under the MIT License. See the `LICENSE` file for details.

© 2025 Rituja Dikshit
