对于 Java、C、C++ 和 C# 等编译语言，{% data variables.product.prodname_codeql %} 分析在工作流程运行过程中构建的所有代码。 要限制要分析的代码量，请通过在 `run` 块中指定自己的构建步骤，仅构建您要分析的代码。 您可以通过对 `pull_request` 和 `push` 事件使用 `paths` 或 `paths-ignore` 过滤器来组合指定自己的构建步骤，以确保工作流程仅在特定代码发生更改时运行。 更多信息请参阅“[{% data variables.product.prodname_actions %} 的工作流程语法](/actions/reference/workflow-syntax-for-github-actions#onpushpull_requestpull_request_targetpathspaths-ignore)”。

对于 Go、JavaScript、Python 和 TypeScript 等语言， {% data variables.product.prodname_codeql %} 分析而不编译源代码，您可以指定其他配置选项来限制要分析的代码量。 更多信息请参阅“[指定要扫描的目录](/code-security/secure-coding/configuring-code-scanning#specifying-directories-to-scan)”。