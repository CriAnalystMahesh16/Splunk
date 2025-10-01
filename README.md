# Splunk
Zero to Hero Splunk
📅 Splunk Daily Plan (Zero to Hero)
Week 1: Foundations

Goal: Install Splunk, understand core concepts.

Day 1: What is Splunk? Use cases in IT & Security. Install Splunk Free. Explore Splunk Web GUI.

Day 2: Learn Index, Sourcetype, Host. Ingest sample logs. Run your first search (index=_internal).

Day 3: Explore Splunk Web layout (Search app, Reports, Dashboards).

Day 4: Basic search commands (search, fields, table, stats).

Day 5: Filtering data (where, eval, sort).

Day 6: Field extraction basics (auto + regex).

Day 7: Mini project → Load Apache Web Server logs. Search for top 5 IPs.
Week 2: SPL Mastery

Goal: Get fluent in Search Processing Language.

Day 8: Learn stats (count, avg, sum).

Day 9: Use timechart & chart for trends.

Day 10: Create dashboards (single values, pie charts, line graphs).

Day 11: Use rex to extract custom fields.

Day 12: Learn eval for calculated fields.

Day 13: Alerts & scheduled searches.

Day 14: Mini project → Build a dashboard showing error rates + login attempts over time.


Week 3: Splunk for Security

Goal: Apply Splunk to detect threats.

Day 15: Install Splunk Security Essentials App.

Day 16: Detect failed SSH logins ("Failed password").

Day 17: Correlation search: brute-force attack (5 failed logins in 1 min).

Day 18: Monitor Windows Event Logs (logon events).

Day 19: Create alerts for suspicious admin logins.

Day 20: Use Threat Intelligence feeds (IOCs).

Day 21: Mini project → Build a SIEM dashboard with failed logins, successful logins, and alerts.

Week 4: Admin + Advanced

Goal: Learn Splunk Admin & scale knowledge.

Day 22: Universal vs Heavy Forwarder.

Day 23: Indexer basics & data lifecycle (hot, warm, cold, frozen).

Day 24: Role-based access control.

Day 25: Distributed Splunk: Search Head, Indexer, Forwarder.

Day 26: Splunk Cloud vs Enterprise.

Day 27: Performance tuning (indexing, filtering data before indexing).

Day 28: Mini project → Simulate a distributed setup with one forwarder + one Splunk instance.
Final 2 Days: Career Prep

Day 29: Review all commands. Do a 1-hr self-test (search queries + dashboards + alerts).

Day 30: Explore Splunk certifications (Power User, Admin). Prepare CV with a Splunk Security Project.

------------------------------------------------------------------------------------------------------------------------


Why Splunk Was Invented?

Before Splunk (early 2000s), IT teams had a huge problem:

Every server, application, network device, and security tool produced logs (machine data).

These logs were often unstructured (different formats, plain text, no order).

To troubleshoot an issue, engineers had to manually open log files, search with grep/find, and hope they spotted the error.

In large companies with hundreds of servers, this became nearly impossible.

💡 So in 2003, three engineers (Michael Baum, Rob Das, Erik Swan) built Splunk to act like Google for logs:

Collect machine data from many sources.

Index it (like a search engine).

Let you run fast searches in real-time.

By 2005, Splunk became popular because it made IT operations and security analysis much faster. Today it’s a leader in SIEM (Security Information & Event Management).

🔹 How Splunk Works (Simple View)

Think of Splunk in 3 steps:

Data Ingestion

Logs, events, metrics from servers, firewalls, applications, IoT devices, etc.

Example: Apache access logs, Windows Event Logs, Linux syslogs.

Indexing

Splunk stores this data in special buckets (hot, warm, cold).

Each event gets a timestamp and metadata (host, source, sourcetype).

Searching & Visualization

You use SPL (Search Processing Language) to query data.

Results can be shown as tables, charts, dashboards, or alerts.

Splunk Architecture (Core Components)

Forwarder: Small agent installed on source machines to send data to Splunk.

Indexer: Stores and indexes the data (the brain).

Search Head: Provides the UI where you search, make dashboards, and run reports.

👉 In small setups, one machine can be all three. In enterprises, they are distributed.



