### v3.7.6 Beta Changelog

- Features or Enhancements
   - Docker base image update to Ubuntu 22.04
   - Dockerfile QA
   - Migrated from Pip to Poetry for dependency management
   - Migrate from setup.py to use poetry for build and publish
   - Python 3.11 support
   - Docker ADB connection improvements (host.docker.internal translation for localhost)
   -  IOS Swift RulesUpdates `ios_biometric_bool`, `ios_biometric_acl`, `ios_keychain_weak_acl_device_passcode`, `ios_keychain_weak_accessibility_value`, `ios_insecure_random_no_generator`, `ios_biometry_hardened`
   - Android SCA rules update
   - Entropies scan support for strings
   - Regex Hardening: Fixes possible Regex DoS in rules and MobSF code base
   - Tox QA
   - Added poetry build test
   - Updated mobsf PyPI publishing workflow 
   - Update local DBs
   - URLs/Email extraction refactor
   - Static and Dynamic Binary Analysis QA
   - Refactor Dex permissions
   - Refactor Androguard `apk.APK()` usage
   - Fallback certificate analysis using apksigtool
   - Use BeautifulSoup4 to prettify malformed XML
   - Detect non standard XML namespace in AndroidManifest.xml, Fixes : #2198
   - Updated android permissions list
   - Updated android permission update check script
   - Github Actions version update
   - Apktool bump
   - Bump httptools
   - Bump yara-python-dex
   - Docker image build test for PRs
   - iOS Source Report Fix
   - Removed unwanted pinned repository
   - Frida APK Patcher (WIP)
   - Fix for Recent Scans `scan not completed` for iOS zip
   - Fix for MachO stripped symbols false positive
   - Fix bug in IPA download
   - iOS/Android form validation fix
   - Fix missing exported components
 - Enterprise Feature Request
      - String extraction from APK, Source, AAR, JAR, SO.
      - Android strings sections to show source of strings extracted
      - Strings extraction refactor
      - Support for independent `.so` scan
      - Dylib analysis support
      - Dylib string extraction
      - Improved iOS Plist secret extraction
      - Support for Independent `.dylib` scan
      - Symbols view for dylib and so
      - Trackers support for so
      - AAR/JAR obfuscation and debug check
      - Independent Static Library(.a) ELF/MachO Analysis
      - Mac FAT binary only supported on Mac


  
     
    
  

## What's Changed
* Update dynamic_analysis.html by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2218
* Hotfix: Handle Docker <-> ADB connectivity internally by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2219
* update apktool to 2.8.1 by @superpoussin22 in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2220
* update apktool by @superpoussin22 in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2225
* HOTFIX: Dynamic Analyzer Support Alert by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2227
* [HOTFIX] Regex + Rule Update by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2232
* [EFR06] Independent Shared Object (.so) Scan and Improved String search by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2228
* Update macho_analysis.py - SYMBOLS STRIPPED False Negative by @Karmaz95 in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2234
* [EFR-08] Dylib + Symbols + Other Features by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2239
* Fix missing exported components by @Abb4d0n in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2176
* [EFR09] AAR/JAR obfuscation and debug check + Exception Handed strings and symbols extraction by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2240
* [EFR10] Independent Static Library(.a) ELF/MachO Analysis by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2242
* Pip to poetry and Dockerfile update by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2244
* Docker Buildx test by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2247
* [HOTFIX] bs4 malformed xml parsing + xml namespace detection by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2248
* [HOTFIX] Migrate from setup.py to poetry, tox QA by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2249

## New Contributors
* @Karmaz95 made their first contribution in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2234
* @Abb4d0n made their first contribution in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2176

**Full Changelog**: https://github.com/MobSF/Mobile-Security-Framework-MobSF/compare/v3.6.9...v3.7.6

### v3.6.9 Beta Changelog

- Features or Enhancements
   - MobSF Dynamic Analysis support for Docker image
   - Updated Documentation to include support for Corellium ARM64 Android VMs
   - Add support for environment variables to configure MobSF
   - Android SCA extract icon from SVG
   - OFAC Sanctioned Country Check
   - Improved Android Certificate Analysis
   - Updated Android Manifest Analysis Rules
   - Enterprise Feature Request
      - Summary of Findings under each section
      - Support for independent scanning of AAR ad JAR files.

## What's Changed
* Adding numeric_owner as a keyword argument by @TrellixVulnTeam in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2050
* Scheduled weekly dependency update for week 41 by @pyup-bot in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2046
* HOTFIX: UI changes and warning on mobsf.live by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2051
* Split certificate analysis out, suppression list fixes by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2052
* hotfix for quark rules location by @superpoussin22 in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2053
* HOTFIX: jadx update to 1.4.5  by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2064
* Installation script error: Solving spelling error by @th3-d4v1d-c0de in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2067
* Android APK support extracting icon SVG from XML by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2060
* HOTFIX: Setup improvement by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2078
* Apktool 2.7.0 update by @superpoussin22 in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2082
* New Android Manifest Rule: App support vulnerable android versions by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2114
* Fix for filenames containing ampersand by @evmxattr in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2129
* HOTFIX - Fix broken docker builds by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2135
* Fix Scorecard Severity Distribution chart data by @antoinbo in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2140
* HOTIX: Update Dockerfile to install jq by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2149
* [HOTFIX] Add support for environment variable for MobSF config by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2150
* HOTFIX: Android min SDK check on janus vulnerability detection by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2159
* [Enterprise Feature Request EFR02] Support summary of severity in each section. by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2160
* [EFR05] Enterprise Feature Request: AAR and JAR support by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2163
* Scheduled weekly dependency update for week 24 by @pyup-bot in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2187
* Feature updates and Bug Fixes by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2197
* HOTFIX: MobSF Android Dynamic Analysis Docker Support by @ajinabraham in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2214

## New Contributors
* @th3-d4v1d-c0de made their first contribution in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2067
* @evmxattr made their first contribution in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2129
* @antoinbo made their first contribution in https://github.com/MobSF/Mobile-Security-Framework-MobSF/pull/2140

**Full Changelog**: https://github.com/MobSF/Mobile-Security-Framework-MobSF/compare/v3.6.0...v3.6.9

### v3.6.0 Beta Changelog

- Features or Enhancements
   - False Positive Triaging / Suppression Triaging Support for critical Android and iOS Security Analysis features.
      - Android Binary & Source - Supports Code Analysis and Manifest Analysis
      - iOS Binary - Supports Binary Code Analysis
      - iOS Source - Supports Code Analysis
      - New REST APIs for Suppression Support
   - Android Certificate Analysis improvements
   - Remove RELRO check from android binary analysis due to false positives
   - iOS Bundle ID extraction improvements
   - Feature parity - Allow IPA downloads from reports view 
   - Code QA: Reduce False positives in identified secrets
   - Check for updates from Github releases
   - M1 Mac support
   - Disabled by default feature to support hotspots in AppSec Scorecard
   - Dependency updates
   - Added CodeQL scan on MobSF python code base

- Bug Fixes
  - Fixes #1999, #1917, #2042 #1981 #2014 #2043 
  - Fixed a bug in JSON response REST API
  - iOS URL view fix
  - Code fixes to address minor security issues in thrid party libraries.
  - Handle JADX timeouts
 

### v3.5.0 Beta Changelog

- Features or Enhancements
   - MobSF Application Security Scorecard for scoring mobile application security
   - Scorecard REST API
   - Published Static Analyzer online [mobsf.live](https://mobsf.live) (Thanks to Jovan Petrovic for sponsoring the server)
   - Improved App Security Scoring Logic
   - Improved PDF Report, Reduce generation times.
   - Disable CVSSv2 by default. 
   - Non blocking file upload from home screen.
   - Android and iOS SAST rule QA
   - Manifest, Certificate, Transport Security and Network Security rule QA
   - Common severity levels High, Warning, Info and Secure.
  

- Bug Fixes
  - Fixes #1885
  - Replaced PWD with dedicated server

### v3.4.6 Beta Changelog

- Features or Enhancements
   - Quark Version Update
   - New Frida Scripts from F-Secure labs
   - Manual Activity Launcher and REST API
   - Suppress warnings from third party
   - LIEF integration QA
   - Update Janus Vulnerability description
   - General Code QA
   - Improve Setup script
   - Update Dockerfile to use non-root user
   - PDF in landscape
   - Add healthcheck to dockerfile
   - Update Android API rules
   - iOS Hardcoded Secret extraction from plists
   - Add browsable activities in android diff
   - Multiplatform docker image
   - Added checks and bypass for certificate transparency
   - Updated Android Static Analysis rules
   - Improved Split APK support, now supports .apks file
   - Ability to lookup and download APK from apktada/apkpure/apkplz
   - Dynamic Analyzer: Get Runtime Application Third party dependencies
   - Persist Frida Code change in session storage
   - Show Base64 strings decoded at runtime and the called class
   - Detect Trackers from Runtime Dependencies and Network Traffic
   - Windows Binskim version pinning
   - Global Proxy Configuration for Dynamic Analyzer

- Bug Fixes
  - Fix Django 4.0 support
  - Fix minor bugs
  - Fix dependency issues

### v3.4.3 Beta Changelog

- Features or Enhancements
   - Android Dynamic Analysis TLS/SSL Security Tester
   - Dynamic Analysis without Static Analysis
   - Support Dynamic Analysis of third party apps in VM/AVD
   - Download and perform static analysis of third party apps from VM/AVD
   - Dynamic Analysis enhancement to preserve app config/data
   - Improved SSL Pinning Bypass script
   - Added Intent dumper auxiliary Frida script
   - Added an auxiliary method bypass template script
   - Security Hardening
   - Addressing LGTM issues and QA
   - Android Permissions Mapping update and Typo fix
   - VirusTotal Code QA
   - Refactored Logcat log viewer to show only app specific logs
   - Xposed Improvements and updates of agents
   - Updated frontend libraries for CodeMirror and EnligherJS
   - New REST API exposed for TLS/SSL tests
   - General Code QA

- Bug Fixes
  - Fixed Windows Setup script
  - Fixed typo and incomplete description in Android permission mapping

### v3.4.0 Beta Changelog

- Features or Enhancements
   - Android Hardcoded Secrets False Positive Improvement
   - New Android Crypto Rule
   - Rescan Fail-Safe and Code QA
   - Auto Comment for PR and Issues
   - USE_HOME by default
   - Dynamically Display Config Location
 

- Bug Fixes
  - Fixed a bug in iOS ATS plist analysis

### v3.3.5 Beta Changelog

- Bug Fixes
  - Removed Android Shared Library PIE Check
  - Improved Frida Instrumentation Logic to prevent Frida bypass
  - Fixed a False positive in Android Java Random rule
  - Fixed a bug that caused multiple first time saves of the same scan
  - Fixed Dynamic Analyzer JSON Report REST API bug
 
### v3.3.3 Beta Changelog
- Features or Enhancements
   - Android Hardcoded Secrets Improvement
   - iOS IPA binary analysis improvements
   - Improved Android Manifest Analysis
   - Improved Setup
   - Updated to APKiD that is maintained by MobSF Team
   - Static Analysis Rule QA
   - macOS BigSur support
   - Update libsast to skip large files.
   - Improved iOS plist analysis
   - Relaxed Android Source code zip requirements
 
- Bug Fixes
  - Fixed a bug in Android Shared Library RELRO check
  - Fixed a bug in Windows setup that prevents detection of python version on the first run
  - Fixed a bug in Recent Scan
  - Fixed a bug in root CA naming that prevented traffic interception

### v3.2.9 Beta Changelog
- Bug Fixes
  - MobSF python package fix

### v3.2.8 Beta Changelog
- Features or Enhancements
  - OWASP MSTG Mapping to Rules
  - Python 3.9 support
  - Prebuilt DEX enabled yara-python wheels 
  - Dynamic Downloading of frida-server binary
  - Code QA
 
- Bug Fixes
  - Windows APPX bug fix

### v3.2.6 Beta Changelog
- Features or Enhancements
  - Added Support for Android 10 Dynamic Analysis
  - Published new REST APIs for Dynamic Analysis
  - New Source Tree Browser for Android Static Analysis 
  - Improved Binary and Shared Object Analysis with LIEF
  - Added Support for NIAP v1.3
  - Added a world map UI plotting server locations
  - Added Maltrail Domain Check
  - Improved Android Permission Analysis
  - iOS Objective C Rule improvements
  - Android Kotlin Rule improvements
  - MobSF now available as a python package and published to pypi
  - Migrated CI from Travis to Github Action
  - Improved File Magic Check on Uploads
  - Post Install Check script
  - Static Analysis Hardcoded Secrets Section from strings.xml
  - Updated Dependencies
  - Custom Header for REST API Key

- Bug Fixes
  - Fixed Install Verification bug on older Android versions
  - Fix a Regex DoS in rule
  - Fixed IPA Static Analysis Bug
  - Minor PDF template fix

### v3.1.1 Beta Changelog
- Features or Enhancements
  - Added Support for Android Network Security Config Analysis
  - Replace SAST core with libsast
  - Support for line numbers in source code
  - Replaced Code Viewer with EnlighterJS
  - Kotlin source scan support
  - Improved Certificate Analysis
  - Genymotion Cloud Support
  - Support Android Emulator AVD x86, ARM, ARM64
  - Verify Dynamic Analysis APK Installation
  - Dynamic Analysis: Support APK with test package requirements
  - Automatic MobSFy on Frida binary update
  - Expose App result compare REST API and Update REST API Docs
  - Clean up MobSF proxy on exit
  - IPA Binary Regex QA
  - Optimize Root Checking Frida Script
  - Environment Checks to see if API Level is supported and /system is writable
  - Prebuilt dex enabled yara-python and improved setup, tox, tests
  - Added Chinese documentation
  - Reduce Docker image size
  - Improved Postgresql Docker Support
  - Android Dynamic Analysis QA
  - Update Dependencies

- Bug Fixes
  - Android Rule Fixes
  - Fixed API Monitor which was broken from Frida 12.8.19
  - Fixed iOS ATS bug
  - Fix Black PDF background issue
  - LGTM Scan Code QA

- Security
  - Fixed Regex DoS in Email Extraction
  - Fixed insecure Default Bind to 0.0.0.0

### v3.0.5 Beta Changelog
- Features or Enhancements
  - iOS Swift Source Code Support
  - Improved iOS Swift and Objective C rules
  - OWASP MASVS/MSTG Standard Support
  - Brand New PDF Reports
  - Improved SAST Core
  - Improved iOS Application Transport Security Checks
  - Improved iOS Permission Checks
  - Added IP to Geolocation Feature for Domain Malware Check
  - URL and IP extraction from IPA
  - App Risk Calculation from App Security Score
  - Improve Recent Scan View
  - Add Jtool2 support
  - Code QA
  - New Docs Site

- Bug Fixes
  - Classdump bug fixes
  - Geolocation bug fixes

### v3.0.1 Beta Changelog
- Features or Enhancements
   - Simplified REST API
   - Improved Android App Name detection
   - Dynamic Analysis proper Root CA naming
   - Changes to Support Android x86 Docker
   - Dependency updates
   - Code QA

- Bug Fixes
  - Handle Invalid ATS domain entries iOS
  - Fixes a Template Bug

### v3.0.0 Beta Changelog
- Features or Enhancements
   - OWASP Mobile Top 10 2016 is supported
   - Major UI Update for MobSF
   - Major Schema changes to rest API
   - iOS URLs Scheme
   - iOS ATS Analysis improved
   - New iOS Static Analysis Rules
   - New iOS Static Analysis Rules
   - New Android Manifest Analysis Rules
   - Updated dependencies
   - Optimized Windows Setup
   - Updated Scoring mechanisms
   - Improved Tracker detection
   - Remove Global Proxy after dynamic analysis
   - Android Permission database update
   - Added Play with Docker support 
   - AppMonsta support
   - Code QA

- Bug Fixes
  - Fix Security issue #1197 (Directory Traversal)
  - iOS Static Analyzer fixes
  - Typo Fix
  - Moved to oscrypto and distro
  - Windows binscope bug fix
  - Reduce False positives 

### v2.0.0 Beta Changelog
- Features or Enhancements
   - Dynamic Analysis Support for Genymotion Android VMs 4.1 -9.0 x86
   - Improved Recent Scan
   - Replaced CapFuzz with HTTPtools
   - Automatic MobSFy with Xposed and Frida
   - Streaming logcat
   - Live API Monitor
   - Better SQlite DB View
   - Inbuilt Frida scripts for basic tasks
   - Custom Frida Script support
   - Frida Log Viewer
   - UI Changes
   - Browser PDF print support
   - Updated Tools
   - Baksmali performance improvements
   - Improved malware domain check
   - Multi OS Travis Support
   - Code QA

- Bug Fixes
  - Typo Fix
  - Reduce False positives 

### v1.1.6 Beta Changelog
- Features or Enhancements
   - 70x performance improvements for large APKs
   - CVSS, CWE tagging with results
   - Trackers Detection
   - App Store/ Playstore Details of supported packages
   - Added Security Score, Average CVSS Score, VirusTotal & Tracker Detection
   - Coloured logging
   - Better Logging and Exception Handling
   - Travis CI/CD integration
   - Optimized & Updated Dockerfile
   - Super fast java decompiling with JADX
   - Large scale Code QA
   - Enforced mandatory code linting
   - Integrated automated travis tests in Linux and OSX
   - Moved to proper production servers Gunicorn & Waitress
   - Improved icon detection
   - Android APK app real name
   - Moved from Oracle JDK to OpenJDK
   - Reduce False Positives
   - Enforced Least privilege mode
   - Improved Setup scripts
   - Moved to androguard based certificate printing
   - File less local db updates for better cross platform support
   - Static Analyzer rule updates and accuracy improvement
   - REST API - Recent Scans
   - classdump support for iOS swift binaries
   - Updated dependencies

- Bug Fixes
  - Fixed bug in Appx Analysis
  - Dynamic Analysis Bug Fix
  - Fix plist bug in iOS SCA
  - Performance Improvements
  
### v1.0.3 Beta Changelog
- Features or Enhancements
   - Android APK Scan Results Diffing Support
   - VirtualBox VM Headless mode
   - UI Changes
   - Improved Android icon analysis
   - CapFuzz for API Fuzzing
   - JSON Report REST API
   - Dependency Updates
   - Code QA and Refactoring
   - More unit tests
   - Update 3rd party tools
   - Improved APKiD Scans
   - Added Basic Environment Checks on first run
   - Docker support for PostgreSQL
   - Improved REST APIs
   - Android AVD 6 Support (Broken)
   - iOS IPA Analysis support in Linux
   - Improved Form Handling
   - REST API CORS Support
   - Improved Plist Parsing
   - Removed Faulty Binary Analysis
   - Improved Manifest Analysis
   - Updated Android Permission Mappings
   - New Setup and Run scripts for easy installation and usage
   - Updated Dockerfile
   - Multi Dex Support
   - Upstream Proxy Support
   - Improved String Extraction for Android

- Bug Fixes
  - Fixed manifest view
  - Performance improvements
  - Find Java Bug fixes
  - Fixed APK String extraction
  - Fixed Regression Bug
  - Fixed Byte Bug

### v0.9.5.4 Beta Changelog
- Features or Enhancements
   - REST API for MobSF and API Docs
   - Icon Extractor Android Static Analysis
   - Updating Libraries to latest
   - Malware Analysis Code refactoring
   - Updated ADB binaries
   - Code Refactoring Android Static Analysis
   - Android and iOS new static analysis rules added

- Bug Fixes
  - iOS file analysis bug fix
  - iOS Classdump exception fix
  - Unicode Unzip fix
  - sqlitedb isinstance bug fix
  - Dockerfile error fix
  - Bug Fix in skip classes
  - Bug Fix in https traffic decryption due to tornado upgrade
  - iOS Binary analysis regex fix
  - Android binary analysis bug fix

### v0.9.5.2 Beta Changelog

* Features or Enhancements
  * Supports Android ARM Emulator for Android Dynamic Analysis. Thanks to Matan Dobrushin - [Documentation](https://github.com/MobSF/Mobile-Security-Framework-MobSF/wiki/1.-Documentation#configuring-dynamic-analyzer-with-with-mobsf-android-412-arm-emulator)
  * Android Dynamic Analysis Code QA and Refactoring
  * Delete Scan Results from DB and related files under Recent Scan
  * Detects Apps Signed with SHA1-RSA
  * Added APKiD to MobSF Android APK Static Analysis
  * Python Dependency updates
  * Dockerfile updated
  * Added unit test for delete scan
  
* Bug Fixes
  * Fixed Android Certificate Analyzer find match bug
  * Android Static Analyzer content provider rules bug fix
  * Windows Static Analyzer Bugfixes
  * Moved from buggy syntaxhighlighter to highlightjs

### v0.9.4 Beta Changelog

* Features or Enhancements
  * Android Binary/ELF Analysis and Resource Analysis
  * Android App Static Analysis: Tapjacking Detection
  * Android App Static Analysis: Better Exported Component Analysis
  * iOS App Static Analysis: Listing App Permissions
  * iOS App Static Analysis: ATS Check
  * Better and Faster PDF Generation
  * Updated Dependencies
  * Optimised DB Interactions
  * Unit Tests for Static Analyzer, PDF Report Generation

* Bug Fixes
  * Windows App Static Analyzer Bug Fix
  * Fixed all PDF Related Bugs
  * Windows App Static Analyzer: BinScope Bug Fix
  * iOS App Static Analysis: Plist Bug Fix

### v0.9.3 Beta Changelog


* Features or Enhancements
  * Added Docker File
  * Clipboard Monitor for Android Dynamic Analysis
  * Windows APPX Static Analysis Support
  * Added Support for Kali Linux
  * Code Quality and Lintering
  * Partial PEP8 Formating, Code Refactoring and Restructuring
  * Imporved Static Analyzer Regex
  * Disabling Syntax Highlighter Edit mode
  * More MIME Type additions
  * Update File Upload Size to 100 MB
  * MobSFfy script to support commandline args
  * New strings.py tool for string extraction in iOS Apps.
  * Updated iOS Static Analysis ruleset.
  * Django Upgrade to 1.10
  * MobSF VM 0.3 Released

* Bug Fixes
  * Fixed Code Analyis Regex Error
  * Fixed iOS Binary Analyis and File Analysus PDF Generation bug
  * API Fuzzer Bug Fixes
  * SQLite3 Bug Fix
  * Fixed Bug when no code signing cert is present
  * Fixed Bug in xhtml2pdf
  * Dynamic Analysis Bug Fixes
  * Unicode Bug Fixes
  * Fixed MobSFy upload error
  * Fixed Variable redefining bug

* Security Fixes
  * Fixed Local File Inclusion casued due to incorrect regex

### v0.9.2 Beta Changelog

* Features
  * Drag and Drop support, allows upto 8 files in Web GUI
  * Mass Static Analysis - Mass static analysis on a directory of app binaries or zipped source code
  * Domain Malware check
  * CFR Decompiler updated to 0_115
  * Added Google Enjarify
  * Added procyon decompiler
  * Allows user to skip inbuilt android classes. (Performance improvement ~ 20%)
  * Android Code signing certificate check
  * Detect hardcoded Keystores
  * Static Analyzer rules updated for Android and iOS
  * Better Android Manifest analysis rule set
  * Dynamic Analysis Base64 Decoding
  * Support for Home Directory - Move all user created files and settings to Home directory

* Bug Fix
  * Dynamic Analyzer report print in Landscape mode
  * Windows fix for command prompt color support
  * Fixed Upper case file extension bug
  * PDF Creator unicode error fixed
  * Fixed manifest analyzer bug
  * Ptrace API recommendation enhancement

### v0.9.1 Beta Changelog

* Minor Bug Fixes
* Static Analyzer rules updated

### v0.9 Beta Changelog

* Improved and Responsive UI
* Search stored Static Analysis reports with APK MD5
* Recent Scan View
* Added Live Device/VM ScreenCast on Dynamic Analyzer view
* Added Basic Touch event based Interaction with ScreenCast
* Better Error Handling and Logging
* Improved Web Proxy
* Added a centralized log file for MobSF
* A new UI component to show the count of vulnerable components of Android App
* Tooltips explaining code nature
* All new API Fuzzer that can do Information Gathering, detect Security Headers, identify vulnerabilities like XXE, SSRF, Path Traversal, IDOR, Rate Limit Checking and perform Session related logical checks.
api tester
* Update APKs and pushed them to VM
* Updated and stable MobSF VM 0.2
* Added rules to static analyzer
* Added Custom VM and Android Device Support for MobSF Dynamic Analysis
* MobSF VM can now bypass Anti-Emulator Checks
* Support for Dynamically Installing and Removing MobSF RootCA
* Bug Fixes
  * Fixed Java path finding issue in windows
  * Fixed Set-Cookie Handling issue of Web Proxy
  * Fixed some UI issues
  * Fixed a bug in finding VirtualBox path in Mac and Linux

### v0.8.8 Beta Changelog

* New name: Mobile Security Framework (MobSF)
* Added Dynamic Analysis
* VM Available for Download
* Fixed RCE
* Fixed Broken Manifest File Parsing Logic
* Sqlite DB Support
* Fixed Reporting with new PDF report
* Rescan Option
* Detect Root Detection
* Added Requiremnts.txt
* Automated Java Path Detection
* Improved Manifest and Code Analysis
* Fixed Unzipping error for Unix.
* Activity Tester Module
* Exported Activity Tester Module
* Device API Hooker with DroidMon
* SSL Certificate Pinning Bypass with JustTrustMe
* RootCloak to prevent root Detection
* Data Pusher to Dump Application Data
* pyWebproxy to decrypt SSL Traffic

### v0.8.7 Beta Changelog

* Improved Static Analysis Rules
* Better AndroidManifest View
* Search in Files

### v0.8.6 Beta Changelog

* Detects implicitly exported component from manifest.
* Added CFR decompiler support 
* Fixed Regex DoS on URL Regex

### v0.8.5 Beta Changelog

* Bug Fix to support IPA MIME Type: application/x-itunes-ipa

### v0.8.4 Beta Changelog

* Improved Android Static Code Analysis speed (2X performance)
* Static Code analysis on Dexguard protected APK.
* Fixed a Security Issue - Email Regex DoS.
* Added Logging Code.
* All Browser Support.
* MIME Type Bug fix to Support IE.
* Fixed Progress Bar.

### v0.8.3 Beta Changelog
 
* View AndroidManifest.xml & Info.plist
* Supports iOS Binary (IPA)
* Bug Fix for Linux (Ubuntu), missing MIME Type Detection
* Check for Hardcoded Certificates
* Added Code to prevent from Directory Traversal

<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-160159852-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-160159852-1');
</script>
