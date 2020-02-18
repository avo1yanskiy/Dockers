#Authenticating to GitHub Packages#

docker login -u USERNAME -p TOKEN docker.pkg.github.com

#Publishing a package#

docker tag IMAGE_ID docker.pkg.github.com/OWNER/REPOSITORY/IMAGE_NAME:VERSION
docker push docker.pkg.github.com/OWNER/REPOSITORY/IMAGE_NAME:VERSION

#Installing a package#

docker pull docker.pkg.github.com/OWNER/REPOSITORY/IMAGE_NAME:TAG_NAME

