node {
	git "$SCM_URL"
	sh "wget 'https://repo.maven.apache.org/maven2/io/spring/nohttp/nohttp-cli/0.0.3.RELEASE/nohttp-cli-0.0.3.RELEASE.jar' -O nohttp.jar"
	withEnv(["JAVA_HOME=${ tool 'jdk8' }"]) {
		sh "$JAVA_HOME/bin/java -jar nohttp.jar -s"
	}
}
