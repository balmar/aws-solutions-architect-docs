Process of tracking changes by adding a new version for each time a file or other versioned thing is updated.
In [[AWS]] the first version has [[VersionID]] = null. Other versions use [[UUID]] hash code.
When the versioned file is deleted. Instead of erasing the file from system, a delete marker is applied.