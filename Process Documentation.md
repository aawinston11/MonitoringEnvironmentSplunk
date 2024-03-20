# Process Documentation

## 1. Log Ingestion and Baseline Establishment
- Objective: Upload historical logs from the Windows operating system and Apache web server to Splunk and establish baselines for normal system behavior.

- Steps:
1. Upload historical Windows logs to Splunk.
2. Upload historical Apache logs to Splunk.
3. Analyze the ingested logs to identify patterns and establish baselines for login activity, system usage, network traffic, HTTP response codes, top 10 domain referrers, and HTTP methods.


## 2. Report Creation
- Objective: Generate reports detailing key security metrics and insights derived from the ingested log data.

- Reports:
1. Windows LogIns: Report on successful and failed login attempts on the Windows operating system.
2. Apache HTTP Response Code: Report on the distribution of HTTP response codes from the Apache web server.
3. Top 10 Domain Referrers: Identify the top 10 domains referring traffic to the Apache web server.
4. HTTP Methods: Report on the distribution of HTTP methods (GET, POST, HEAD, etc.) used in requests to the Apache web server.

## 3. Alert Configuration
- Objective: Configure alerts within Splunk to proactively detect potential security threats and anomalous behavior.
- Alerts:
1. Configure alerts for detecting successful and failed logins on the Windows operating system.
2. Set up alerts for user account deletions to identify potentially malicious activity.
3. Create alerts for detecting high activity originating from outside the United States.
4. Configure alerts for detecting HTTP POST method usage on the Apache web server.

## 4. Baseline and Threshold Determination
- Objective: Utilize the ingested log data to establish baselines for normal system activity and define thresholds for alert triggers.

- Steps:

1. Analyze the ingested log data to determine typical system behavior.
2. Define thresholds for alert triggers based on deviations from the established baselines.

## 5. Dashboard Development
- Objective: Design interactive dashboards within Splunk to visualize key security metrics and facilitate rapid detection and response to potential threats.

- Steps:
1. Identify key security metrics and information to be included in the dashboards.
2. Design and configure interactive dashboards in Splunk to display login activity, alert summaries, severity levels of security events, HTTP response code distribution, top domain referrers, HTTP method distribution, and other relevant metrics.
