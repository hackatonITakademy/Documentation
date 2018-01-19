# Documentation utilitaires

## PHPStan


Installation : 
`composer require --dev phpstan/phpstan`

Utilisation : 
`vendor/bin/phpstan analyse DossToScan`

## PHPCodeSniffer
PHP_CodeSniffer detects violations of a defined coding standard

Installation : 
`composer require "squizlabs/php_codesniffer=*"`

Utilisation : 
`phpcs --report=json --extensions=php /path/to/code`

## PHPCodeBeautifier and Fixer
PHP Code Beautifier and Fixer fixes violations of a defined coding standard.

Installation : 
Installé en même temps que PHPCodeSniffer

Utilisation : 
`phpcbf --report=json --extensions=php /path/to/code`

