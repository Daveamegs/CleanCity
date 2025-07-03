# CLEANCITY - WASTE PICKUP SCHEDULER

## TEST PLAN

**Project Name:** CleanCity - A Waste Pickup Scheduler
**Prepared By:** Alpha Testers
**Date:** July 2, 2025
**Version:** 1.0

### Introduction

CleanCity is a React-based web application that simulates a waste collection system. It is designed for QA students to perform manual and automated testing with built-in flaws.

### Test Objectives

- Verify all forms work correctly, including validation and error messaging.
- Confirm data is correctly filtered and displayed on the dashboard.
- Ensure accessibility standards are met (e.g., alt-text).
- Check admin features like status updates and data persistence.
- Validate all key user workflows across core modules.
- Uncover functional and non-functional issues through exploratory testing.
- Evaluate the system’s performance, security, and cross-browser compatib

### Scope of Testing

#### In-Scope:

- Functional workflows across all modules
- Static code analysis using browser dev tools, linters or SonarQube setup
- Performance under user load using simulated data
- Security (basic auth flaws, XSS test attempts)
- Compatibility across Chrome, Firefox, and mobile browsers
- Accessibility checks on Awareness page
- Admin status updates and UI refresh

#### Out of Scope:

- Backend API Infrastructure and performance (No Backend)
- Mobile app version (Not Included)

### Test Types

- Functional Testing
- Exploratory Testing
- Static Code Analysis
- Performance Testing
- Security Testing
- UI/UX Testing
- Accessibility Testing
- Compaatibility Testing
- Boundary and Negative Value Testing

### Core Modules to Be Tested

- Authentication System
  - Login, Logout, Session checks
- Waste Management
  - Request form, scheduling, missed pickups
- Dashboard & Analytics
  - Filtering, status badges, city-based segmentation
- Content Management
  - Awareness page, text/image assets, accessibility
- Community Features
  - Feedback forms, missed pickups reporting
- Administrative Functions
  - Marking requests as completed, status updates

### Test Deliverables

- Test Plan
- Test Scenarios & Test Cases
- Bug Reports
- Test Summary Report

### Test Schedule

Test Planning and Design
Manual/Exploration Test Execution
Security and Performance Testing
Compatibility Tests
Automated Test Development
Summary and Reporting

### Resources

- 3 QA Students
- Test environment with localStorage and test data
- Live website link

### Risks

- React components might be too dynamic for basic locators
- Mock data may reset unexpectedly, affecting consistency

### Exit Criteria

- All test notes compiled and reviewed
  - Accessibility issues identified and documented
  - All high-priority bugs fixed
  - Test summary reviewed and approved
- 98% test coverage

## TEST STRATEGY

### Scope

This strategy defines the testing approach for the CleanCity project. It applies to all front-end components and UI workflows of the web application.

### Testing Approach

#### Manual Testing

- **Exploratory Testing:** Unscripted scenario-based interaction to discover flaws.
- **Static Analysis:** Reviewing HTML/CSS structure, broken tags, missing semantics.
- **Accessibility Checks:** Using Lighthouse and screen readers.
- **Performance Testing:** Simulate user load, analyze loading speed, form responsiveness.
- **Security Testing:** Attempt basic XSS, CSRF, and auth bypass checks using browser tools.
- **Compatibility Testing:** Chrome, Firefox, Edge, mobile (responsive behavior).
- **UI/UX:** UI consistency across pages

#### Automated Testing

- **Use Cypress or Playwright for:**

  - Smoke tests on core pages
  - Form submission and validation
  - Integration Testing

### Test Levels

- **Unit Testing:** Perform using jest or pytest
- **Integration Testings:** Perform on all the core modules
- **System Testing:** End-to-end flows including admin interactions
- **User Acceptance Testing (UAT):** Manual UAT by QA students

### Test Environments

#### Browsers

- Chrome
- Firefox
- Edge
- Safari

#### Device

- Mobile
- Desktop
- Tablet

### Test Tools

- **Manual Testing:** TestRail
- **Automation Testing:** Cypress, Playwright
- **Bug Tracking:** Jira, GitHub Issues
- **Accessibility Testing:** Axe DevTools, Chrome Lighthouse

### Roles and Responsibilities

--------------------------------------------------------------------------------------------
| Role                 |               Responsibility                                      |
|----------------------|-------------------------------------------------------------------|
| Manual Testers       | Execute manual test cases, report bugs                            |
| Automation Testers   | Write and run automated scripts                                   |
|                      |                                                                   |
|__________________________________________________________________________________________|

### Defect Management

- Bugs reported on Jira
- Severity Levels: Critical, High, Medium, Low

### Test Data Management

- Use provided test data for form inputs
- Reset localStorage as part of setup/teardown scripts

### Exit Criteria

- All planned test cases explored and executed
  - All core workflows explored
  - Major browser/device compatibility flaws documented
  - All intentional flaws documented

## Team Members (QA Students)

- David K. Amegayibor
- Duncan Osano
- Giresse Mujeque
