# Screenshot checklist

The repository is designed to work without screenshots initially, but these images will make the two reading paths much stronger.

## Images to add

### `form-overview.png`

**Audience:** non-technical / hiring manager

Capture the top of the live Jotform showing:

- form title;
- demo/data-use notice;
- first few job fields.

Do not include browser/account UI that reveals personal account information.

### `conditional-no-issue.png`

**Audience:** non-technical

Show the form after:

- Installation completed = Yes
- Issue identified = No

The point of the image is to demonstrate the short, uncluttered path.

### `conditional-issue.png`

**Audience:** non-technical

Show the form after:

- Issue identified = Yes
- Severity = Urgent

The screenshot should make the progressive disclosure obvious.

### `make-scenario.png`

**Audience:** technical

Capture the full Make scenario so the viewer can see:

```text
Custom Webhook -> Parse JSON -> Router -> Urgent / Not urgent markers
```

### `routing-filter.png`

**Audience:** technical

Show the Urgent route filter with the severity comparison visible:

```text
q13_issueSeverity = Urgent
```

### `routing-test.png`

**Audience:** technical

Show successful execution evidence demonstrating the selected route.

If one screenshot cannot show both tested branches clearly, use two images:

- `routing-test-urgent.png`
- `routing-test-not-urgent.png`

## Redaction / safety checklist

Before adding any screenshot to GitHub, check every visible area for:

- webhook URLs or tokens;
- API keys or credentials;
- email addresses or usernames;
- IP addresses;
- account identifiers;
- Jotform or Make private IDs that do not need to be public;
- browser bookmarks, tabs or notifications containing private information;
- real names, customer information, addresses or uploaded files;
- any employer/company name or branding connected to the job application that prompted the exercise.

Use only fictional demonstration data.

## Suggested placement

The recruiter-facing `README.md` should use:

1. `form-overview.png`
2. `conditional-no-issue.png`
3. `conditional-issue.png`
4. `make-scenario.png` or a cropped high-level version
5. `routing-test.png`

The technical walkthrough can reuse the Make images and add the detailed routing-filter screenshot.
