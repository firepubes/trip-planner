# iPhone app setup

Trip Planner is configured to run as a native iOS app using Capacitor.

## On a Mac

1. Install Node.js and Xcode.
2. Clone the repository.
3. Install dependencies:

```bash
npm install
```

4. Build and generate the iOS project:

```bash
npm run cap:add:ios
```

5. Open the native project:

```bash
npm run cap:open:ios
```

6. In Xcode, select your iPhone as the run destination, configure your Apple Developer Team under **Signing & Capabilities**, then press **Run**.

The app ID is `com.firepubes.tripplanner` and the display name is `Trip Planner`.

## GitHub Actions

The `Build iOS app` workflow can also generate the native `ios/` project on a macOS GitHub runner. It uploads the generated project as a workflow artifact. App Store/TestFlight signing is intentionally not configured because that requires your Apple Developer account and signing credentials.
