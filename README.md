# The Daily Ration

A nutrition tracker for people who cook and don't want or need another account or subscription.

If you make most of your food from real ingredients and you've spent ten minutes inside a mainstream nutrition app wondering where the recipe button is, this is for you. The Daily Ration treats recipes as the main thing — not a premium upsell — and gets out of your way.

> _SCREENSHOT: top-of-page shot — Log tab on iPhone, chart header with rings + a couple of meal cards below._

---

## What it does

- **Scan a barcode, scan a label.** Point your camera at a barcode or a nutrition label and the app reads it into a new ingredient.
- **Over 350 ingredients on day one.** Eggs, olive oil, chicken thighs, black beans, cheddar, oats — the stuff you actually cook with is already there with full USDA nutrition data. No data entry before your first meal.
- **Search 400,000+ foods.** Need something niche? The full USDA FoodData Central database is a tap away.
- **Cook a recipe once, log it forever.** Build a recipe out of ingredients, and every time you eat it, log it as one tap.
- **See your day at a glance.** Calories, protein, carbs, fat, plus the micronutrients you actually care about — all on one screen.
- **Trends across days and weeks.** Tap any nutrient on the day view to see a 7-day chart with your target line.
- **Sync across your devices.** iCloud sync is opt-in — enable it in Settings if you want multi-device. No account, no signup, no password.
- **Optional Apple Health integration.** Publish what you eat to Health, or pull in your active calories burned to compare against what you ate. Both are off by default and independently configurable.

> _SCREENSHOT: split image of iPhone Log view + iPad Recipes view to show multiplatform._

---

## How it's organized

Four tabs.

### Log
Your day. The top of the screen is a chart header showing macros, calories vs. target, micronutrients, and limit nutrients (the things you want to stay under). Below that, a list of meals you've logged today.

Swipe left or right anywhere on the day view to walk through previous days.

> _SCREENSHOT: Log tab with chart header expanded (rings, bars, donut). Day with a few meals logged so totals are non-trivial._

**Tap any nutrient on the chart** — a ring, a bar, the calorie center, anything — to open a 7-day trend popup with a target line. Swipe inside the popup to walk back through earlier weeks.

> _SCREENSHOT: nutrient trend popup open over the Log view, showing the 7-day bar chart with target line._

### Trends
The longer view. Daily totals across weeks, average values, and a per-nutrient breakdown for whatever stretch you're looking at.

> _SCREENSHOT: Trends tab on iPhone or iPad._

### Recipes
Your cookbook. Each recipe is a list of ingredients with quantities. The nutrition is computed from the ingredients — you don't enter it by hand.

When you log a recipe as a meal, it captures a snapshot of the nutrition at that moment. So if you tweak the recipe later, your historical meals don't change.

> _SCREENSHOT: Recipes tab showing the list, plus a recipe detail with its ingredients and computed nutrition._

### Ingredients
Your pantry. Every ingredient you've added — whether from a USDA search, a label scan, or typed in by hand — lives here with its full nutrition breakdown.

> _SCREENSHOT: Ingredients tab showing the list._

---

## Reading the chart header

The chart header packs a lot into a small space. Here's the cheat sheet:

- **Big donut** on the left: today's macros (protein, carbs, fat). Tap a wedge for that nutrient's trend.
- **Calorie ring** in the middle of the donut: how close you are to your calorie target. Past target it shifts toward red.
- **Inner green ring** (only if you've enabled Apple Health active calories): how much you've burned today, scaled against the same calorie target so the two are directly comparable.
- **Limit bars** on the right (Sodium / Saturated Fat / Sugar): horizontal bars that go from green to amber to red as you approach your daily limit. You only see the ones you've enabled in Settings.
- **Micro rings** below (Iron / Calcium / Magnesium / Potassium / Fiber): small rings that fill toward your daily target. Each one can be toggled on or off independently in Settings.

Tap anything to drill in.

> _SCREENSHOT: chart header on its own, annotated with callouts for each element. (You can also leave this un-annotated and let the next caption explain — your call.)_

---

## Apple Health

Off by default. Two independent toggles in Settings → Apple Health:

**Publish nutrients to Health.** When on, every meal you save also writes a nutrition entry to Apple Health, grouped under "DailyRation" as a meal correlation. Edits and deletes propagate. To stop sharing later, open the Health app → Sharing → Apps and Services → DailyRation.

**Show active calories.** When on, the calorie display reads your active energy burned from Health and renders a green ring inside the orange calorie ring, scaled to the same target.

> _SCREENSHOT: Settings → Apple Health section with both toggles visible._

These are split because they're useful independently. You might want to publish nutrition to Health without trusting Apple's calorie burn estimate. Or you might want to see your burn against your intake without writing anything back to Health.

---

## Customizing the display

**Settings → Nutrients** lets you toggle each non-macro nutrient on and off independently. If you don't care about Sugar, hide Sugar — the Sugar bar disappears from the day view and the rest stays untouched.

**Settings → Appearance** has eight accent colors. The colors flow through every accent in the app — toggles, selection rings, and segmented controls will all have your personal hue.

> _SCREENSHOT: Settings showing the Nutrients section AND the Appearance accent grid._

---

## Privacy

There is no Daily Ration server. Nothing is collected, sold, transmitted, profiled, or analyzed.

- Your data lives on your device. If you enable iCloud sync in Settings, it also lives in your private iCloud database — accessible only by you.
- USDA ingredient search hits USDA's public API directly from your device. The query is the food name; nothing personal.
- Apple Health integration is opt-in, runs entirely on-device, and never leaves your iCloud account.

A formal privacy policy ships with the App Store listing.

---

## Requirements

- iPhone or iPad running iOS 17 or later
- Mac running macOS 14 or later
- Apple ID signed in (for iCloud sync — the app works without it, but you'll need it for multi-device)

---

## Support

Found a bug? Have a feature request? [Open an issue.](https://github.com/w15p/dailyration/issues)

---

© 2026 w15p
