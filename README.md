# Drones For Good

## Cloning & Installing

Run the following commands:

```
git clone https://github.com/CatalystCode/drones-for-good
cd drones-for-good
git submodule init
git submodule update
```

## Adding updates
You can work on each repo separately as you would any other repo.

You can also work on the submodules from this parent clone, and commit the changes:

```
cd drones-for-good-demo
git checkout master
git add .
git commit -m "changes made to..."
git push origin master
```

Once you include updates and push them, you need to update the refs on the parent repo:

```
git submodule foreach git pull origin master
git add .
git commit -m "sub modules updated"
git push origin master
```