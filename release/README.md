# Release artifact

worlds.jar is the shaded plugin built for Canvas 26.3 build 973 with Java 25.
Every source update must rebuild and replace this file. The release workflow publishes
worlds.jar whenever this artifact changes on main.

The 26.3 Folia implementation uses Canvas internals. Compile the 26.3 module
with the Canvas server JAR and its libraries ahead of the Paper development bundle
on the Java compilation classpath. Do not package those server dependencies.

The latest fix schedules saved level data serialization on the global tick thread.
Compilation succeeded against Canvas 26.3 build 973; runtime verification is pending.
