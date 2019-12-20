# Rails App


## Getting started

```bash
  # Start the dev environment
  ./auto/dev

  # Run Rails
  ./run.sh

  # The first time you will also have to run the following...
  # ctrl-z to have it rails run in the background

  rake db:create
  # (this creates db files in .tmp folder which is not checked into git)

  #Visit http://localhost:3000
```

## Steps to Initially setup Rails (can redo if required from commit 67bd5d2604444b8e5ade2d12ebfb2d68feafa110)

```bash
  bundle exec rails new . --force --no-deps --database=postgresql

  # Update config/database.yml
  # as per https://docs.docker.com/compose/rails/

  ./run.sh
  # (^ and then ctrl-z to have it run in the background)

  rake db:create
```
