Sites
=============

See http://getcomposer.org/doc/articles/handling-private-packages-with-satis.md#setup

## satis.json

	{
	    "name": "My Repository",
	    "homepage": "http://packages.example.org",
	    "repositories": [
	        { "type": "vcs", "url": "http://github.com/mycompany/privaterepo" },
	        { "type": "vcs", "url": "http://svn.example.org/private/repo" },
	        { "type": "vcs", "url": "http://github.com/mycompany/privaterepo2" }
	    ],
	    "require-all": true
	}


## Usage


	{
	    "repositories": [ { "type": "composer", "url": "http://packages.example.org/" } ],
	    "require": {
	        "company/package": "1.2.0",
	        "company/package2": "1.5.2",
	        "company/package3": "dev-master"
	    }
	}
