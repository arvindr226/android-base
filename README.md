# android-base

This Docker registry will help you to make build.
This docker build will help you to make apk build using Continous Integration (Gitlab, jenkins, Bitrise etc )

For Example you want to make build of react-native code using this docker registry/image.
get in the react-native code.
<pre>
cd React-NativeApp
</pre>

Below command will make build of your react-native code.
<pre>
docker run -it --rm -v $PWD:/app -w /app arvindr226/android-base /bin/sh -c 'cd android && ./gradlew AssembleDebug'
</pre>

