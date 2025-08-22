# Simple Calculator (iOS, SwiftUI)

A minimal, accessible calculator with no tracking and no data collection. Built for fast App Store approval.

## Requirements
- Xcode 15+
- iOS 15+ target

## Build (with XcodeGen)
1. Install XcodeGen: `brew install xcodegen`
2. Generate project: `xcodegen generate`
3. Open `SimpleCalculator.xcodeproj` and build/run.

## Configure for App Store
1. In `project.yml`, set your `DEVELOPMENT_TEAM` and `PRODUCT_BUNDLE_IDENTIFIER`.
2. Provide App Icon assets: run the script below or drop your icons in `App/Assets.xcassets/AppIcon.appiconset/`.
3. Set app name, subtitle, keywords, and description in App Store Connect.
4. Privacy: This app collects no data and does not track. `App/PrivacyInfo.xcprivacy` is included.
5. Screenshots: Provide at least 6 (5.5", 6.7"). Use light and dark appearances.

## Tests
`⌘U` or run `SimpleCalculatorTests` scheme.

## Icon Generation (optional)
Run:
```bash
./scripts/generate_app_icons.sh icon-base.png
```
Produces all required sizes into `AppIcon.appiconset`.
