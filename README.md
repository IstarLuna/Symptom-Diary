# Offline Symptom Diary

A personal iOS diary for recording symptoms, moods, body areas, medications, activities, water intake, and period history. Customizable Quick Logs make recurring entries easy, while calendars, charts, body heat maps, and reports help you review what you have recorded.

## Privacy & security

This information describes the current implementation. It should be reviewed whenever storage, sharing, or networking features change.

### Your diary stays on your device

- Diary records are stored locally using Core Data. The app does not upload or synchronize your diary to a developer-operated service or CloudKit.
- No app account is required. The current app contains no advertising or third-party analytics integration.
- Charts, summaries, and period estimates are calculated on your device.
- Hosting this project's source code on GitHub does not upload the diary stored on your phone.

### Protection at rest

The persistent diary database is configured with Apple's **Complete Data Protection** (`NSPersistentStoreFileProtectionKey` with `FileProtectionType.complete`). iOS manages the database's encryption and access when the device is locked.

Use a strong device passcode and keep iOS updated. This protection depends on the device's security and does not constitute a separate app password, custom encryption system, or guarantee against every form of access. It applies to the diary database; it is not a claim that every preference or exported file has the same protection.

### Device backups

Local storage does not mean that no copies can leave the phone. Depending on your settings, iCloud device backups or computer backups may include app data. Their storage and protection are controlled by the backup service and your device settings. Review those settings if you want to restrict where copies are kept.

### Exports and sharing

You choose when to export PDF reports, CSV data, or a restorable JSON backup and where to send or save them. These files may contain sensitive, identifiable health information.

Symptom Diary does not add password protection or encryption to exported files. Once shared or saved elsewhere, those copies are outside the app's control. Protection depends on the destination and recipient. Deleting an entry inside the app does not remove copies already exported or backed up.

The app displays a sensitive-data warning before export. Share only the information you intend to disclose, check the destination, and remove copies you no longer need.

### Your controls

You can review, edit, and delete recorded entries. The More screen provides history-management, export, and backup/restore tools. Restoring a backup replaces the current diary data; review the in-app confirmation before proceeding.

The privacy and security notice is shown for acknowledgment and remains available under **More → Privacy & Security**.

### External links

Opening an external guidance link takes you to a third-party website. That website's own privacy practices apply to your visit.

## Tracking and estimates

Symptom Diary is a personal tracking tool. It does not diagnose conditions, provide medical advice, monitor emergencies, or replace professional care. Historical trends describe recorded entries and do not establish causes or medical relationships.

Period estimates use confirmed start dates and recent cycle history. Suggested starts derived from older flow logs require review and confirmation. Estimates can be inaccurate, especially with missing entries or changing cycles. Displayed historical ranges are not probability-based confidence intervals. The app does not predict fertility or ovulation.

## HIPAA

Symptom Diary is not represented as a HIPAA-compliant service. Organizations considering its use in a regulated workflow are responsible for an independent legal and security review, including how exported information is handled.

Further information: [HHS resources about health apps and HIPAA](https://www.hhs.gov/hipaa/for-professionals/special-topics/health-apps/index.html).

## Reporting issues

When reporting a problem, describe what happened and the steps that led to it. Do not include personal health records, diary exports, or unredacted screenshots in GitHub issues. Review diagnostic information before sharing it.
