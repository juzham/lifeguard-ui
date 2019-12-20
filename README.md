# Rails App


## Getting started

```bash
  # Start the dev environment
  ./auto/dev

  # Run Rails
  ./run.sh
```

## Steps to Initially setup Rails

```bash
  bundle exec rails new . --force --no-deps --database=postgresql

  # Update config/database.yml
  # as per https://docs.docker.com/compose/rails/

  ./run.sh

  rake db:create
```
