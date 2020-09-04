# Databus Resources
Resources for uploading data to the DBpedia Databus and installing DBpedia dockerized Apps.

## How to upload data to the Databus

### 1. Create your Databus account

Go to http://databus.dbpedia.org to create your account.

### 2. Create your WebID
Follow [instructions on how to create your WebID](https://github.com/dbpedia/webid)

### 3. Link you WebID to your Databus account
You must have a WebID and it must be linked to your DBpedia Databus account.

### 4. Install Maven
On MacOS use 'brew install maven'

### 5. Configure your pom.xml using the templates in this tutorial
Set your group, artefact and version metadata.  Configure the public download url for your data.

### 6. Validate
Run 'mvn validate' to check everything is configured properly.

### 7. Deploy
Run 'mvn deploy' to package your data for your server, and upload metadata to the Databus.  The actual data does not get copied to the Databus, and must remain accessible via the public download url set in your pom.xml.
