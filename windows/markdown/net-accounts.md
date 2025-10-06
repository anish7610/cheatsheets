## `net accounts` Command Overview

The `net accounts` command is used to manage user account policies on local or domain systems in Windows. It helps administrators set parameters such as password requirements and account lockout policies.

### Common Options

| Option                   | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `/minpwlen:length`       | Sets the minimum number of characters for a password.                       |
| `/maxpwage:days`         | Sets the maximum number of days a password is valid.                        |
| `/minpwage:days`         | Sets the minimum number of days that must pass before a password can be changed. |
| `/uniquepw:number`       | Ensures a user cannot reuse the same password until they have used the specified number of new passwords. |
| `/lockoutthreshold:attempts` | Specifies the number of failed logon attempts before the account is locked. |
| `/lockoutduration:minutes` | Sets the time (in minutes) an account remains locked after exceeding the logon attempts. |
| `/lockoutwindow:minutes` | Defines the time frame (in minutes) for counting failed logon attempts.     |

### Usage Examples

#### Set Minimum Password Length

```bash
net accounts /minpwlen:8
```

This command sets the minimum required password length to 8 characters.

#### Set Password Expiry to 30 Days

```bash
net accounts /maxpwage:30
```

This command ensures that passwords must be changed every 30 days.

#### Configure Account Lockout After 3 Attempts

```bash
net accounts /lockoutthreshold:3
```

This command locks the user account after 3 unsuccessful sign-in attempts.

#### Set Minimum Password Age to 1 Day

```bash
net accounts /minpwage:1
```

This command prevents users from changing their password more than once per day.

### Cheat Sheet

- Min password length: `net accounts /minpwlen:<number>`
- Max password age: `net accounts /maxpwage:<days>`
- Min password age: `net accounts /minpwage:<days>`
- Password history: `net accounts /uniquepw:<number>`
- Lockout threshold: `net accounts /lockoutthreshold:<attempts>`
- Lockout duration: `net accounts /lockoutduration:<minutes>`
