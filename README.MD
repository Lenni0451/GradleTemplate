# Gradle Template
A template project for my gradle based repos.

## Maven Server Setup
To use the maven servers in this template you need to enter your credentials into your `gradle.properties` files.\
The file can be found in the `.gradle` folder in your home directory (create it if it doesn't exist).
```properties
#Config for a Reposilite maven server
reposiliteUsername=user
reposilitePassword=123456

#Config for Sonatype
ossrhUsername=user
ossrhPassword=123456

#Config for the gradle plugin portal
gradle.publish.key=123456
gradle.publish.secret=123456
```

## Signing Setup
To sign your artifacts you need to enter your signing credentials into your `gradle.properties` files.\
The file can be found in the `.gradle` folder in your home directory (create it if it doesn't exist).
```properties
signing.keyId=ABC12345
signing.password=123456
signing.secretKeyRingFile=secretkey.gpg
```

The secretkey can be exported using the `gpg` command:
```bash
gpg --export-secret-key > secretkey.gpg
```
