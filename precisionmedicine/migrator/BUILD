
package(default_visibility = [ "//visibility:public" ])

java_library(
    name = "migrator",
    srcs = glob(["**/*.java"], exclude = ["**/test/**", "*Test.java"]),
    deps = [
        "@graknlabs_client_java//:client-java",
        "@graknlabs_grakn_core//concept:concept",
        "@graknlabs_grakn_core//common:common",
        "@graknlabs_graql//java:graql",
        "@graknlabs_grakn_core//api:api",

        "//dependencies/maven/artifacts/org/apache/poi:poi-ooxml",
        "//dependencies/maven/artifacts/org/apache/commons:commons-csv",
        "//dependencies/maven/artifacts/edu/stanford/nlp:stanford-corenlp",
        "//dependencies/maven/artifacts/edu/stanford/nlp:stanford-corenlp-java-models",
    ],
    data = [
        "//precisionmedicine/dataset",
        "//precisionmedicine/schema"
    ],
)