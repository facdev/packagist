packagist
=========


### packages

	{
	    "packages": {
	        "vendor/package-name": {
	            "dev-master": { @composer.json },
	            "1.0.x-dev": { @composer.json },
	            "0.0.1": { @composer.json },
	            "1.0.0": { @composer.json }
	        }
	    }
	}


### packages type

	{
	    "repositories": [
	        {
	            "type": "composer",
	            "url": "http://packages.example.com"
	        },
	        {
	            "type": "composer",
	            "url": "https://packages.example.com",
	            "options": {
	                "ssl": {
	                    "verify_peer": "true"
	                }
	            }
	        },
	        {
	            "type": "vcs",
	            "url": "https://github.com/Seldaek/monolog"
	        },
	        {
	            "type": "pear",
	            "url": "http://pear2.php.net"
	        },
	        {
	            "type": "package",
	            "package": {
	                "name": "smarty/smarty",
	                "version": "3.1.7",
	                "dist": {
	                    "url": "http://www.smarty.net/files/Smarty-3.1.7.zip",
	                    "type": "zip"
	                },
	                "source": {
	                    "url": "http://smarty-php.googlecode.com/svn/",
	                    "type": "svn",
	                    "reference": "tags/Smarty_3_1_7/distribution/"
	                }
	            }
	        }
	    ]
	}
	
### repo for bitbucket.org

	{
	    "require": {
	        "vendor/my-private-repo": "dev-master"
	    },
	    "repositories": [
	        {
	            "type": "vcs",
	            "url":  "git@bitbucket.org:vendor/my-private-repo.git"
	        }
	    ]
	}
	

### PEAR

	{
	    "repositories": [
	        {
	            "type": "git",
	            "url": "https://github.com/foobar/intermediate.git"
	        },
	        {
	            "type": "pear",
	            "url": "http://pear.foobar.repo",
	            "vendor-alias": "foobar"
	        }
	    ],
	    "require": {
	        "foobar/TopLevelPackage1": "*",
	        "foobar/TopLevelPackage2": "*"
	    }
	}
	
