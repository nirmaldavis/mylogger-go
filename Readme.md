A Sample Go module

go mod init github.com/nirmaldavis/mylogger-go

git init

git remote add origin https://github.com/nirmaldavis/mylogger-go.git

git add .

git commit -m "Initial commit"

git push --set-upstream origin master

git tag "v1.0.0"

git push --tags

If want to add to existing tag

) Delete and recreate the tag locally
	git tag -d {tagname}
	git tag {tagname}

) Delete and recreate the tag remotely
	git push origin :{tagname} // deletes original remote tag
	git push origin {tagname} // creates new remote tag
		
)  Update local repository with the updated tag (suggestion by @wyattis)
	git fetch --tags
