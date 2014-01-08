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
