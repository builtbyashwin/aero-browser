# Privacy in Aero



Aero is designed for everyday privacy, not high-risk anonymity.



Its goal is to reduce unnecessary tracking and data collection while keeping the browser practical for normal use. Aero is based on ungoogled-chromium and aims to ship with Google telemetry removed, fingerprint resistance enabled by default, uBlock Origin built in, and DNS-over-HTTPS enabled by default.



## What Aero protects against



Aero is intended to reduce common forms of browser tracking, including:



- Advertising and analytics trackers

- Third-party tracking requests

- Browser telemetry and usage reporting

- Some browser fingerprinting techniques

- Plaintext DNS visibility on networks where DNS-over-HTTPS is used

- Unnecessary connections to Google services that are removed through the ungoogled-chromium base and Aero's patch set



Aero does not include privacy-hostile product features. The project does not include ads, affiliate links, cryptocurrency features, telemetry, VPN upsells, or AI features that send user data to a remote service.



## What Aero does not protect against



Aero is not an anonymity system.



It does not protect you from every form of tracking, surveillance, or compromise. In particular, Aero does not claim to protect against:



- A compromised operating system

- Malware, keyloggers, or other software already running on your device

- A malicious or compromised browser extension

- Websites you intentionally sign in to

- Tracking based on account identity or information you voluntarily provide

- Network-level observation of the fact that you are connecting to a particular IP address or service

- Advanced traffic analysis by an ISP, network operator, or other observer

- Browser or operating-system vulnerabilities

- Physical access to an unlocked device

- State-level adversaries or targeted surveillance



If you need strong anonymity against powerful adversaries, use a tool designed for that threat model, such as Tor Browser.



## DNS-over-HTTPS



Aero intends to enable DNS-over-HTTPS by default.



This prevents ordinary plaintext DNS queries from being visible to the local network or ISP DNS resolver. However, DNS-over-HTTPS does not make your browsing anonymous.



Your network provider can still observe connection metadata such as destination IP addresses, timing, and traffic volume. The DNS-over-HTTPS provider may also receive DNS queries, depending on the selected configuration.



DNS-over-HTTPS should therefore be treated as one privacy layer, not a complete protection against network surveillance.



## Fingerprinting



Aero aims to provide fingerprint resistance by default.



Browser fingerprinting combines characteristics such as screen size, fonts, browser features, graphics capabilities, language, time zone, and other signals to distinguish one browser from another.



Fingerprint resistance can reduce the uniqueness of these signals, but it cannot guarantee that every user will appear identical or that all fingerprinting techniques will fail.



Installing unusual extensions, changing uncommon settings, or using a distinctive system configuration may make a browser easier to identify.



## Telemetry



Aero's policy is simple: no telemetry.



The project does not intend to collect analytics, crash reports, usage statistics, browsing history, or background usage pings.



If a future feature requires sending user data to a remote service, that feature should not be added unless the project's privacy principles are explicitly reconsidered in public.



## Ads, affiliate links, crypto, and monetization



Aero does not include:



- Advertising

- "Acceptable ads"

- Affiliate links

- Cryptocurrency wallets or related features

- VPN upsells

- Sponsored content

- AI assistants that send user data to a server



These are product decisions, not optional privacy modes.



## What Aero will never do

Aero will never include:

- Advertising
- "Acceptable ads"
- Affiliate links
- Cryptocurrency wallets or related features
- VPN upsells
- Sponsored content
- Telemetry
- AI features that send user data to a server

These are project boundaries, not temporary product choices.

If any of these change, that change is a fork.
## Extensions



Browser extensions can weaken Aero's privacy protections.



An extension may be able to read page content, observe browsing activity, modify requests, or communicate with third-party services depending on the permissions it is granted.



Only install extensions you trust, and review their permissions before enabling them.



## Privacy tradeoffs



Privacy features can have costs.



Stronger blocking or fingerprint resistance may cause some websites to behave differently or break. DNS-over-HTTPS changes which resolver receives DNS queries. Disabling telemetry can reduce the amount of diagnostic information available when debugging crashes.



Aero's preference is to choose privacy by default while being clear about the resulting limitations.



## Threat model



Aero is intended for users who want stronger everyday browser privacy from common web tracking and unnecessary data collection.



It is not intended to defend against:



- A fully compromised device

- Highly targeted surveillance

- Powerful state-level adversaries

- An attacker with physical control of the device

- Anonymity correlation attacks



Aero should not be presented as a replacement for Tor Browser or other tools designed specifically for high-risk anonymity.



## Verifiability

Privacy claims should be verifiable in a shipped build.

Aero should make its privacy behavior auditable through:

- Reproducible builds where practical, so published binaries can be compared against source
- Auditable network behavior, so users and researchers can inspect what connections Aero makes by default
- Release notes that document changes to default network connections, telemetry behavior, and privacy-relevant features
- Clear separation between features that are implemented and features that are still planned

If a privacy claim cannot yet be verified in a released build, it should be labeled as aspirational rather than presented as an implemented guarantee.
## Honest limitations



Aero is still in its founding phase and is not finished.



Privacy claims should match what is actually implemented and verifiable in the current build. Planned features should not be described as complete until they are shipped and testable.



If Aero cannot protect against something, the documentation should say so clearly.
## Reporting privacy issues

If you find unexpected network traffic, a privacy leak, telemetry, or any request that should not be present, open an issue in the Aero repository with as much detail as possible.

Privacy regressions should be treated with the same seriousness as security bugs.

Include reproduction steps, affected versions, relevant logs or network traces, and any other information that helps verify the issue.
