<picture>
  <source media="(prefers-color-scheme: dark)" srcset="faultwise-logo-dark.png">
  <img src="faultwise-logo.png" alt="Faultwise" width="320">
</picture>

**When a test fails, is the app wrong, or the test?**

Faultwise reads your test results, looks at each failure together with the test and your application code, and tells you what's at fault:

- **App bug:** severity, root cause, the evidence, and a suggested code fix
- **Broken test:** what's wrong with the test, and a corrected version (for Playwright, a repaired copy you review before using)
- **Environment problem:** when neither the app nor the test is to blame

### Why teams use it

- **Any test framework.** It reads Playwright JSON and JUnit XML, which almost every framework writes: web (Playwright, Cypress, WebdriverIO, Selenium), mobile (Appium, Espresso, XCUITest), desktop (NUnit or xUnit runners) and server tests (pytest, JUnit, TestNG, Jest, Go, .NET).
- **Any AI, including a local model.** Use Claude, any OpenAI-compatible service, or a local model through Ollama, so your code never has to leave the company.
- **Runs where you already work.** A command-line tool and a GitHub Action that puts the report on the run's Summary page.
- **Measured, not just claimed.** Every setup starts by checking Faultwise's verdicts against your own team's, so you know how accurate it is on your failures before you rely on it.

### See it work

The public demo, [**AI QA Lab**](https://github.com/adidaGross/ai-qa-lab), uses Faultwise on a shop with planted bugs and broken tests ([live site](https://adidagross.github.io/ai-qa-lab/)):

- 23 of 23 failures classified correctly, and 8 of 8 broken tests repaired and passing
- 37 tests across UI, API, 2FA and passkey sign-in, security and load
- A mutation benchmark of Claude Opus, Sonnet and Haiku on generated bugs: with the application code, Opus and Sonnet classified all 115 hard failures correctly

### Modules

| Module | Status |
|---|---|
| **Faultwise Triage**: app bug or broken test, with evidence and a fix | Available |
| **Faultwise Heal**: repaired copies of broken tests | Available for Playwright |
| **Faultwise Bench**: accuracy measured on known faults | In the demo |
| Flaky tests, CI and deployment failures, incidents | Planned |

### Getting Faultwise

Faultwise is offered as a **self-hosted license with support**: it runs in your own CI, with your own AI key or local model. Pricing is per company, on request.

To try it on your project, [contact me on LinkedIn](https://www.linkedin.com/in/adi-gorsky-6319bb14b/).
