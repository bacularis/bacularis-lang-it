# Bacularis translations into Italian

This is repository with files that provide the Italian translations
for the Bacularis web interface and the Bacularis API panel.

The files in this repository are part of Bacularis.

## General

Translation files have been translated with help of AI technology and they can
contain language errors.

## Installation

### Step 1 - create directories for new translation files

The command form to create the language directories is following:

```
mkdir -p {PROJECT_DIR}/protected/vendor/bacularis/bacularis-api/API/Lang/it/
mkdir -p {PROJECT_DIR}/protected/vendor/bacularis/bacularis-web/Web/Lang/it/
```

where:

 * ``{PROJECT_DIR}`` - is the main Bacularis directory.

If you installed Bacularis using binary packages, they are the following commands:

```
mkdir -p /usr/share/bacularis/protected/vendor/bacularis/bacularis-api/API/Lang/it/
mkdir -p /usr/share/bacularis/protected/vendor/bacularis/bacularis-web/Web/Lang/it/
```

### Step 2 - copy translation files to Bacularis

Copy files from this repository to Bacularis:

```
cp ./API/messages.mo {PROJECT_DIR}/protected/vendor/bacularis/bacularis-api/API/Lang/it/
cp ./Web/messages.mo {PROJECT_DIR}/protected/vendor/bacularis/bacularis-web/Web/Lang/it/
```

where:

 * ``{PROJECT_DIR}`` - is the main Bacularis directory.

If you installed Bacularis using binary packages, they are the following commands:

```
cp ./API/messages.mo /usr/share/bacularis/protected/vendor/bacularis/bacularis-api/API/Lang/it/
cp ./Web/messages.mo /usr/share/bacularis/protected/vendor/bacularis/bacularis-web/Web/Lang/it/
```

### Step 3 - set new language in Bacularis

Change the language code in the following configuration files below. Both contain
an option ``lang`` that you need to set to ``it``:

```
{PROJECT_DIR}/protected/vendor/bacularis/bacularis-api/API/Config/api.conf
{PROJECT_DIR}/protected/vendor/bacularis/bacularis-web/Web/Config/settings.conf
```

If you installed Bacularis using binary packages, they are the following paths:

```
/usr/share/bacularis/protected/vendor/bacularis/bacularis-api/API/Config/api.conf
/usr/share/bacularis/protected/vendor/bacularis/bacularis-web/Web/Config/settings.conf
```

### Step 4 - log out and log in

New language setting will start working after logging out and loggin in. Please log out
from the web interface and then log in.

## Important notes

This new language is not listed in the language list on the web interface. If you save
language settings on the web interface, the language will be switched to the currently
selected language on the web interface.
