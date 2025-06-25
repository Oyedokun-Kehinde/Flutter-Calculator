````markdown
# 📱 Flutter Calculator App

A lightweight, minimal, and elegant calculator app built using **Flutter** and powered by the **math_expressions** package to parse and evaluate mathematical expressions.

This app demonstrates stateful widget usage, grid-based button UI, and dynamic string evaluation for real-time math computation — a great starter project for beginners learning Flutter.

---

## 🚀 Demo

<img src="https://user-images.githubusercontent.com/yourimage.png" alt="Flutter Calculator Screenshot" width="280"/>

---

## 🛠 Features

- Simple calculator UI with digits and basic operators
- Real-time expression rendering
- Support for basic arithmetic: `+`, `-`, `×`, `÷`
- Uses the `math_expressions` package for safe, structured parsing
- Responsive design using GridView
- Clean and modular code with reusable widgets
- Error handling for invalid expressions

---

## 🧱 Tech Stack

| Technology      | Purpose                            |
|----------------|-------------------------------------|
| `Flutter`       | UI Framework                        |
| `Dart`          | Programming Language                |
| `math_expressions` | Expression parsing and evaluation |

---

## 📦 Dependencies

Add this to your `pubspec.yaml`:

```yaml
dependencies:
  flutter:
    sdk: flutter
  math_expressions: ^2.2.0
````

---

## 📂 Project Structure

```
lib/
├── main.dart          # Entry point
└── calculator_screen  # UI logic and calculator layout
```

---

## 💡 How It Works

* The app uses a `StatefulWidget` to track the calculator's current expression.
* Taps on each button update the `_expression` string using `setState`.
* When the `=` button is pressed:

  * The string is parsed using the `Parser()` from `math_expressions`.
  * Evaluated via a `ContextModel()`.
  * The result is rendered back to the screen.
* Button layout is handled using `GridView.builder`, allowing for a responsive keypad interface.

---

## 🧪 Example Usage

```dart
// Tapping '7', '+', '3', '=' will:
_expression = '7+3';
// Result:
_expression = '10.0';
```

---

## ✨ UI Preview

| Expression Entry | Evaluation       | Clear Button   |
| ---------------- | ---------------- | -------------- |
| ✅ Live rendered  | ✅ Instant result | ✅ Clears state |

---

## 📌 Buttons Defined

The buttons array holds all UI keys in a flat list, structured in 4x4 grid:

```dart
final List<String> buttons = [
  '7', '8', '9', '/',
  '4', '5', '6', '*',
  '1', '2', '3', '-',
  'C', '0', '=', '+',
];
```

---

## 🎯 To Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/your-username/flutter-calculator.git
cd flutter-calculator

# 2. Install dependencies
flutter pub get

# 3. Run on emulator or device
flutter run
```

---

## 🔧 To-Do & Extensions

* [ ] Add percentage (%) and decimal point support
* [ ] Add brackets `()`, `mod`, and power `^`
* [ ] Switch to `CustomPainter` for UI styling
* [ ] Theme toggling (Dark Mode / Light Mode)
* [ ] Persist history using local storage

---

## ❤️ Best For:

* Beginners learning `StatefulWidgets`
* Practicing Flutter layouts with `GridView`
* Understanding runtime expression evaluation

---

## 🧠 Author’s Notes

> “A simple calculator app is one of the best ways to learn event handling, state management, and UI layout in Flutter. It’s not just about math — it’s about mastering input + state + logic = app.”

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 📬 Contact

Built by [Your Name](https://github.com/Oyedokun-Kehinde)
For suggestions, open issues or pull requests 🤝

---

