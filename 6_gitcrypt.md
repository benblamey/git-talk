## Git Crypt ## 

(ensure no other branches)

$ git branch

$ git crypt init

$ git crypt export-key ~/my-test-key

(if cloning, we need to get the key, and then git crypt unlock)

$ git checkout add_creds

echo "credentials.txt filter=git-crypt diff=git-crypt" > .gitattributes

echo "password:Passw0rd" > credentials.txt

git push origin add_creds

(go on github, make PR, look at binary file)

(discuss: when deploying, my build machine needs to de-crypt)