# Security Policy

## Overview

BTP Screen Control is a Windows desktop application designed to connect to and control Android devices locally.

The application does not require a cloud backend, remote database, or user account to provide its core functionality. Device connections are initiated by the user through supported local connection methods.

## Connection Security

BTP Screen Control may use USB debugging, Android Wireless Debugging, ADB Platform Tools, and the official scrcpy distribution.

Users should follow these precautions:

- Connect only Android devices they own or are authorized to control.
- Approve ADB authorization prompts only for trusted computers.
- Use Wireless Debugging only on trusted local networks.
- Disable USB Debugging or Wireless Debugging when no longer needed.
- Keep the application and its bundled third-party components up to date.

BTP Screen Control does not operate a remote-control server as part of its normal local device-control workflow.

## Supported Versions

Security reports are welcome for the latest published release of BTP Screen Control.

## Reporting a Security Vulnerability

Please do not publish sensitive vulnerability details, credentials, or exploit instructions in public GitHub Issues.

If private vulnerability reporting is enabled for this repository, use GitHub's **Report a vulnerability** feature to contact the maintainer privately.

If private reporting is unavailable, open a GitHub Issue requesting a private reporting channel without including sensitive technical details.

## Third-Party Components

BTP Screen Control uses third-party components, including ADB Platform Tools and scrcpy. These components are maintained by their respective projects and may have separate security advisories and license terms.

Please consult the relevant upstream projects for their security updates.
