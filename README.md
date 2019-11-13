How to download this FORK package with versioning

You should add the following inside your composer.json:

```
{
  "repositories": [
    {
      "type": "package",
      "package": {
        "name": "safecharge/magento2-module-safecharge",
        "version": "VERSION THAT MATCH WHAT YOU WANT",
        "type": "package",
        "source": {
	  "url": "https://github.com/kstatua-alpenite/safecharge-magento-2-plugin.git",
          "type": "git",
	  "reference": "TAG OR BRANCH OF FORM" 
        }
      }
    }
  ],
  "require": {
    "safecharge/magento2-module-safecharge": "VERSION THAT MATCH WHAT YOU WANT"
  }
}
```

For example by changing "VERSION THAT MATCH WHAT YOU WANT" with "1.6.2" and running "composer update" it will update the current "TAG OR BRANCH OF FORM".

If you need to change branch that you need on your forked repo, you must change the "TAG OR BRANCH OF FORM" AND "VERSION THAT MATCH WHAT YOU WANT".


Sample test of this repo: 

```
{
  "repositories": [
    {
      "type": "package",
      "package": {
        "name": "safecharge/magento2-module-safecharge",
        "version": "1.6.2",
        "type": "package",
        "source": {
	  "url": "https://github.com/kstatua-alpenite/safecharge-magento-2-plugin.git",
          "type": "git",
		      "reference": "v1.6.2-dev" 
		    }
      }
    }
  ],
  "require": {
    "safecharge/magento2-module-safecharge": "1.6.2"
  }
}
```
