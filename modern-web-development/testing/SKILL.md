---
name: web-application-testing
description: Expert knowledge in testing web applications across all levels, from unit tests to end-to-end testing. Covers unit testing, integration testing, E2E testing, Test-Driven Development (TDD), test coverage, mocking and stubbing, performance testing, and visual regression testing. Use when writing tests or implementing testing strategies.
metadata:
  version: 1.0.0
---

# Web Application Testing Skill

Expert knowledge in testing web applications across all levels, from unit tests to end-to-end testing.

## Core Competencies

- **Unit Testing**: Testing individual functions and components
- **Integration Testing**: Testing component interactions
- **End-to-End Testing**: Testing complete user workflows
- **Test-Driven Development (TDD)**: Writing tests before implementation
- **Test Coverage**: Ensuring adequate code coverage
- **Mocking and Stubbing**: Isolating code under test
- **Performance Testing**: Testing application performance
- **Visual Regression Testing**: Detecting visual changes

## Testing Pyramid

```
        /\
       /E2E\         Few, slow, expensive
      /------\
     /Integration\   Some, moderate speed
    /------------\
   /  Unit Tests  \  Many, fast, cheap
  /________________\
```

## Unit Testing

**Tools**: Jest, Vitest, Mocha, Jasmine

**Best Practices**:
- Test one thing at a time
- Use descriptive test names
- Follow AAA pattern (Arrange, Act, Assert)
- Keep tests independent
- Mock external dependencies
- Aim for 80%+ coverage for critical code

**Example Test Structure**:
```javascript
describe('Component/Function Name', () => {
  it('should behave in specific way when condition', () => {
    // Arrange
    const input = setupInput();
    
    // Act
    const result = functionUnderTest(input);
    
    // Assert
    expect(result).toBe(expectedValue);
  });
});
```

## Component Testing

**Tools**: React Testing Library, Vue Testing Library, Testing Library family

**Best Practices**:
- Test behavior, not implementation
- Query by accessibility attributes (role, label)
- Avoid testing internal state
- Simulate user interactions
- Test error states and edge cases

**What to Test**:
- Component renders correctly
- Props affect output correctly
- User interactions work as expected
- Conditional rendering works
- Error handling works

## Integration Testing

**Tools**: Jest, Testing Library, Playwright Component Testing

**Focus Areas**:
- Component interactions
- State management
- API integration
- Routing
- Form submissions
- Data flow

## End-to-End Testing

**Tools**: Playwright, Cypress, Puppeteer, Selenium

**Best Practices**:
- Test critical user journeys
- Keep tests independent
- Use stable selectors (data-testid)
- Handle async operations properly
- Take screenshots on failure
- Run against staging environment

**Common Scenarios**:
- User registration and login
- Shopping cart checkout
- Form submissions
- Search functionality
- Navigation flows

## Test-Driven Development (TDD)

**Process**:
1. Write a failing test
2. Write minimal code to pass
3. Refactor while keeping tests green
4. Repeat

**Benefits**:
- Better code design
- Higher confidence
- Built-in documentation
- Fewer bugs

## Mocking and Stubbing

**When to Mock**:
- External APIs
- Database calls
- File system operations
- Date/time functions
- Random number generators

**Tools**:
- Jest mock functions
- MSW (Mock Service Worker) for API mocking
- Sinon for spies, stubs, mocks

## Accessibility Testing

**Tools**: jest-axe, axe-core, Pa11y

**What to Test**:
- Keyboard navigation
- Screen reader compatibility
- Color contrast
- ARIA attributes
- Focus management

## Performance Testing

**Tools**: Lighthouse CI, WebPageTest, k6

**Metrics to Test**:
- Load time
- Time to Interactive
- Core Web Vitals
- Bundle size
- API response times

## Visual Regression Testing

**Tools**: Percy, Chromatic, BackstopJS, Playwright visual comparisons

**Use Cases**:
- Detecting unintended UI changes
- Cross-browser compatibility
- Responsive design validation

## Testing Best Practices

1. **Test Naming**
   - Use descriptive names
   - Include what's being tested and expected behavior
   - Use "should" or "it" format

2. **Test Organization**
   - Group related tests
   - Use setup and teardown appropriately
   - Keep tests close to source code

3. **Assertions**
   - Use specific assertions
   - One logical assertion per test
   - Use meaningful error messages

4. **Test Data**
   - Use realistic test data
   - Create test data factories
   - Clean up test data after tests

5. **Flaky Tests**
   - Avoid time-dependent tests
   - Handle async operations properly
   - Ensure proper test isolation
   - Don't rely on test execution order

6. **CI Integration**
   - Run tests on every commit
   - Fail builds on test failures
   - Track test coverage over time
   - Run different test suites appropriately

## Coverage Guidelines

- **Critical paths**: 90-100%
- **Business logic**: 80-90%
- **UI components**: 70-80%
- **E2E tests**: Cover main user journeys

## Common Pitfalls

- Testing implementation details
- Not testing edge cases
- Over-mocking (making tests brittle)
- Slow test suites
- Flaky tests
- Low coverage of critical code
- Tests that don't fail when they should
