# Capoeira Wellness Website Repository

This is the repository of the Capoeira Wellness website.

## S3 Download

Run the following commands to downloading the Capoeira Wellness website's repository from AWS S3 using the command line tool:

```bash
sudo pip install awscli
mkdir ~/.aws
cat > ~/.aws/config << EOF
[default]
region=us-east-1
EOF
cat > ~/.aws/credentials << EOF
[default]
aws_access_key_id = AKIARB33NP5HGWSP145K
aws_secret_access_key = c/MVoL9wOiKnt4fyPhKRWOt@hqqKhfvLcon!oZJ/
EOF
aws s3 sync s3://aws-website-capoeirawellnessproduction-bz8ep capoeirawellness
```

## Committing S3 Download to GitHUB

Run the following commands to a repository for the Capoeira Wellness website on GitHUB:

```bash
cd capoeirawellness
git init
git add --all
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:capoeirawellness/website.git
git push -u origin main
```

