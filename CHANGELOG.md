## [Unreleased]

## 0.3.1

### Fixed
- Login with mapped UID for new users
  [#4](https://spicyhub.de/spicy-web/nextcloud-user-ispconfig/issues/4) @quest

## 0.3.0

### Added
- Password change for ISPConfig Mailusers
  [#2](https://spicyhub.de/spicy-web/nextcloud-user-ispconfig/issues/2) @quest  
  Remote API user needs permission to *Customer Functions, Server Functions, E-Mail User Functions* to update mailuser passwords

### Changes
- Code refactoring, adds new intermediate abstract class for ISPConfig SOAP API handling

## 0.2.2 - 2018-11-20
### Added
- Add Changelog File
- appinfo: Multilingual description and php-soap dependency
- Possibility to set default preferences in other apps on users first login, see Readme
  [#3](https://spicyhub.de/spicy-web/nextcloud-user-ispconfig/issues/3) @quest

## 0.2.1 – 2018-11-17
### Added
- Set new users email in email settings, too
  @quest
- Check for php-soap, log error if not available
  @quest
- Add error handling and understandable messages in admin log for some soap errors
  @quest
  
### Fixed
- Fix error in mapping UID -> E-Mail
  @quest

## 0.2.0 – 2018-11-17
### Added
- Support UID to mail mapping with prefix, suffix or bare-name
  @quest

### Changed
- Delete all information added to DB on first login when user gets deleted
  @quest
- Recognize returning users from DB by UID or mail address
  [#1](https://spicyhub.de/spicy-web/nextcloud-user-ispconfig/issues/1) @quest

### Fixed
- Fix error in mapping UID -> E-Mail
  @quest

## 0.1.0 – 2018-11-13
### Added
- Autenticate users by ISPConfig 3 SOAP api
  @quest
- Global quota and group membership settings for new users
  @quest
- Possibility to set quota and group membership per domain
  @quest
- Possibility to restrict login to specific domains by whitelisting
  @quest