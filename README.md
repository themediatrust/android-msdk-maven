# TMT Maven Repository

[![Maven](https://img.shields.io/badge/Maven-repository-blue.svg)](https://themediatrust.github.io/maven/)
[![Platform](https://img.shields.io/badge/platform-Android%2021%2B-lightgrey.svg)](https://developer.android.com/)

Static Maven repository served via GitHub Pages, hosting binary artifacts for The Media Trust mobile SDKs.

**Base URL:** `https://themediatrust.github.io/maven/`

## Available Artifacts

| Group ID | Artifact ID | Description |
|----------|-------------|-------------|
| `com.themediatrust` | `media-filter-sdk` | Media Filter SDK for Android |

Latest version: see the [maven-metadata.xml](com/themediatrust/media-filter-sdk/maven-metadata.xml) for the up-to-date version list.

## Installation

### Gradle (Kotlin DSL)

```kotlin
repositories {
    google()
    mavenCentral()
    maven { url = uri("https://themediatrust.github.io/maven/") }
}

dependencies {
    implementation("com.themediatrust:media-filter-sdk:1.3.0")
}
```

### Gradle (Groovy DSL)

```groovy
repositories {
    google()
    mavenCentral()
    maven { url 'https://themediatrust.github.io/maven/' }
}

dependencies {
    implementation 'com.themediatrust:media-filter-sdk:1.3.0'
}
```

## Quick Start

```kotlin
import com.themediatrust.mediafilter.MediaFilter

// Initialize the SDK during Application.onCreate().
MediaFilter.configure(this, apiKey = "YOUR_API_KEY")
```

See the integration guide for full setup including ad-network adapters.

## Versioning

Versions follow [Semantic Versioning](https://semver.org/spec/v2.0.0.html). Detailed release notes for the SDK itself (filter behavior, ad-network adapter changes, bug fixes) are distributed to publishers separately.

## Documentation

Full integration documentation and API reference are provided to publishers under separate cover. Contact your account representative for access.

## Support

For integration support, contact [support@themediatrust.com](mailto:support@themediatrust.com).

## License

Proprietary. See [LICENSE](LICENSE) for terms.

Copyright (c) 2026 The Media Trust LLC. All rights reserved.
