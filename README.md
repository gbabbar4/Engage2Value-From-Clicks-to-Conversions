# **Engage2Value-From-Clicks-to-Conversions**
Predict customer purchase value using multi-session digital behavior data, including traffic sources, device details, browser types, and geographic indicators. The project uses machine learning to identify behavioral patterns and estimate user purchase potential for improved marketing and engagement strategies.

# **Dataset Description**

This dataset captures detailed session-level information from a large-scale digital commerce platform. Each row corresponds to a unique user session and includes data on user behavior, acquisition channels, device information, and geographical location.

Participants are expected to predict the purchaseValue, which represents the total amount spent during a given session.
Key Feature Categories

1. **<u>User Behavior & Session Metrics</u>**
        `totalHits`, `pageViews`, `totals.bounces`, `new_visits`, `totals.visits` : Indicators of user engagement and session activity.
        sessionNumber, sessionStart: Information related to session sequence and timing.

2. **<u>Device & Technical Attributes</u>**
        `deviceType`, `os`, `browser`, `screenSize`, `device.browserSize`, `device.language` : Details about the user's device and browsing environment.
        browserMajor, device.*: Encompasses a variety of device-level descriptors such as model, version, and screen specifications.
        gclIdPresent: Signals the presence of a Google Click ID used in ad tracking.

3. **<u>Traffic & Marketing Source</u>**
        `userChannel`, `trafficSource`, `trafficSource.medium`, `trafficSource.keyword`, `trafficSource.campaign` : Insights into how users arrived at the platform.
        `trafficSource.adwordsClickInfo.*`: Contains attributes from advertising sources, including ad network type and slot.
        `trafficSource.adContent`, `trafficSource.referralPath`, `trafficSource.isTrueDirect` : Provide further attribution details.

4. **<u>Geographical Context</u>**
        `geoNetwork.city`, `locationCountry`, `geoNetwork.continent`, `geoNetwork.subContinent`, `geoNetwork.metro`, `geoNetwork.region`
         : Geographic identifiers to help understand regional behavior trends.
        `geoCluster`, `locationZone` : Groupings based on geographic or behavioral patterns.

5. **<u>Identifiers</u>**
        userId, sessionId: Unique identifiers for each user and session, allowing for multi-session analysis.

6. **<u>Target Variable</u>**
        `purchaseValue` : The amount (in currency units) spent by the customer during the session. This is the target variable to be predicted.
