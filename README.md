composer init composer require johnpbloch/wordpress git init

composer.json

"repositories":[ { "type":"composer", "url":"https://wpackagist.org", "only": [ "wpackagist-plugin/", "wpackagist-theme/" ] } ], "extra": { "installer-paths": { "wordpress/wp-content/mu-plugins/{$name}/": [ "wpackagist-plugin/akismet" ], "wordpress/wp-content/plugins/{$name}/": [ "type:wordpress-plugin" ], "wordpress/wp-content/themes/{$name}/": [ "type:wordpress-theme" ] } },

.gitignore vendor wordpress

composer require wpackagist-plugin/wordpress-seo composer require wpackagist-theme/astra