# evergreen-java-system-function

This buildpack is intended to override the `SPRING_CLOUD_FUNCTION_LOCATION` to the expected `jar` output of the `heroku/java-buildpack` in `/workspace/target/*built.jar*` during launch.

This is required by the riff java buildpack in order for the riff java invoker to classload the function.
