# Documentation of the Process with Laravel Herd

## Social Networks

- [Github](https://github.com/Yannx79)
- [Likedin](www.linkedin.com/in/yannick-yasuhiro-funes-chavez)

## Index
1. [Introduction](#1-introduction)
2. [Installation of Laravel Herd](#2-installation-of-laravel-herd)
3. [PHP Configuration](#3-php-configuration)
4. [Node.js Configuration](#4-nodejs-configuration)
5. [Troubleshooting](#5-troubleshooting)
6. [Version Checks](#6-version-checks)
7. [Conclusions](#7-conclusions)

---

## 1. Introduction
Laravel Herd is a powerful tool for managing local development environments. This documentation outlines the steps followed during the setup and use of Herd, including PHP and Node.js management and the complications encountered during the process.

---

## 2. Installation of Laravel Herd
1. Download Laravel Herd from [https://herd.laravel.com/windows](https://herd.laravel.com/windows).

---

## 3. PHP Configuration
Laravel Herd allows you to manage different PHP versions easily. Below are the steps:

### Switch PHP Version:
```bash
herd use <VERSION>
```
This sets PHP version 8.3 as the default for the current project.

### Verify Current Configuration:
```bash
php -v
```

Replace `<VERSION>` with the desired version number.

---

## 4. Node.js Configuration
Node.js is a common dependency in Laravel projects for frontend management. Use `nvm` to manage multiple versions of Node.js.

### List Installed Versions:
```bash
nvm list
```

### Switch to a Specific Version:
```bash
nvm use <VERSION>
```

### Uninstall a Version:
```bash
nvm uninstall <VERSION>
```

Replace `<VERSION>` with the desired version number.

---

### Verify Current Configuration:
```bash
nvm current
node -v
```

## 5. Troubleshooting
During the process, the following issues were encountered:

1. Environment Variable Conflicts: PHP paths were causing conflicts. These paths were deleted to resolve the issue.
2. Node.js Installation Conflict: There was a conflict between the standalone Node.js installation and the one installed with Laravel Herd. To resolve this, Node.js was uninstalled.

---

## 6. Version Checks
```bash
herd --version
php --version
laravel --version
composer --version
node --version
```

## 7. Conclusions
Laravel Herd simplifies local development by managing dependencies and configurations. However, it is crucial to check existing configurations to avoid conflicts. Documenting these processes ensures a helpful reference for future projects.

