Tracking Breaking changes in upcoming release

* Minimum required PHP version is now 7.1 (was 5.6) because explicit nullable parameter types (`?Type`) are used for PHP 8.4 compatibility.

Tracking Breaking changes in 1.0.0

* Removed `dataSerializer` parameter from `FileRextProxy` constructor.
* Option parameter type of `FileRestProxy::CreateFileFromContent` changed and added `setUseTransactionalMD5` method.
* Deprecated PHP 5.5 support.