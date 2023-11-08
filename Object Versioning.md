#S3 #Storage 

Keeping the whole history of the file in [[S3]].

* All versions are kept in [[S3]],
* Great backup tool,
* Cannot be disabled, only suspended,
* Can be used in conjunction with [[Lifecycle management]],
* Supports [[Multi-Factor Authentication]]

> [!TIP] Version ID = null; means there were no changes to the file

> [!INFO] If a bucket is publicly accessible, the previous versions of the files inside of it are not available publicly
### Deleting a versioned file
When delete was initiated on a versioned file it adds a Delete Marker on top of the Version history of the file.
By removing the Delete Marker, we bring back the file.
### Related
[[Versioning]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7202718b-2595-4fb5-9c0f-62eedc9c7820/adf2b16c-32b2-41da-b605-c9c870b5bf3f/watch