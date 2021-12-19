# cState Site v5.0.5

This is the default cState status page website directory/folder.

* Example site repository link (you are here): https://github.com/cstate/example
* Main cState source code repository: https://github.com/cstate/cstate

## Are you updating? Use these commands

Download your site with all the directories. `git clone --recursive <your repo link goes here>`

![IMG_20211219_105139](https://user-images.githubusercontent.com/73424060/146664973-1044dde6-520b-4c37-a506-e690f518ace6.jpg)


Update the cState theme submodule. `git submodule foreach git pull origin master`

![IMG_20211219_105201](https://user-images.githubusercontent.com/73424060/146664994-0f0402a7-0281-4c25-acb3-7cd793be6ac6.jpg)


In the parent directory, type `hugo serve`. Check to see if everything is working.

Then do `git add -A; git commit -m "Update cState"; git push origin <branch, probably main or master>`. Your status page is now updated and uploaded.

![IMG_20211219_105220](https://user-images.githubusercontent.com/73424060/146665004-1a805aea-b4e2-4db1-b74b-4894425ed11e.jpg)



## For maintainers (probably not for you)

Maintainers need to update both cstate/cstate and cstate/example for each new version.

Download this repo with all the directories. `git clone --recursive -b master https://github.com/cstate/example.git`

Add your changes from cstate/cstate's exampleSite folder.

Update the cState theme submodule. `git submodule foreach git pull origin master`

Then push `git add -A; git commit -m "Update cState vX.X.X"; git push origin master`.

## License

MIT © Mantas Vilčinskas
