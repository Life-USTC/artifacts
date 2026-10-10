# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: src/app/young-events/public-browse-contract.test.ts >> young-event.web-browse-context
- Location: tests/e2e/src/app/young-events/public-browse-contract.test.ts:37:1

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('a[href^="/catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-00?"]:visible').first()
Expected: visible
Timeout: 5000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 5000ms
  - waiting for locator('a[href^="/catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-00?"]:visible').first()

```

```yaml
- link "Skip to main content":
  - /url: "#main-content"
- navigation "Second Classroom":
  - list:
    - listitem:
      - link "Back to Home":
        - /url: /
  - button "Second Classroom" [expanded]
  - list:
    - listitem:
      - link "Activity list":
        - /url: /catalog/young-events
    - listitem:
      - link "Event calendar":
        - /url: /catalog/young-events/calendar
    - listitem:
      - link "Organizers":
        - /url: /catalog/young-events/organizers
- button "Toggle Sidebar"
- main:
  - button "Open search": Search sections, teachers, courses… Ctrl K
  - button "Language selector"
  - button "Theme selector"
  - link "Sign In":
    - /url: /account/sign-in
  - region "Main content scroll region":
    - heading "Second Classroom" [level=1]
    - paragraph:
      - text: Signup events from the
      - link "USTC second classroom platform":
        - /url: https://young.ustc.edu.cn
      - text: .
    - text: Search
    - group:
      - group
      - searchbox "Search": young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event
      - group: Ctrl Shift K
    - group:
      - text: Activity scope
      - combobox "Activity scope":
        - option "All events"
        - option "Current signup list" [selected]
        - option "Historical activity list"
    - button "Search"
    - button "More filters (4)": More filters 4
    - group "Applied filters":
      - link "Remove young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event filter":
        - /url: /catalog/young-events?category=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category&module=%E6%99%BA&activityLevel=%E6%A0%A1%E7%BA%A7&organizerId=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-org-00&active=true&timeBasis=activity
        - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event
      - link "Remove Current signup list filter":
        - /url: /catalog/young-events?search=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694+Event&category=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category&module=%E6%99%BA&activityLevel=%E6%A0%A1%E7%BA%A7&organizerId=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-org-00&timeBasis=activity
        - text: Current signup list
      - link "Remove young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-org-00 filter":
        - /url: /catalog/young-events?search=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694+Event&category=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category&module=%E6%99%BA&activityLevel=%E6%A0%A1%E7%BA%A7&active=true&timeBasis=activity
        - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-org-00
      - link "Remove young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category filter":
        - /url: /catalog/young-events?search=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694+Event&module=%E6%99%BA&activityLevel=%E6%A0%A1%E7%BA%A7&organizerId=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-org-00&active=true&timeBasis=activity
        - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category
      - link "Remove 智 filter":
        - /url: /catalog/young-events?search=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694+Event&category=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category&activityLevel=%E6%A0%A1%E7%BA%A7&organizerId=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-org-00&active=true&timeBasis=activity
        - text: 智
      - link "Remove 校级 filter":
        - /url: /catalog/young-events?search=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694+Event&category=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category&module=%E6%99%BA&organizerId=young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-org-00&active=true&timeBasis=activity
        - text: 校级
      - link "Clear":
        - /url: /catalog/young-events
    - paragraph: Showing 9 of 9 events
    - text: 1 / 1
    - table:
      - rowgroup:
        - row "Event Event time Location Capacity Status":
          - columnheader "Event"
          - columnheader "Event time"
          - columnheader "Location"
          - columnheader "Capacity"
          - columnheader "Status"
      - rowgroup:
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 10 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-15 23:59 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 10 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 10":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-10
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-15 23:59"
          - cell
          - cell
          - cell "Current signup list"
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 00 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-15 10:00 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 00 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 00":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-00
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-15 10:00"
          - cell
          - cell
          - cell "Current signup list"
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 01 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-15 10:00 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 01 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 01":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-01
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-15 10:00"
          - cell
          - cell
          - cell "Current signup list"
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 02 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-15 10:00 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 02 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 02":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-02
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-15 10:00"
          - cell
          - cell
          - cell "Current signup list"
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 03 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-15 10:00 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 03 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 03":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-03
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-15 10:00"
          - cell
          - cell
          - cell "Current signup list"
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 04 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-15 10:00 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 04 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 04":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-04
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-15 10:00"
          - cell
          - cell
          - cell "Current signup list"
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 05 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-15 10:00 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 05 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 05":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-05
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-15 10:00"
          - cell
          - cell
          - cell "Current signup list"
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 08 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-14 10:00 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 08 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 08":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-08
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-14 10:00"
          - cell
          - cell
          - cell "Current signup list"
        - row "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 12 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie 2035-09-14 10:00 Current signup list":
          - cell "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 12 young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie":
            - link "young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 Event 12":
              - /url: /catalog/young-events/young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-event-12
            - text: young-browse-135176f1-b53a-49ed-ab62-b417c55a3694-category 智 校级 Z young-browse-135176f1-b53a-49ed-ab62-b417c55a3694 tie
          - cell "2035-09-14 10:00"
          - cell
          - cell
          - cell "Current signup list"
    - paragraph: Source freshness is unknown
- contentinfo:
  - navigation "Footer navigation":
    - link "Terms of Service":
      - /url: /terms
    - link "Privacy Policy":
      - /url: /privacy
    - link "GitHub":
      - /url: https://github.com/Life-USTC/server
    - link "Mobile App":
      - /url: /usage/mobile
  - paragraph: Life@USTC
- region "Notifications alt+T"
```

# Test source

```ts
  1   | import { expect, type Page, test } from "@playwright/test";
  2   | import {
  3   |   cleanupYoungBrowseFixture,
  4   |   createYoungBrowseFixture,
  5   |   type YoungBrowseFixture,
  6   | } from "../../../../shared/young-browse-fixture";
  7   | import { withE2ePrisma } from "../../../utils/e2e-db/prisma";
  8   | import { gotoAndWaitForReady } from "../../../utils/page-ready";
  9   | 
  10  | let fixture: YoungBrowseFixture;
  11  | const root = "/catalog/young-events";
  12  | test.beforeEach(async () => {
  13  |   fixture = await withE2ePrisma(createYoungBrowseFixture);
  14  | });
  15  | test.afterEach(async () => {
  16  |   await withE2ePrisma((db) => cleanupYoungBrowseFixture(db, fixture));
  17  | });
  18  | function eventLink(page: Page, index: number) {
  19  |   return page
  20  |     .locator(`a[href^="${root}/${fixture.eventIds[index]}?"]:visible`)
  21  |     .first();
  22  | }
  23  | async function openYoungSidebar(page: Page) {
  24  |   const sidebar = page.getByTestId("young-sidebar");
  25  |   if (!(await sidebar.isVisible())) {
  26  |     await page.locator('[data-slot="sidebar-trigger"]').click();
  27  |   }
  28  |   await expect(sidebar).toBeVisible();
  29  |   return sidebar;
  30  | }
  31  | function sharedContext(page: Page, expected: Record<string, string>) {
  32  |   expect(Object.fromEntries(new URL(page.url()).searchParams)).toMatchObject(
  33  |     expected,
  34  |   );
  35  | }
  36  | 
  37  | test("young-event.web-browse-context", async ({ page }) => {
  38  |   for (const width of [1280, 390]) {
  39  |     await page.setViewportSize({ width, height: 844 });
  40  |     const filters = {
  41  |       search: fixture.search,
  42  |       category: fixture.category,
  43  |       module: "智",
  44  |       activityLevel: "校级",
  45  |       organizerId: fixture.organizerIds[0],
  46  |       active: "true",
  47  |       timeBasis: "activity",
  48  |     };
  49  |     await gotoAndWaitForReady(page, `${root}?${new URLSearchParams(filters)}`);
  50  |     sharedContext(page, filters);
  51  |     await expect(
  52  |       page.locator("#main-content").getByRole("searchbox"),
  53  |     ).toBeVisible();
> 54  |     await expect(eventLink(page, 0)).toBeVisible();
      |                                      ^ Error: expect(locator).toBeVisible() failed
  55  |     const sidebar = await openYoungSidebar(page);
  56  |     await sidebar
  57  |       .getByRole("link", { name: /^(活动日历|Event calendar)$/ })
  58  |       .click();
  59  |     await expect(page).toHaveURL(/\/catalog\/young-events\/calendar$/);
  60  |     await expect(
  61  |       page.locator("#main-content").getByRole("searchbox"),
  62  |     ).toHaveCount(0);
  63  |     await expect(
  64  |       page.getByRole("button", { name: /更多筛选|More filters/ }),
  65  |     ).toHaveCount(0);
  66  |     const listNav = await openYoungSidebar(page);
  67  |     await listNav
  68  |       .getByRole("link", { name: /^(活动列表|Activity list)$/ })
  69  |       .click();
  70  |     await expect(page).toHaveURL(/\/catalog\/young-events$/);
  71  |     for (const timeBasis of ["activity", "registration"]) {
  72  |       await gotoAndWaitForReady(
  73  |         page,
  74  |         `${root}?${new URLSearchParams({ search: fixture.search, dateUnknown: "true", timeBasis })}`,
  75  |       );
  76  |       const applied = page.getByRole("group", {
  77  |         name: /已选条件|Applied filters/,
  78  |       });
  79  |       await expect(applied).toContainText(
  80  |         timeBasis === "activity"
  81  |           ? /活动时间未知|Unknown activity date/
  82  |           : /报名时间未知|Unknown signup date/,
  83  |       );
  84  |       await expect(
  85  |         eventLink(page, timeBasis === "activity" ? 7 : 10),
  86  |       ).toBeVisible();
  87  |       await page.getByRole("button", { name: /^(搜索|Search)$/ }).click();
  88  |       await expect(page).toHaveURL(
  89  |         (url) => url.searchParams.get("dateUnknown") === "true",
  90  |       );
  91  |       sharedContext(page, { dateUnknown: "true", timeBasis });
  92  |     }
  93  |   }
  94  | });
  95  | 
  96  | test("young-event.web-organizer-order", async ({ page }) => {
  97  |   const webOrder = [
  98  |     ...fixture.organizerIds.slice(0, 6),
  99  |     ...fixture.organizerIds.slice(12),
  100 |     ...fixture.organizerIds.slice(6, 12),
  101 |   ];
  102 |   for (const width of [1280, 390]) {
  103 |     await page.setViewportSize({ width, height: 844 });
  104 |     await gotoAndWaitForReady(
  105 |       page,
  106 |       `${root}/organizers?${new URLSearchParams({ search: fixture.marker })}`,
  107 |     );
  108 |     const organizerLinks = page.locator(
  109 |       `#main-content a[href^="${root}/organizers/${fixture.marker}"]:visible`,
  110 |     );
  111 |     const ids = () =>
  112 |       organizerLinks.evaluateAll((elements) =>
  113 |         elements.map((element) =>
  114 |           element.getAttribute("href")?.split("/").at(-1),
  115 |         ),
  116 |       );
  117 |     expect(await ids()).toEqual(webOrder.slice(0, 20));
  118 |     await page.getByRole("link", { name: /下一页|Next page/ }).click();
  119 |     await expect(page).toHaveURL((url) => url.searchParams.get("page") === "2");
  120 |     sharedContext(page, { search: fixture.marker });
  121 |     expect(await ids()).toEqual(webOrder.slice(20));
  122 |     await organizerLinks.first().click();
  123 |     await expect(page).toHaveURL(`${root}/organizers/${webOrder[20]}`);
  124 |     await gotoAndWaitForReady(
  125 |       page,
  126 |       `${root}/organizers?${new URLSearchParams({ search: fixture.marker, page: "3" })}`,
  127 |     );
  128 |     await expect(organizerLinks).toHaveCount(0);
  129 |     await expect(
  130 |       page.getByText(/未找到主办方|No organizers found/),
  131 |     ).toBeVisible();
  132 |   }
  133 | });
  134 | 
  135 | test("young-event.fixed-browse-filter-options", async ({ page }, testInfo) => {
  136 |   await page.setViewportSize({ width: 390, height: 844 });
  137 |   await gotoAndWaitForReady(
  138 |     page,
  139 |     `${root}?${new URLSearchParams({ search: fixture.search })}`,
  140 |   );
  141 |   await expect(eventLink(page, 7)).toContainText("未知模块");
  142 |   await expect(eventLink(page, 7)).toContainText("未知级别");
  143 |   await gotoAndWaitForReady(page, `${root}/calendar?date=2035-09-15&view=day`);
  144 |   await expect(
  145 |     page.getByRole("button", { name: /更多筛选|More filters/ }),
  146 |   ).toHaveCount(0);
  147 |   {
  148 |     const prefix = "young-event";
  149 |     const path = root;
  150 |     const context = {
  151 |       search: fixture.search,
  152 |       module: "未知模块",
  153 |       activityLevel: "未知级别",
  154 |     };
```