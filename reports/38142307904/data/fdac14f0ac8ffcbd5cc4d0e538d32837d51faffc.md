# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: src/app/shared-policy/property-priority-helper.test.ts >> priority fields reject transparent and hidden elements through their ancestors
- Location: tests/e2e/src/app/shared-policy/property-priority-helper.test.ts:25:1

# Error details

```
Test timeout of 120000ms exceeded.
```

# Page snapshot

```yaml
- main [ref=e2]:
  - heading "Public task" [level=1] [ref=e3]
  - generic [ref=e4]: Tomorrow 12:30
  - text: Pending
  - generic [ref=e5]: High
```