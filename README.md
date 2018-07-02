## git describe output Heroku Buildpack

This buildpack gets the output of `git describe` that was placed into an S3 bucket; it is to get
around the limitations of Heroku accessing the .git directory during the Heroku build process.

**This is a temporary solution** until we switch to proper Distillery releases which will have the tag
info baked into them!

### Configuration

Set `app_name` and `s3_releases_root` in the git_describe_output_buildpack.config file.
