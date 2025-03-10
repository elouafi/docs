---
title: "LTS, MTS, and Monthly Releases"
url: /releasenotes/studio-pro/lts-mts/
category: "Studio Pro"
weight: 1
---

## 1 Introduction

The goal of this document is to clarify Mendix Studio Pro version options and help you decide which version to run your applications on.

To understand the different types of versions and releases, consider the example of Studio Pro version  [8.18.1](/releasenotes/studio-pro/8.18/#8181) and see the sections below.

### 1.1 Major Version {#major-version}

In the 8.18.1 example, the first number (**8**) indicates the major version.

Mendix supports three major versions at a time. To clarify our current offering and in relation to our SLA, today Mendix supports major versions 7, 8, and 9. Once version 10 has been released, version 7 will only be supported via the Extended Support product.

As of Mendix 10, to make planning version upgrades easier for our users, Mendix will release in a two-year cadence, which means that every two years we plan to release a new major version in June. This will help in preparing and planning to adopt new releases and upgrade older Mendix versions. Each major version release will start with two Beta releases.

For Mendix 10 and 11, we are planning to follow this release timeline:

| Release | Date |
| --- | --- |
| 9.24 LTS | March 2023 |
| 10 Beta 1 | April 2023 |
| 10 Beta 2 | May 2023 |
| 10.0 GA | June 2023 |
| 10.6 MTS | December 2023 |
| 10.12 MTS | June 2024 |
| 10.18 MTS | December 2024 |
| 10.21 LTS | March 2025 |
| 11 Beta 1 | April 2025 |
| 11 Beta 2 | May 2025 |
| 11.0 GA | June 2025 |

### 1.2 Minor Version

In the 8.18.1 example, the second number (**18**) indicates the minor version. 

A minor version is generally released every month. It includes new features and fixes, but it does not include breaking changes.

### 1.3 Patch Version

In the 8.18.1 example, the third number (**1**) indicates the patch version. 

A patch version is released on an as-needed basis. It includes security fixes and critical bug fixes, but it does not include new features or breaking changes.

## 2 Long-Term Support Version (LTS) {#lts}

An LTS version is the latest minor version before a new major version is released for General Availability. Once a minor version becomes an LTS, it will not have new features added to it. 

These are the current LTS versions of Studio Pro:

* [9.24](/releasenotes/studio-pro/9.24/) (started in March, 2023)
* [8.18](/releasenotes/studio-pro/8.18/) (started in March, 2021)
* [7.23](/releasenotes/studio-pro/7.23/) (started in February, 2019)

Mendix advises using LTS versions for all production apps, as LTS versions of Studio Pro enjoy the highest security and stability. LTS versions also have the longest support duration compared to other versions.

### 2.1 Support Duration

Support for an LTS version ends when a third consecutive major version is released for General Availability (for example, support on version 6 ended with the GA release of version 9).

This diagram illustrates the LTS concept with version and [end of support](#end) examples:

{{< figure src="/attachments/releasenotes/studio-pro/lts-mts/lts.png" >}}

{{% alert color="info" %}}For details on extending support for an older major version, see the [Extended Support](/developerportal/support/#extended-support) section in *Mendix Support*.{{% /alert %}}

### 2.2 Release Cycle

An LTS starts with the release of a new higher major version for General Availability. For a description of Mendix’s major release cadence, see the [Major Version](#major-version) section above.

For an LTS version, there will only be [patch](#patch) releases on an as-needed basis.

### 2.3 Support with Patch Releases

For the support duration, the LTS will receive patch releases only. 

### 2.4 Upgrading Impact

The impact of upgrading from an LTS to an LTS is often the lowest of these options. That is because an LTS has the longest support duration and only gets critical fixes, which results in high stability over time. In addition, depending on how rigorous your application update/release process is, the upgrade would only have to be done once, as opposed to multiple times between MTS versions or monthly release versions.

## 3 Medium-Term Support Version (MTS) {#mts}

An MTS is a minor version released approximately every 6 months after a new major version release for General Availability.

These are the current MTS versions for Studio Pro:

* [9.18](/releasenotes/studio-pro/9.18/) (started in September, 2022)
* [9.12](/releasenotes/studio-pro/9.12/) (started in March, 2022)
* [9.6](/releasenotes/studio-pro/9.6/) (started in September, 2021)

{{% alert color="info" %}}
Older MTS versions (for example, 9.6) remain supported until the next major version has been released for General Availability (for example, 10).
{{% /alert %}}

If you are on an innovation track with your development and need to get the latest and greatest Mendix has to offer every month, then upgrade to an MTS and stay on that version with its patch releases until the next MTS version is released.

### 3.1 Support Duration

The support duration for an MTS depends on when a new higher major version is released for General Availability, which thus creates a new LTS and ends support for all MTS versions for that respective major version.

### 3.2 Release Cycle

MTS versions are introduced as minor versions approximately every 6 months after a new major version release for General Availability. There will only be patch releases for an MTS on an as-needed basis.

### 3.3 Support with Patch Releases

For the support duration, the MTS will receive patch releases only.

### 3.4 Upgrading Impact

The impact of upgrading between MTS versions is higher than upgrading between LTS versions. That is because an MTS has a shorter support duration than an LTS, which means it has less time to become as stable as an LTS version. In addition, the upgrade has to be done approximately every six months.

## 4 Monthly Release Version {#patch}

A monthly release is a a non-MTS/LTS minor release that only receives patches for critical/security issues if they can be released earlier and faster than the next minor version release.

### 4.1 Support Duration

Monthly release versions do not enjoy regular patch releases like MTS and LTS versions do. Bugs found in monthly release versions are directly resolved in the subsequent monthly release. 

For example, if a bug is found in version 9.1, it will only be fixed in the next monthly release, which would be version 9.2.

### 4.2 Release Cycle

This is a monthly release that includes new features as well as security patches that are applied to existing MTS and LTS versions.

### 4.3 Support with Patch Releases

A monthly release only receives patches for critical/security issues if they can be released earlier and faster than the next minor version release. Otherwise, bugs found in a monthly release will only be fixed rolling forward to the next minor version. 

For example, if you are using version 9.1 after 9.2 has been released and you find a critical issue in 9.1, that fix will only be released in the next monthly release, which would be 9.3.

If a bug is found in a monthly-release version for an older major version, it will only be fixed as a patch on the existing LTS (for example, a bug found in 8.16 will only be fixed for a patch release on the LTS version 8.18). 

### 4.4 Upgrading Impact

The impact of upgrading between monthly releases is the highest of these options. That is because every month, all new features are shipped in such minor versions, including all bug fixes and security patches. In addition, the upgrade has to be done monthly, which can be a significant drain on resources.

## 5 End of Support {#end}

The "end of support" for a version means that fixes, updates, investigating, troubleshooting, and other forms of assistance are no longer provided.

If a new major version is nearing release, that means an older major version is nearing its end of support. If you are still using a major version for which support will end, Mendix recommends that you stop using that version and move to a newer LTS version that is supported. 

Furthermore, you should uninstall old versions for which support has ended. If you continue to use versions for which support has ended, you do so at your own risk for your applications, data, and security. Mendix does not recommend using versions for which support has ended unless you have purchased the [Extended Support](/developerportal/support/#extended-support) product.
