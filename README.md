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

## PHP Parallel Lint
This tool checks syntax of PHP files faster than serial check with a fancier output.

Installation : 
`composer require --dev jakub-onderka/php-parallel-lint`

Utilisation : 
`vendor/bin/parallel-lint --exclude vendor --json /path/to/code`

## Psalm
Psalm is a static analysis tool for finding errors in PHP applications.

Installation : 
`composer require --dev vimeo/psalm`

Utilisation : 
`./vendor/bin/psalm --init /path/to/code`
`./vendor/bin/psalm`

## PHP Copy/Paste Detector (PHPCPD)
Copy/Paste Detector (CPD) for PHP code.

Installation :
Already installed with PHPQA

Utilisation : 
`vendor/bin/PHPCPD /path/to/code`

