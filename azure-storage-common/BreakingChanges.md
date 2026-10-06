Tracking Breaking changes in upcoming release

* Minimum required PHP version is now 7.1 (was 5.6) because explicit nullable parameter types (`?Type`) are used for PHP 8.4 compatibility.

Tracking Breaking changes in 1.0.0

* Removed `ServiceBuilder.php`, moved static builder methods into `BlobRestProxy`, `TableRestProxy`, `QueueRestProxy` and `FileRestProxy`.
* Moved method `SharedAccessSignatureHelper::generateBlobServiceSharedAccessSignatureToken()` into `BlobSharedAccessSignatureHelper`.
* Moved method `SharedAccessSignatureHelper::generateTableServiceSharedAccessSignatureToken()` into `TableSharedAccessSignatureHelper`.
* Moved method `SharedAccessSignatureHelper::generateQueueServiceSharedAccessSignatureToken()` into `QueueSharedAccessSignatureHelper`.
* Moved method `SharedAccessSignatureHelper::generateFileServiceSharedAccessSignatureToken()` into `FileSharedAccessSignatureHelper`.
* `CommonMiddleWare` constructor requires storage service version as parameter now.
* `AccessPolicy` class is now an abstract class, added children classes `BlobAccessPolicy`, `ContainerAccessPolicy`, `TableAccessPolicy`, `QueueAccessPolicy`, `FileAccessPolicy` and `ShareAccessPolicy`.
* Deprecated PHP 5.5 support.