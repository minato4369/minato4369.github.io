# minato4369.github.io
Privacy &amp; policies
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>

    <!-- ═══════════════════════════════════════════════════
         NSPrivacyTracking
         TRUE because AdMob uses IDFA for ad personalisation
         when the user grants ATT permission.
    ════════════════════════════════════════════════════ -->
    <key>NSPrivacyTracking</key>
    <true/>

    <!-- ═══════════════════════════════════════════════════
         NSPrivacyTrackingDomains
         Domains contacted for tracking purposes (AdMob).
    ════════════════════════════════════════════════════ -->
    <key>NSPrivacyTrackingDomains</key>
    <array>
        <string>googleadservices.com</string>
        <string>googlesyndication.com</string>
        <string>doubleclick.net</string>
        <string>google-analytics.com</string>
        <string>googletagmanager.com</string>
    </array>

    <!-- ═══════════════════════════════════════════════════
         NSPrivacyCollectedDataTypes
         Data types collected by the app and its SDKs.
    ════════════════════════════════════════════════════ -->
    <key>NSPrivacyCollectedDataTypes</key>
    <array>

        <!-- Device ID (IDFA) — AdMob, only with ATT consent -->
        <dict>
            <key>NSPrivacyCollectedDataType</key>
            <string>NSPrivacyCollectedDataTypeDeviceID</string>
            <key>NSPrivacyCollectedDataTypeLinked</key>
            <false/>
            <key>NSPrivacyCollectedDataTypeTracking</key>
            <true/>
            <key>NSPrivacyCollectedDataTypePurposes</key>
            <array>
                <string>NSPrivacyCollectedDataTypePurposeThirdPartyAdvertising</string>
            </array>
        </dict>

        <!-- Coarse location — AdMob uses IP-based country targeting -->
        <dict>
            <key>NSPrivacyCollectedDataType</key>
            <string>NSPrivacyCollectedDataTypeCoarseLocation</string>
            <key>NSPrivacyCollectedDataTypeLinked</key>
            <false/>
            <key>NSPrivacyCollectedDataTypeTracking</key>
            <false/>
            <key>NSPrivacyCollectedDataTypePurposes</key>
            <array>
                <string>NSPrivacyCollectedDataTypePurposeThirdPartyAdvertising</string>
            </array>
        </dict>

        <!-- Purchase history — StoreKit IAP (packs + full game) -->
        <dict>
            <key>NSPrivacyCollectedDataType</key>
            <string>NSPrivacyCollectedDataTypePurchaseHistory</string>
            <key>NSPrivacyCollectedDataTypeLinked</key>
            <false/>
            <key>NSPrivacyCollectedDataTypeTracking</key>
            <false/>
            <key>NSPrivacyCollectedDataTypePurposes</key>
            <array>
                <string>NSPrivacyCollectedDataTypePurposeAppFunctionality</string>
            </array>
        </dict>

        <!-- Other data — player names entered locally, never transmitted -->
        <dict>
            <key>NSPrivacyCollectedDataType</key>
            <string>NSPrivacyCollectedDataTypeOtherUserContent</string>
            <key>NSPrivacyCollectedDataTypeLinked</key>
            <false/>
            <key>NSPrivacyCollectedDataTypeTracking</key>
            <false/>
            <key>NSPrivacyCollectedDataTypePurposes</key>
            <array>
                <string>NSPrivacyCollectedDataTypePurposeAppFunctionality</string>
            </array>
        </dict>

    </array>

    <!-- ═══════════════════════════════════════════════════
         NSPrivacyAccessedAPITypes
         System APIs accessed by the app or linked SDKs.
    ════════════════════════════════════════════════════ -->
    <key>NSPrivacyAccessedAPITypes</key>
    <array>

        <!-- UserDefaults — game settings, purchased packs, player stats -->
        <dict>
            <key>NSPrivacyAccessedAPIType</key>
            <string>NSPrivacyAccessedAPICategoryUserDefaults</string>
            <key>NSPrivacyAccessedAPITypeReasons</key>
            <array>
                <string>CA92.1</string>
            </array>
        </dict>

        <!-- File timestamp — required by GoogleMobileAds SDK -->
        <dict>
            <key>NSPrivacyAccessedAPIType</key>
            <string>NSPrivacyAccessedAPICategoryFileTimestamp</string>
            <key>NSPrivacyAccessedAPITypeReasons</key>
            <array>
                <string>C617.1</string>
            </array>
        </dict>

        <!-- System boot time — required by GoogleMobileAds SDK -->
        <dict>
            <key>NSPrivacyAccessedAPIType</key>
            <string>NSPrivacyAccessedAPICategorySystemBootTime</string>
            <key>NSPrivacyAccessedAPITypeReasons</key>
            <array>
                <string>35F9.1</string>
            </array>
        </dict>

        <!-- Disk space — required by GoogleMobileAds SDK -->
        <dict>
            <key>NSPrivacyAccessedAPIType</key>
            <string>NSPrivacyAccessedAPICategoryDiskSpace</string>
            <key>NSPrivacyAccessedAPITypeReasons</key>
            <array>
                <string>85F4.1</string>
            </array>
        </dict>

    </array>

</dict>
</plist>
