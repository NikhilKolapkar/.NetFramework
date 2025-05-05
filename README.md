
# Selenium C# .Net Automation Framework (.Net | C# | NUnit | POM)

This is a robust, scalable Selenium WebDriver automation framework built in C# using the Page Object Model (POM) design pattern and NUnit test framework. It supports local and remote execution (e.g., BrowserStack), multiple browsers (Chrome, Firefox, IE), and parallel test execution with reporting.

---

## 🔧 Tech Stack

- **Language**: C#
- **Framework**: NUnit
- **Design Pattern**: Page Object Model (POM)
- **Browsers Supported**: Chrome, Firefox, Internet Explorer
- **Execution**: Local & Remote (e.g., BrowserStack)
- **Reporting**: ExtentReports
- **Test Data**: XML & Constants

---

## 📁 Project Structure

```
NUnitAutomationFramework/
├── Pages/                  # Page Object Model classes
├── TestSuites/             # Test classes (e.g., Regression.cs)
├── Resources/              # Test data files (Testdata.xml, Environment.json)
├── Reports/                # Test execution reports (index.html)
├── app.config              # Browser & environment configuration
└── NUnitFramework.sln      # Solution file
```

---

## 🚀 Getting Started

### Prerequisites

- Windows OS
- Visual Studio
- .NET SDK

### Setup Instructions

1. Clone this repo to your local machine.
2. Open `NUnitFramework.sln` in Visual Studio.
3. Update `app.config` with:
   - `Browser`: chrome | firefox | IE
   - `Environment`: QA | UAT | PROD
   - `RunEnvironment`: Local | Remote

4. Add environment URLs in `Resources/Environment.json`.

---

## 🧪 Writing Test Cases

1. Create your test methods inside `TestSuites/Regression.cs`.
2. Use `Pages/HomePage.cs` to interact with UI elements (follows POM).
3. Pass test data via:
   - Constant variables
   - `Resources/Testdata.xml`

---

## ▶️ Running Tests

**Using Visual Studio:**

- Build the solution.
- Open **Test Explorer** → Run selected tests.

**Using CLI:**

```bash
cd NUnitFramework
dotnet test NUnitFramework.csproj
```

Tests will execute in parallel as per the config.

---

## 📊 Reporting

After execution, open:

```
Reports/index.html
```

...in any browser to view the test execution report (ExtentReports).

---

## 📌 Highlights

- ✅ Page Object Model for clean, maintainable code
- ✅ Supports test data-driven testing
- ✅ Parallel execution for faster runs
- ✅ Easy environment switching
- ✅ Ready for CI/CD integration

---

