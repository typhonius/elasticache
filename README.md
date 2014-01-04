Requirements
------------
- The Amazon AWS SDK for PHP.

Installation
------------
- Set up your Elasticache Server

- Download the [http://aws.amazon.com/sdkforphp/](AWS SDK for PHP) to a location the webserver is able to access.
- The default location is /path/to/elasticache although this may be overridden by manually setting the $conf['elasticache_sdk_path'] in settings.php.

If the SDK is downloaded to sites/all/libraries/aws, set the configuration variable thus:

    $conf['elasticache_sdk_path'] = DRUPAL_ROOT . '/sites/all/libraries/aws';

Configuration
-------------
To connect to Elasticache, take the access key, secret key and region name obtained from the AWS account and place them in the settings.php of the site.

    $conf['elasticache_access_key'] = ACCESS_KEY;
    $conf['elasticache_secret_key'] = SECRET_KEY;
    $conf['elasticache_region_name'] = REGION_NAME;

Why use this Elasticache as a Drupal cache backend?
------------------------------------------------
