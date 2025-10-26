# Valentino Magic Beans – Production E2E Testing 🚀

![Node.js](https://img.shields.io/badge/Node.js-18+-green)
![Playwright](https://img.shields.io/badge/Playwright-Test-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

This project is a **complete end-to-end testing suite** for an e-commerce application. It covers the full user journey, including authentication, product catalog interactions, checkout, and API integrations, showcasing my skills in Playwright automation and test organization.

---

## 🗂 Project Overview

### Features
- **User authentication** with email verification  
- **Product catalog** browsing and shopping cart functionality  
- **Complete checkout** process including payment  
- **Order tracking** and contact forms  
- **API request interception and mocking**  

### Key Test Files
- `auth-flow.spec.ts` – User registration with email verification  
- `product-flow.spec.ts` – Complete purchase workflow  
- `EmailUtils.ts` – Email testing using MailSlurp integration  
- **Page Objects** – Modular and reusable test design  

---

## ⚡ Getting Started

### Prerequisites
- Node.js 18+ (22+ recommended)  
- npm or yarn  

### Setup & Running Tests

```bash
# Navigate to project folder
cd valentino-magic-beans

# Install dependencies
npm install

# (Optional) Set MailSlurp API key for email tests
export MAIL_SLURP_API_KEY="your_api_key_here"

# Run all tests
npx playwright test

# Run tests in a specific browser (Chromium)
npx playwright test --project=chromium

# Run specific test files
npx playwright test auth-flow.spec.ts
npx playwright test product-flow.spec.ts

# Run authentication flow with account creation
SIGN_UP_FLOW=true npx playwright test auth-flow.spec.ts

# Run tests with browser visible
npx playwright test --headed

# Debug mode (interactive)
npx playwright test --debug

# Generate HTML report
npx playwright test --reporter=html

# Open the HTML report
npx playwright show-report
```

## 🛠 Testing Practices Demonstrated

- **Locators & Actions:** Form filling, clicks, selections, keyboard/mouse events  
- **API Interception & Mocking:** Validate server interactions and test scenarios  
- **Email Verification:** Automated email flow testing with MailSlurp  
- **Page Object Model:** Modular, reusable, and maintainable test structure  
- **Advanced Features:** Parallel execution, fixtures/hooks, parameterized tests  

---

## 🤝 Contributing

- Follow existing Page Object structure  
- Add appropriate test tags for filtering  
- Include both positive and negative test cases  
- Document any new external dependencies  

---

## 📞 References

- [Playwright Documentation](https://playwright.dev/)  
- Use `--headed` or `--debug` for troubleshooting
