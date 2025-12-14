## 🚀 Drupal 11 Installation (DDEV)

This project uses **DDEV** for local development. Follow the steps below to get the site up and running.

### 1. Prerequisites

Make sure you have the following tools installed:

- Docker
- DDEV
- Composer

👉 https://ddev.readthedocs.io/en/stable/#installation

### 2. Clone the Repository

```bash
git clone <REPOSITORY_URL>
cd <PROJECT_DIRECTORY>
```

### 3. Start the DDEV Environment
```bash
ddev start
```

### 4. Install PHP Dependencies
```bash
ddev composer install
```

### 5. Import DB
```bash
ddev import-db --file=path/to/database.sql
```

### 6. Copy Files to `web/sites/default`

### 7. Import configuration
```bash
ddev drush cim -y
```

### 8. Clear cache
```bash
ddev drush cr
```

### 9. Access the Site
```bash
ddev launch
```
Go to /user/login

Or generate a one-time login link
```bash 
ddev drush uli
```
