# MongoDb Installation

## Mac

**Install home brew**
It is a package manager for mac
go to home page of [Home Brew](https://brew.sh/)
copy following line from site

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

and past it to terminal

**Install node**

```bash
brew install node
```

**Install mongo**

```bash
brew install mongo
```

**run mongod command**
this command will give error initialy.

```bash
mongod
```

we have to create `/data/db` directory.

```bash
sudo mkdir -p /data/db
```

this directory will be read-only so we need to change permissions

```bash
whoami // to get username to give permission
sudo chown -Rv nirav /data/db
```

now you can run mongodb

```bash
mongod // this needs to up and running
mongo // run on new terminal
```

install services so that we don't have to run above commands again and again

```bash
brew services start mongo
```
