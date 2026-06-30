# mobileMoneySubSaharanAfrica
This project contains metadata for mobile money applications in Sub-Saharan Africa.

## Dataset Metadata

This dataset contains metadata for Android applications collected from the Google Play Store and APK samples. Each row represents a single application version and includes information about its identity, publisher, technical specifications, and APK file characteristics.

### Metadata Fields

| Column | Description |
|---------|-------------|
| `country_name` | Country associated with the data collection or Play Store region. |
| `app_name` | Name of the Android application. |
| `provider` | Application developer or publisher. |
| `Package_Name` | Unique Android package identifier (e.g., `com.example.app`). |
| `Version_Name` | Human-readable version of the application. |
| `SHA256_APK_base` | SHA-256 cryptographic hash of the APK file (APK splits not included), used to uniquely identify the application binary and verify its integrity. |
| `APK_base_Size_MB` | Size of the APK file (APK splits not included) in megabytes (MB). |
| `Collection_Date` | Date when the application metadata and APK were collected. |
| `category` | Google Play Store application category (e.g., Tools, Education, Finance, Games). |
| `playstore_url` | URL of the application's Google Play Store page. |
| `Min_SDK` | Minimum Android SDK version required to install and run the application. |
| `Target_SDK` | Android SDK version targeted by the application during development. |

### Notes

- Each record corresponds to a specific application version.
- The `Package_Name` uniquely identifies an Android application across versions.
- The `SHA256_APK_base` field can be used to detect duplicate APKs and verify file integrity.
- SDK-related fields (`Min_SDK` and `Target_SDK`) provide information about Android compatibility.
- The `Collection_Date` indicates when the metadata was retrieved and may differ from the application's release date.
