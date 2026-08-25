# The intention of this project

vet is a dependency audit for PHP. A PHP developer uses it to read what a `composer update` puts into `vendor/`, one package at a time, and to record each tree that the developer trusts in a `vet.json` trust file.

Install the dependencies with `composer install`. Run the tests with `composer test`. Start the program with `./vet`.

- `app/` — the program: the commands, the actions, the value objects, the enums and the Composer plugin
- `bootstrap/` — the Laravel Zero application and its providers
- `builds/` — the executable `vet` that the package gives to a project
- `config/` — the configuration of the application and the list of the commands
- `tests/` — the tests, in Pest, with a project fixture for each shape of a trust file
