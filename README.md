# OSLogViewer

A SwiftUI-based viewer for inspecting `OSLog` entries directly inside your iOS or iPadOS app — no Mac or external tools required.

## ✨ Features

- 🔍 View OSLog logs inside your app
- 🧭 Filter logs by `subsystem` and `category`
- 🔎 Full-text search
- 📤 Export logs for sharing or offline analysis
- 📱 Adaptive layout for both iPhone and iPad
- 🧱 Built entirely with **SwiftUI**

## Preview

![Preview](preview.gif)

## Installation

You can add Dependencies to an Xcode project by adding it to your project as a package.

> https://github.com/gonefish/OSLogViewer

If you want to use Dependencies in a [SwiftPM](https://swift.org/package-manager/) project, it's as
simple as adding it to your `Package.swift`:

``` swift
dependencies: [
 .package(url: "https://github.com/gonefish/OSLogViewer.git", branch: "main")
]
```

And then adding the product to any target that needs access to the library:

```swift
.product(name: "OSLogViewer", package: "OSLogViewer"),
```

## Quick start

```swift
import OSLogViewer

struct ContentView: View {
    var body: some View {
        NavigationStack {
          OSLogViewer()
        }
    }
}
```

## License

This library is released under the MIT license. See [LICENSE](LICENSE) for details.
