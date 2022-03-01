# java-word-count-beam

* Follow https://beam.apache.org/get-started/quickstart-java/ page instructions.
* Initially open the powershell administration in 44517 windows file explorer.
* Run the command  :  mvn archetype:generate `
 -D archetypeGroupId=org.apache.beam `
 -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
 -D archetypeVersion=2.36.0 `
 -D groupId=org.example `
 -D artifactId=word-count-beam `
 -D version="0.1" `
 -D package=org.apache.beam.examples `
 -D interactiveMode=false
* New file(word-count-beam) will be uploaded in 44517 folder.
* Run cd .\word-count-beam . This is enter into word-count-beam directory.
* Run dir and dir .\src\main\java\org\apache\beam\examples . Directories information will be listed accordingly.
* Create a text file in the directory. [Sonnets](https://00f74ba44bfa47cef22b7063b644755056a497414d-apidata.googleusercontent.com/download/storage/v1/b/apache-beam-samples/o/shakespeare%2Fsonnets.txt?jk=AFshE3XL7Hz2dROqOfRfTh0fzJETaPBUPJUvSOrvqQB6sMaYABgnv3POdK-IFYMWyIvGfKvEt6E2Xi4FWQ-BBirSwtfe5ut4t0dcvANqTc2DnuBWM48jqrqHMSsRJ6MCj4BhNKcijn-vqbMEPohwzt5xcOACjAUPg7MSIbPYnKs1SQng3isQgoPk5cfSHjywEYJ-gBICLfA0Rf5KsEnwEV-EmchcBdX6chNSNYOw6VEdP7_k2KCGb9e7JqY5Yxa8H-keq9kLFX0EqjD5o4Z6MDS9JljD43EJDpwlPZ-VUSpfmcw0-NWTsLknVKRb6NnpxS3K3YqOwu6YgVGP_9McJBpZhMQ-ujQuXsCT4nYFulG_5Rr7IVUlUzgff9iFnrGbtrU7z8Txs6RBnoIBz6sE0_-3hDCjuIJNz90e0ZiWsOhz-AxBWizlcxeXisI9PFAfOu1FrNgstB-wpRwsmikFE3-X3j_9r7jTz6DcG31m6rr-6KMT4ygMLGzGi5k5ptBSEB76geGVVzd60jszkGNvuaSSaPk5cZk7WtkER9hkQGzfSNVuU8y8xo-KsFQq7C1tq8wEhTHKdkwzKV0nqRQBuBUUqVRraXyamdailGHaDlVmaaRiv5bNg3zJCgeqK7bxWWzAXYQALJuxQiXAgGI0wVa7x4YaboldHJ2vL3R-AC7bOW77tNtgdeCCKOW6bh2O4cESlU9chWRNNnbC8FGhvIRafz8k3GsOK7SZ1KcS1WAXx-EJbWfzaYm3tOOmmzku_KpZvFAFBq6zWU-KpouQvxFu-gnc4NomebnVt3GWVFME38z-tTcsOpt5YikPSvBb1qSUdwtVaI_MX1lH3HfgQUqFrPvt-XaKbTjxpG-54UWjqUVxcjB3-qkfNY6HzsH0B184QYtxxgNsf7hg7w4Vca0j6IxSvfpWKl4MomEmTapXzQtRAfOhoIdcYKW26INr_GxANYQmEJJkDXAcJq2hfhUD-f-w2w&isca=1)
* Now run the pipeline command : mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner
* Inscept the results using command for list counts : ls counts* 
* Run command for more list counts : more counts*
