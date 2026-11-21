# Comrades Stocker Privacy Policy

**Effective date** November 21, 2026

## 1. Who we are and what this policy covers

Comrades Stocker (“Stockbot”) is an independent Blox Fruits fan project maintained by CruzXIIII. This policy describes how Stockbot handles information when you use the Discord bot, use the project-operated stock API, or contact the maintainer for support. For service rules and eligibility, see the [Terms of Service](TERMS_OF_SERVICE.md).

Discord handles your Discord account and use of its platform under its [Privacy Policy](https://discord.com/privacy). An independent operator who hosts a copy of Stockbot controls that installation and its data practices. Direct requests about a separately hosted copy to its operator.

## 2. Information we handle and how we use it

Most Stockbot features start when someone uses a slash command, selects a button, or requests autocomplete suggestions. Discord supplies the interaction and the account, server, channel, and permission information needed to handle it. Stockbot uses that context to answer in the correct place, apply server permissions, and associate saved choices with the correct account or server. Stockbot operates without reading ordinary channel messages, ordinary DMs to the bot, or voice conversations.

| Feature | Information we handle | Why we use it |
| --- | --- | --- |
| Stock lookups, trade comparisons, and other commands | Command and button inputs such as fruit names, dealer selections, display formats, and proposed trade items, together with the interaction context. | Return the requested information and handle command errors. |
| Personal fruit alerts | Discord user ID, selected fruit, registration time, relevant dealer rotation timestamps, and whether the alert is active or paused. | Match your fruit to a verified new rotation, send a one-time Discord DM, and manage delivery failures. |
| Beli savings goals | Discord user ID, selected fruit, and the Beli amount you choose to save. Beli is an in-game currency. | Show your saved amount and how much more Beli you need. A matching stock alert DM can include that calculation. |
| Restock guesses | Discord user and server IDs, selected dealer and fruit, submission and rotation timestamps, and the result. | Enforce one pick per dealer per round, score guesses against verified stock, and produce server results and leaderboards. |
| Server stock announcements | Server, configured channel, and role IDs, watchlists, display preferences, and delivery records such as rotation and retry times, delivery status, and errors. | Send and format announcements, mention configured roles when appropriate, retry failed posts, and prevent duplicates. |
| HTTP stock API | Network information made available by the connection, such as the connecting IP address, and the request path and headers. | Receive and answer the request. The project’s host or network infrastructure may log connection and request details. An error while handling a fruit request can record the request’s fruit value in diagnostic logs. |
| Diagnostics | Operational timestamps, errors, interaction IDs or error details, delivery records, and server, channel, or role IDs and names where relevant. | Keep the service running, investigate failures, and resolve support and security issues. |
| Support and privacy requests | Your email address or Discord account details, what you send us, and the information needed to identify the relevant records or verify a request. | Respond to you, investigate the issue, and handle your request. |

The public stock API provides game stock, catalog, countdown, and service health data without creating a Stockbot account or setting a tracking cookie. Stockbot’s game inventory history records dealer rotations and fruit availability from its stock data source. Personal alerts, savings goals, and restock guesses are optional. Share the fruit choices and in-game amounts needed for the feature you choose. Keep passwords, account tokens, and payment details out of commands and support messages.

## 3. Who can see information

- **Discord.** Stockbot uses Discord to receive interactions and to send message replies, configured role mentions, attachments, and DMs. Discord handles these deliveries on its platform. [Discord Privacy Policy](https://discord.com/privacy)
- **People with access to a Discord channel.** Public replies and automated posts can be seen by anyone who has permission to view that channel. Restock leaderboards show leading users and their win counts. A configured stock announcement channel can show a round’s results and identify some winning users. Your individual pick confirmation, personal results, and savings-goal responses are shown privately in Discord. Personal alert messages go to your Discord DMs.
- **Hosting providers.** The project uses Google Compute Engine to host the bot. Its infrastructure handles service requests, application storage, and operational data needed to run the hosted service. [Google Cloud Data Processing Addendum](https://cloud.google.com/terms/data-processing-addendum/)
- **Stock-data sources.** Stockbot requests game inventory from Blox Fruits Values or another configured stock source. Stockbot sends its own game inventory requests without forwarding your Discord account ID, alerts, goals, or guesses. If you visit Blox Fruits Values directly, the site handles that visit under its own policy. [Blox Fruits Values Privacy Policy](https://bloxfruitsvalues.com/privacy-policy)
- **Support communications.** Email and Discord DMs to the maintainer are handled through the communications service you use. Requests sent to the project’s Gmail address go through Google’s email service. [Google Privacy Policy](https://policies.google.com/privacy)
- **Legal and platform obligations.** Information may be disclosed to the extent required by applicable law or a valid legal request. Stockbot may also provide information to Discord as required under Discord’s developer terms, for example to report unauthorized access to Discord API data. [Discord Developer Terms of Service](https://support-dev.discord.com/hc/en-us/articles/8562894815383-Discord-Developer-Terms-of-Service)

Stockbot uses Discord data to operate the features described here. We do not sell Discord data or use it for advertising, profiling, or AI training.

## 4. Storage, retention, and security

| Record | How long it stays in use |
| --- | --- |
| Personal alerts | An alert stays active until you remove it or it is successfully sent. If Discord cannot accept the DM, it can remain saved in a paused state until you remove or re-enable it. |
| Savings goals | A saved goal remains available until you clear it or it is deleted following a request. Entering a new amount replaces the amount on file for that fruit. |
| Restock guesses | Results and leaderboards use guesses for rounds that closed in the previous seven days. Older guesses are excluded from results and pruned from saved data when the guess file is next successfully rewritten with current records. |
| Server settings and delivery records | Settings persist across restarts for as long as they are configured. Recent delivery state is kept separately to retry posts, prevent duplicates, and diagnose failures. Disabling announcements removes the configured destination. |
| Logs and support records | Retention depends on the type of record, what is needed to investigate or resolve an issue, and applicable storage or legal requirements. |

These controls apply to Stockbot’s own records. Messages already delivered in Discord are subject to Discord’s and the server’s message controls. Removing the bot from a server can stop its access there while previously saved settings, delivery records, personal preferences, and Discord messages remain subject to their respective retention rules.

The bot stores configured settings and saved feature state on its host, outside the public stock API. Google Cloud documents encryption at rest for data stored on Compute Engine disks. We access hosted records and correspondence to operate Stockbot, investigate service issues, and respond to support and privacy requests. Discord and Google Cloud may process data in locations that differ from where you live. [Compute Engine disk encryption](https://docs.cloud.google.com/compute/docs/disks/disk-encryption)

## 5. Your choices and privacy requests

- Use `/fruit-alerts list` to review active and paused alerts, `/fruit-alerts add <fruit>` to re-enable a paused alert, and `/fruit-alerts remove <fruit>` to cancel an alert.
- Use `/goal <fruit>` to review a goal, or set `clear` to `true` and leave `beli` blank to delete the saved goal for that fruit.
- If you manage a server, use `/stock-alerts disable` to remove the announcement destination, run `/stock-alerts role` without selecting a role to clear role mentions, and use `/watchlist remove <fruit>` to update the watchlist.
- Contact the maintainer to ask for access to, correction of, or deletion of information Stockbot stores about you, including restock guesses. Server administrators can also contact the maintainer about removing saved settings for their server.

Email [coksikhi55@gmail.com](mailto:coksikhi55@gmail.com) with the subject **Stockbot privacy request**, or send a private message to [@cruzxiiii_wikiman on Discord](https://discord.com/users/1290291783514980427). Describe the information or feature involved, the action you want, and your Discord user ID if known. For server requests, include the server ID and your role. We may ask for confirmation through your Discord account or confirm your authority to act before disclosing or changing information. Keep personal requests out of public channels and issue trackers.

We handle verified requests under applicable law and Discord’s developer terms, including prompt removal of Discord API data when required. Depending on where you live, you may also have rights to obtain a portable copy, restrict or object to certain processing, withdraw consent where processing relies on it, or complain to your local privacy regulator. For information held by Discord itself, use the controls and contact methods in the [Discord Privacy Policy](https://discord.com/privacy).

## 6. Children’s privacy

Stockbot is intended for users who are at least 13 years old and meet the minimum age for Discord in their country. If you are a parent or guardian and believe a child below the applicable age has provided information to Stockbot, use the privacy contact in Section 5 so the maintainer can investigate and remove information as appropriate. [Discord age requirements](https://discord.com/terms)

## 7. Changes to this policy

The current policy and its effective date will be published with the project documentation. We will update this notice when our data practices change and provide additional notice where required. For questions about any version of the policy, use the contact methods in Section 5.
