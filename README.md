# c226-xml-dtd-route-planning
building and validating xml + dtd, CSCI 226


Decision: Given an origin and destination, and then decide the best route, and report the distance.

Signals:
  1. Origin location (text)
  2. Destination Location (text)
  3. Distance value (numeric, miles/km)
  4. Route ID (unique identifier)
  5. Timestamp of when the route was created

Gaps: No information about traffic, road closures, or travel mode (driving/walking). Missing these reduces confidence in the distance being most accurate.

Risk: If wrong or stale, a user could take a longer path or miss critical updates (closed roads). At scale, this creates bad navigation results.

Stewardship: The XML + DTD files are stored in GitHub for this assignment. In real applications, routes should be refreshed often, retained briefly, and restricted to authorized systems for user privacy.

Data Domain: Primary: Route Planning.
Adjacent: Traffic Data, Weather.
