<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-zai 1.2.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-zai.git", from: "1.2.0")
```

Products: `SwiftAIZAI`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Z.AI for Swift

`SwiftAIZAI` adds Z.AI to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/zai` and supports text generation.

Provider guide with models, options, streaming and errors:

- [Z.AI](https://swiftaisdk.github.io/SwiftAISDK/providers/zai/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIZAI` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIZAI

let provider = try AIProviders.zai(configuration: ZAIProviderSettings())
```

By default the provider reads `ZAI_API_KEY` from the environment; values set in `ZAIProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-zai` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
